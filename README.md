# python3-learning
step by step(continue updating)
{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## 廖雪峰python3课程笔记"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "#### 2019.2.24 第一个python程序：输出和输入\n",
    "print()和input()"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### 输入：print()\n",
    "参考网址：[廖雪峰] (https://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/001431643484137e38b44e5925440ec8b1e4c70f800b4e2000) [RUBOOB.COM] (http://www.runoob.com/w3cnote/python3-print-func-b.html)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "hello world\n",
      "The quick brown fox jumps over the lazy dog\n",
      "100\n",
      "300\n",
      "100+200= 300\n",
      "ok\n",
      "[1, 2, 'a']\n",
      "(1, 2, 'a')\n",
      "{'a': 1, 'b': 2}\n"
     ]
    }
   ],
   "source": [
    "\"\"\"\n",
    "print() 基本操作：字符串，数字, 其他\n",
    "\"\"\"\n",
    "#1.对字符串\n",
    "print('hello world')\n",
    "print('The quick brown fox', 'jumps over', 'the lazy dog')#print可以接受多个字符串，用逗号“,”隔开，就可以连成一串输出,会依次打印每个字符串,\n",
    "                                                                             # 遇到逗号“,”会输出一个空格\n",
    "#2.也可以打印整数，或者计算结果\n",
    "print(100)\n",
    "print(100+200)\n",
    "print('100+200=',100+200)\n",
    "\n",
    "#3.其他：变量，列表，元组，字典\n",
    "str = 'ok'\n",
    "print(str)     #变量\n",
    "L=[1,2,'a']\n",
    "print(L)       #列表\n",
    "t=(1,2,'a')\n",
    "print(t)        #元组\n",
    "d={'a':1,'b':2}\n",
    "print(d)        #字典"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "the length of (runoob) is 6\n",
      "nHex=ff,nDec=255,nOct=377\n",
      "3.141593\n",
      "     3.142\n",
      "3.142     \n"
     ]
    }
   ],
   "source": [
    "\"\"\"\n",
    "print() 格式化输出：字符串，数字, 其他\n",
    "\"\"\"\n",
    "#1.常用 %s:格式化字符串，%d:格式化整数，%f:格式化浮点数，可指定小数点后的精度\n",
    "print(\"the length of (%s) is %d\" %('runoob',len('runoob')))\n",
    "\n",
    "#2.格式化输出十六进制，十进制，八进制整数\n",
    "\"\"\"\n",
    "%x---hex十六进制\n",
    "%d---dec十进制\n",
    "%o---oct八进制\n",
    "\"\"\"\n",
    "nHex=0xFF\n",
    "print('nHex=%x,nDec=%d,nOct=%o'%(nHex,nHex,nHex))\n",
    "\n",
    "#3.格式化输出浮点数\n",
    "pi=3.141592653\n",
    "print('%f'%pi)\n",
    "print('%10.3f'%pi)    #字段宽10，精度3\n",
    "print('%-10.3f'%pi)  #左对齐"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 20,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0\n",
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "012345"
     ]
    }
   ],
   "source": [
    "\"\"\"\n",
    "在python中print默认是换行的，要不想换行你应该写成print(i,end='')\n",
    "\"\"\"\n",
    "for i in range(6):\n",
    "    print(i)\n",
    "for i in range(6):\n",
    "    print(i,end='')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### 输入 input()\n",
    "参考网址：[廖雪峰] (https://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/001431643484137e38b44e5925440ec8b1e4c70f800b4e2000)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 23,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Alice\n",
      "hello Alice\n",
      "please enter your name:Alicd\n",
      "hello Alicd\n"
     ]
    }
   ],
   "source": [
    "\"\"\"\n",
    "示例：用户把内容输入到name(变量)中\n",
    "\"\"\"\n",
    "name=input()\n",
    "print('hello',name)\n",
    "\n",
    "#更加用户友好地：\n",
    "name=input('please enter your name:')\n",
    "print('hello',name)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
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
   "version": "3.7.1"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
