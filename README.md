from copy import deepcopy
from random import randint


def shuffle(arr):
    temp_arr = deepcopy(arr)
    m = len(temp_arr)
    while (m):
        m -= 1
        i = randint(0, m)
        temp_arr[m], temp_arr[i] = temp_arr[i], temp_arr[m]
    return temp_arr
function switchTheme() {
  wrapper.classList.toggle('dark-theme')
  wrapper.classList.toggle('light-theme')

  if (wrapper.classList.contains('dark-theme')) {
    localStorage.setItem('theme', 'dark')
  } else {
    localStorage.setItem('theme', 'light')
  }
}

if (localStorage.getItem('theme') == 'dark') {
  themeSwitcher.setAttribute('checked', '')
  switchTheme()
} else {
  themeSwitcher.removeAttribute('checked')
}

themeSwitcher.addEventListener('click', switchTheme)
from math import floor
difference_by([2.1, 1.2], [2.3, 3.4],floor) # [1.2]
difference_by([{ 'x': 2 }, { 'x': 1 }], [{ 'x': 1 }], lambda v : v['x']) # [ { x: 2 } ]

.wrap {
  filter: drop-shadow(0 0 10px gray);
}

.element {
  display: inline-block;
  width: 111px;
  height: 111px;
  background-color: #fff;
  border-radius: 2em;
}
