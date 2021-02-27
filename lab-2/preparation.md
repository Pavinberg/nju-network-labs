# Task 1: Preparation

There is an example of a switch without learning implemented in `switchyard/examples/exercises/learning_switch/myswitch.py`. Let's start with it.

1. Create a directory named `lab_2` in `switchyard`.
2. Copy `examples/exercises/learning_switch/switchtopo.py` to `lab_2/start_mininet.py`.
3. Make 4 copies of `examples/exercises/learning_switch/myswitch.py` to:
   1. `lab_2/myswitch.py`: Your basic learning switch.
   2. `lab_2/myswitch_to.py`: Your learning switch with timeout based entry removal.
   3. `lab_2/myswitch_lru.py`: Your learning switch with LRU based entry removal.
   4. `lab_2/myswitch_traffic.py`: Your learning switch with traffic volume based entry removal.
4. \(Optional\) Create your test files in `lab_2`.
   1. `lab_2/mytests.py`: Your test file of `lab_2/myswitch.py`.
   2. `lab_2/mytests_to.py`: Your test file of `lab_2/myswitch_to.py`.
   3. `lab_2/mytests_lru.py`: Your test file of `lab_2/myswitch_lru.py`.
   4. `lab_2/mytests_traffic.py`: Your test file of `lab_2/myswitch_traffic.py`.

Though we will provide the test files, they are incomprehensible. So you should still write test scenarios that test all aspects of your code. You can find our test files below. Download it and you will use it to test your switch later. You can unzip the test files we provide into the folder `lab_2`.

[Download compiled test cases here](https://box.nju.edu.cn/d/123a70ac8ff34595b18f/).

Finally, your project will look like

```text
switchyard
  ├─docs/
  ├─.../
+ ├─lab_2/
+ │ ├─myswitch.py
+ │ ├─myswitch_to.py
+ │ ├─myswitch_lru.py
+ │ ├─myswitch_traffic.py
  │ ├─...
+ │ └─start_mininet.py
  ├─.gitignore
  └─...
```

{% hint style="warning" %}
All of your modifications should be done on the files under your directory `lab_2`. We will check and compare the **git commits** to judge the originality of your work. So remember to commit every time you complete one small task.
{% endhint %}

