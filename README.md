# Реализация дерева на базе AbstractList.

## Поля класса, описывающего тип элементов дерева:
- String elementName
- boolean availableToAddLeftChildren, availableToAddRightChildren
- Entry<T> parent, leftChild, rightChild

## Методы:
1) add(String s) - добавляет элементы дерева, искать место для вставки начинает слева направо
2) size() - возвращает текущее количество элементов в дереве
3) getParent(String s) - возвращает имя родителя элемента дерева
4) remove(Object o) - удаляет элемента дерева. Если в дереве присутствует несколько элементов с переданным именем - удаляет только первый найденный.
Если переданный объект не является строкой, метод должен бросить UnsupportedOperationException.

Для удобства реализован итератьор по коллекции
  
1) public String get(int index)
2) public String set(int index, String element)
3) public void add(int index, String element)
4) public String remove(int index)
5) public List<String> subList(int fromIndex, int toIndex)
6) protected void removeRange(int fromIndex, int toIndex)
7) public boolean addAll(int index, Collection<? extends String> c)
