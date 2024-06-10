#define SIZE 10
int hash_table[SIZE];

void insert(int key) {
    int index = key % SIZE;
    while (hash_table[index] != 0) {
        index = (index + 1) % SIZE;
    }
    hash_table[index] = key;
}
