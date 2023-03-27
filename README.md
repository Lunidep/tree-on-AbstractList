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

public String get(int index)
public String set(int index, String element)
public void add(int index, String element)
public String remove(int index)
public List<String> subList(int fromIndex, int toIndex)
protected void removeRange(int fromIndex, int toIndex)
public boolean addAll(int index, Collection<? extends String> c)
