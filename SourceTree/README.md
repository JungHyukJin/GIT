# SourceTree - CLI					   - 2020.02.10

- unstaged(working copy) : 수정된 파일들의 리스트가 표시되는 공간
- staged (index *or* staging area) : 중간단계, 커밋 시 만들어질 버전에 합류할 파일들을 모아놓은 공간
- add : unstaged 파일들을 staged에 올리는 작업
- history : 버전들이 표시되는 타임라인

> 즉, working copy에 있는 작업들을 add를 통해 index or staging are에 올린 후, commit을 통해 하나의 버전을 만들어 repository에 저장한다. 이 후에 history 타임라인에 최신버전부터 위쪽에 표시됨.
>
> 커밋전에 수정사항 취소 후 되돌리기 가능.
>
> commit 전에 현재까지 작업한 내역을 review 하는 버릇을 가지자.

---

- Revert(Reverse): 선택한 버전은 취소한 뒤 남겨두고, 이전버전으로 돌아간다.
  - 취소할 선택버전을 남겨둔 체, 직전 버전을 (Revert+취소버전)이라는 이름으로 새로운 버전을 만든다.
  - 최근버전부터 순차적으로 선택한 버전을 취소하고, Revert로 새로 만들어 남긴 체 직전 버전으로 돌아간다. 순차적으로 취소하지 않을 경우 충돌이 발생할 수 있다.

- Reset: 선택버전 이후의 버전들은 모두 삭제하고, 선택한 버전으로 돌아간다. 파일 유지만 Hard(삭제) or Mixed(유지)로 결정.
  - Reset - hard: 선택한 버전으로 돌아가고, 현재 파일상태와 상관없이 그 이후의 버전 + 파일 전부 삭제.
  - Reset - mixed: 선택한 버전으로 돌아가고, 현재 파일 상태는 uncommited changes로 남긴다.
- Discard: 현재 파일 수정 후 저장된 상태에서, commit을 하지 않았다면, 다시 직전의 파일로 돌아갈 수 있다.