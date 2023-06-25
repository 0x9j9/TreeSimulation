# TreeSimulation
这个代码库包含了一个简单的Python程序，用于模拟小树的生长过程。通过该程序，你可以观察到树的生长过程以及树干、树枝和叶子的形成。
import time

def grow_tree(height):
    for i in range(height):
        print(' ' * (height - i - 1) + '*' * (2 * i + 1))
        time.sleep(0.5)  # 控制打印速度，可调整时间间隔

    print(' ' * (height - 1) + '|')
    time.sleep(0.5)

    for _ in range(3):
        print(' ' * (height - 2) + '|||')
        time.sleep(0.5)

    print(' ' * (height - 2) + '~~~')
    time.sleep(0.5)

    for _ in range(3):
        print(' ' * (height - 2) + '|||')
        time.sleep(0.5)

    print(' ' * (height - 1) + '|')
    time.sleep(0.5)

    print(' ' * (height - 1) + '|')

# 在这里调用函数，传入树的高度参数
grow_tree(5)
