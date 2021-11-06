# 實作7: AI-based ES? AI? ML? DL? 要如何入門 (How To Learn)?

## Lab 7-1 在你的Google Drive建立你的第一個Colab Notebook

1. 安裝Colab
2. 新增ES2021的Folder
3. 在此Folder下, 建立你的第一個Colab Notebook (i.e. 'hello-ai'). 將你的Google Drive和Google VM (Virtual Machine)掛接
4. 在你Colab Notebook顯示以下訊息(OOO: 你的英文名字; e.g., Joe biden)
5. 新增文字儲存格 (請用你的英文名字)

### 實作成果

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/140591920-5133e03b-f824-4ff4-af9f-23c1128fad48.png" 
      width="80%" height="80%">
    </div>

## Lab 7-2 暖身: 一起來十分鐘學會Python

### 程式
````python
# task 1: string variable
name = "TA Grace"
print(name)

# task 2: number variable
number = 26
print(number)
print(number*3)
print(number/2)
print(number + number)
print(number - number)

# task 3: function

def printName(firstName, lastName):
  print(lastName + ' ' + firstName)

printName('Grace', 'TA')

# task 4: if else

def printName(firstName, lastName, isCool):
  if isCool:
    print(lastName + ' ' + firstName + ' very cool!')
  else:
    print(lastName + ' ' + firstName + ' not cool!')

# Start
printName('Grace', 'TA', True)
printName('Grace', 'TA', False)

# task 5: for loop

def printName(firstName, lastName, isCool, num):
  for i in range(1, num):
    if isCool:
      print(i, lastName + ' ' + firstName + ' very cool!')
    else:
      print(i, lastName + ' ' + firstName + ' not cool!')

# Start
printName('Grace', 'TA', True, 10)

````

### Task 5的結果

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/140593288-6e469d77-d817-44bd-ba32-ed5d99dd47d5.png" 
      width="50%" height="50%">
    </div>
   

### 我的雲端硬碟/ES2021

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/140593517-4d733763-a3b5-4206-9365-f4056aa57acb.png" 
      width="50%" height="70%">
    </div>
    


