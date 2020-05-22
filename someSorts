
class Sorts:
    def __init__(self, array, n):
        self.array = array
        self.n = n

    def gnomeSort(self):
        index = 0
        while index < n:
            if index == 0:
                index = index + 1
            if array[index] >= array[index - 1]:
                index = index + 1
            else:
                array[index], array[index - 1] = array[index - 1], array[index]
                index = index - 1

        return array

    def insertionSort(self):
        for i in range(1, n):
            key = array[i]
            j = i - 1
            while j >= 0 and key < array[j]:
                array[j + 1] = array[j]
                j -= 1
            array[j + 1] = key

        return array

    def selectionSort(self):
        for i in range(len(array)):
            index = i
            for j in range(i + 1, n):
                if array[index] > array[j]:
                    index = j

            array[i], array[index] = array[index], array[i]

        return array

    def bubbleSort(self):
        for i in range(n):
            for j in range(0, n - i - 1):
                if array[j] > array[j + 1]:
                    array[j], array[j + 1] = array[j + 1], array[j]

        return array


if __name__ == '__main__':

    array = [5,1,8,3,0,2,56,78,12,23,34,45,56,14,69]
    n = len(array)
    f1 = Sorts(array, n)
    gnomeArray = f1.gnomeSort();
    insertionArray = f1.insertionSort();
    selectionArray = f1.selectionSort();
    bubbleArray = f1.bubbleSort();

    print("Using Gnome Sort: ", gnomeArray)
    print("Using Insertion Sort: ", insertionArray)
    print("Using Selection Sort: ", selectionArray)
    print("Using Bubble Sort: ", bubbleArray)

