## revert & reset
### revert

```bash
# 특정 commit을 없던 일로 만드는 작업
git revert <commit id>
```

- 의미 
  - 과거의 commit 개수를 유지하면서 이전 변경사항을 지운 결과만 새로운 commit으로 생성
- commit의 개수를 유지시키는 이유
  - commit은 이전 commit에 종속되어 있어, 변경시 문제 발생 가능
  - 협업 시, 문제가 발생하지 않도록 하기 위함함


### reset

```bash
# 특정 commit으로 되돌아가는 작업, 되돌아 간 이후의 commit은 모두 삭제
git reset [옵션] <commit id>
```

- 의미
  - 옵션 수준에 따라 삭제된 commit들에 대한 단계를 설정 가능
- 옵션
  - soft
    - 삭제된 commit의 기록을 staging area에 남김
  - mixed
    - 삭제된 commit의 기록을 working directory에 남김 (디폴트)
  - hard
    - 삭제된 commit의 기록을 남기지 않음