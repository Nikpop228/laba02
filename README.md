# laba02

## Домашнее задание 2

## Part I

***Студента группы ИУ8-23***

***Попова Николая***

1. Создайте пустой репозиторий на сервисе github.com (или gitlab.com, или bitbucket.com).
2. Выполните инструкцию по созданию первого коммита на странице репозитория, созданного на предыдещем шаге.
```sh
  $ cd ${GITHUB_USERNAME}/workspace/projects
  $ mkdir lab02
  $ cd lab02
  $ git init
  hint: Using 'master' as the name for the initial branch. This default branch name
  hint: is subject to change. To configure the initial branch name to use in all
  hint: of your new repositories, which will suppress this warning, call:
  hint:
  hint:   git config --global init.defaultBranch <name>
  hint:
  hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
  hint: 'development'. The just-created branch can be renamed via this command:
  hint:
  hint:   git branch -m <name>
  Initialized empty Git repository in /home/nikpop228/Nikpop228/workspace/projects/laba02/.git/
  $ echo "# laba02" >> README.md
  $ git add README.md
  $ git remote add origin https://github.com/Nikpop228/laba02.git
  $ git add README.md
  $ git commit -m "README.md added"
  -m "README.md added"
  [master (root-commit) 9e3e311] README.md added
  1 file changed, 1 insertion(+)
  create mode 100644 README.md
  $ git push origin master
  Username for 'https://github.com': Nikpop228
  Password for 'https://Nikpop228@github.com':
  Enumerating objects: 3, done.
  Counting objects: 100% (3/3), done.
  Writing objects: 100% (3/3), 231 bytes | 231.00 KiB/s, done.
  Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
  To https://github.com/Nikpop228/laba02.git
   * [new branch]      master -> master
```
3. Создайте файл `hello_world.cpp` в локальной копии репозитория (который должен был появиться на шаге 2). Реализуйте программу **Hello world** на языке C++ используя плохой стиль кода. Например, после заголовочных файлов вставьте строку `using namespace std;`.
```sh
  $ touch hello_world.cpp
  $ cat > hello_world.cpp << EOF
  > #include <iostream>
  > using namespace std;
  >
  > int main()
  > {
  > cout << "Hello world!";
  > }
  > EOF
  $ git add hello_world.cpp
  $ git commit -m "Hello world had created"
  [master ac43ad7] Hello world had created
   1 file changed, 7 insertions(+)
   create mode 100644 hello_world.cpp
  $ vim hello_world.cpp
  $ git commit -m "from @name had added to file" -a
  [master b77868a] from @name had added to file
   1 file changed, 1 insertion(+), 1 deletion(-)
  $ git push origin master
  Username for 'https://github.com': Nikpop228
  Password for 'https://Nikpop228@github.com':
  Enumerating objects: 7, done.
  Counting objects: 100% (7/7), done.
  Delta compression using up to 16 threads
  Compressing objects: 100% (6/6), done.
  Writing objects: 100% (6/6), 662 bytes | 331.00 KiB/s, done.
  Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
  remote: Resolving deltas: 100% (1/1), done.
  To https://github.com/Nikpop228/laba02.git
     9e3e311..b77868a  master -> master