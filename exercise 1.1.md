{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 42,
   "id": "99c1e4c1",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "C:\\Users\\ksm94\n"
     ]
    }
   ],
   "source": [
    "cd"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 46,
   "id": "a82baa21",
   "metadata": {},
   "outputs": [],
   "source": [
    "mkdir myfolder"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 55,
   "id": "c5ae9632",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "C:\\Users\\ksm94\\myfolder\n"
     ]
    }
   ],
   "source": [
    "cd myfolder"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 57,
   "id": "f511eece",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "'C:\\\\Users\\\\ksm94\\\\myfolder'"
      ]
     },
     "execution_count": 57,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "pwd"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 61,
   "id": "b451fed0",
   "metadata": {},
   "outputs": [],
   "source": [
    "f = open('test.txt', 'w')\n",
    "f.write(\"Hello World\")\n",
    "f.close()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 67,
   "id": "c725bd25",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      " C 드라이브의 볼륨에는 이름이 없습니다.\n",
      " 볼륨 일련 번호: 089B-9171\n",
      "\n",
      " C:\\Users\\ksm94\\myfolder 디렉터리\n",
      "\n",
      "2022-03-08  오후 08:40    <DIR>          .\n",
      "2022-03-08  오후 08:40    <DIR>          ..\n",
      "2022-03-08  오후 08:45                11 test.txt\n",
      "               1개 파일                  11 바이트\n",
      "               2개 디렉터리  97,724,715,008 바이트 남음\n"
     ]
    }
   ],
   "source": [
    "!dir"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 104,
   "id": "650f0910",
   "metadata": {},
   "outputs": [],
   "source": [
    "%more test.txt"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 106,
   "id": "0b236ce7",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Hello World\n"
     ]
    }
   ],
   "source": [
    "f = open('test.txt','r')\n",
    "print(f.read())\n",
    "f.close()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 124,
   "id": "68052dd7",
   "metadata": {},
   "outputs": [
    {
     "ename": "PermissionError",
     "evalue": "[WinError 32] 다른 프로세스가 파일을 사용 중이기 때문에 프로세스가 액세스 할 수 없습니다: 'test.txt'",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mPermissionError\u001b[0m                           Traceback (most recent call last)",
      "\u001b[1;32m~\\AppData\\Local\\Temp/ipykernel_24572/363473314.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[1;32mimport\u001b[0m \u001b[0mos\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0;32m      2\u001b[0m \u001b[1;33m\u001b[0m\u001b[0m\n\u001b[1;32m----> 3\u001b[1;33m \u001b[0mos\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0munlink\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;34m'test.txt'\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mPermissionError\u001b[0m: [WinError 32] 다른 프로세스가 파일을 사용 중이기 때문에 프로세스가 액세스 할 수 없습니다: 'test.txt'"
     ]
    }
   ],
   "source": [
    "import os\n",
    "    \n",
    "os.unlink('test.txt')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 125,
   "id": "010fc38a",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "C:\\Users\\ksm94\n"
     ]
    }
   ],
   "source": [
    "cd"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 126,
   "id": "156ae392",
   "metadata": {},
   "outputs": [
    {
     "name": "stderr",
     "output_type": "stream",
     "text": [
      "디렉터리가 비어 있지 않습니다.\n"
     ]
    }
   ],
   "source": [
    "rmdir myfolder"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
