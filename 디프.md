### git stash

커밋할 필요 없이 파일을 변경 하려고 하거나, 변경 사항을 숨기면서 저장할 수 있는 도구입니다.

- `git log --all` 로 확인 시 stash 정보도 나온다.

```bash
git stash                    # wa, sa 임시 저장 및 wd, sa 수정 사항 지우기
git stash -u                 # untracked 파일까지 임시 저장하기
git stash list               # stash 목록 확인하기
git stash show               # stash와 현재 디렉터리의 차이 알아보기
git stash show -p            # 차이를 더 자세히 보기
git stash show -p stash@{1}  # 1번째 index의 stash 와 wd 차이 보기

# pop
git stash pop                # 임시로 저장한 wd 불러오기 (stash 목록에서 빠짐)
git stash pop --index        # wd와 sa 까지 이동 적용하기

# apply
git stash apply              # 임시로 저장한 wd 불러오기 (stash 목록 유지)
git stash apply --index      # wd와 sa 까지 복사 적용하기

# keep index
git stash --keep-index       # sa는 유지하고 wd만 복사함

git stash branch [브랜치명]    # 브랜치 생성 및 해당 브랜치에 wd, sa, ut 복사

git stash clear              # stash list 삭제하기
```

### git clean

```bash
git clean     # ut 파일 삭제하기 (삭제 안됨)
git clean -f  # ut 파일 강제 삭제하기
git clean -n  # ut 파일 목록 확인하기
git clean -i  # 대화모드로 삭제하기
# Would remove the following item:
# [삭제 목록]
# *** Commands ***
# 1: clean                2: filter by pattern    3: select by numbers
# 4: ask each             5: quit                 6: help
```
