---
marp: true
math: mathjax
theme: rose-pine
# theme: rose-pine-dawn
# theme: rose-pine-moon
---

<style lang=css>
/*
Rosé Pine theme create by RAINBOWFLESH
> www.rosepinetheme.com

palette in :root
*/

@import "default";
@import "schema";
@import "structure";

:root {
  --base: #232136;
    --surface: #2a273f;
    --overlay: #393552;
    --muted: #6e6a86;
    --subtle: #908caa;
    --text: #e0def4;
    --love: #eb6f92;
    --gold: #f6c177;
    --rose: #ea9a97;
    --pine: #3e8fb0;
    --foam: #9ccfd8;
    --iris: #c4a7e7;
    --highlight-low: #2a283e;
    --highlight-muted: #44415a;
    --highlight-high: #56526e;

  font-family: Pier Sans, ui-sans-serif, system-ui, -apple-system,
    BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", Segoe UI Symbol,
    "Noto Color Emoji";
  font-weight: initial;

  background-color: var(--base);
}
/*Common style*/
h1 {
  color: var(--rose);
  padding-bottom: 2mm;
  margin-bottom: 12mm;
}
h2 {
  color: var(--rose);
}
h3 {
  color: var(--rose);
}
h4 {
  color: var(--rose);
}
h5 {
  color: var(--rose);
}
h6 {
  color: var(--rose);
}
a {
  color: var(--iris);
}
p {
  font-size: 20pt;
  font-weight: 600;
  color: var(--text);
}
code {
  color: var(--text);
  background-color: var(--highlight-muted);
}
text {
  color: var(--text);
}
ul {
  color: var(--subtle);
}
li {
  color: var(--subtle);
}
img {
  background-color: var(--highlight-low);
}
strong {
  color: var(--text);
  font-weight: inherit;
  font-weight: 800;
}
mjx-container {
  color: var(--text);
}
marp-pre {
  background-color: var(--overlay);
  border-color: var(--highlight-high);
}

/*Code blok*/
.hljs-comment {
  color: var(--muted);
}
.hljs-attr {
  color: var(--foam);
}
.hljs-punctuation {
  color: var(--subtle);
}
.hljs-string {
  color: var(--gold);
}
.hljs-title {
  color: var(--foam);
}
.hljs-keyword {
  color: var(--pine);
}
.hljs-variable {
  color: var(--text);
}
.hljs-literal {
  color: var(--rose);
}
.hljs-type {
  color: var(--love);
}
.hljs-number {
  color: var(--gold);
}
.hljs-built_in {
  color: var(--love);
}
.hljs-params {
  color: var(--iris);
}
.hljs-symbol {
  color: var(--foam);
}
.hljs-meta {
  color: var(--subtle);
}

</style>

# Let's begin wit H1 title

Start writing!
<!-- 111 i am comment -->
*I am italic*

> I am `note` ,,, ... """''';;;:::<><>??!~!#@$!^%&%*()"

1. ww
2. 22

- $\sqrt{1+x} = {(1+x)}^\frac{1}{2} = 1+\frac{1}{2x}+o{x}$
**I am blob**

<https://marp.app>

---

## How to use

Put this to vscode setting

```json
{
    // etc...
    "markdown.marp.themes": [
      "https://raw.githubusercontent.com/rainbowflesh/Marp/master/css/rosepine-dawn.css",
      "https://raw.githubusercontent.com/rainbowflesh/Marp/master/css/rosepine-moon.css",
      "https://raw.githubusercontent.com/rainbowflesh/Marp/master/css/rosepine.css",
    ]
    // etc...
}
```

### I am H3 Title

#### I am H4

##### H5?

###### H6 juesus

---

## Test code block color

Pythong

```python
class test_class
def __superIdol
    # A very super function
    with open("myfile.txt", "r", encoding='utf8') as file:
    for line in file:
        print(line)
    return Null
```

---
Jvav

```java
public class Hello {
  // main method
  public static void main(String[] args)
  {
    // Output: Hello, world!
    System.out.println("Hello, world!");
  }
}
```

---
TypeScript

```typescript
mounted() {
    console.log("Wanna try something big? y/n");
    console.log("%c >> n", "color:red");
  }
```

---
JavaScript

```javascript
// Named function
function rocketToMars() {
  return 'BOOM!';
}
const sum = (param1, param2) => {
  return param1 + param2;
};
console.log(sum(2,5)); // => 7
```

---
Bash

```bash
echo "wtf"
```

---
Rust

```rust
fn main(){
  let mut array: [i32 ; 5] = [1,2,3,4,6];
  let mut boo: true
  print_arrays(array);
  println!("The elements: {array:?}");
}

fn print_arrays(mut array:[i32; 5]) {
  array[0] = 89;
  array[1] = 90;
  array[2] = 91;
  array[3] = 92;
  array[4] = 93;
  println!("The elements: {array:?}");
}
```

---

Ruby

```ruby
class Person < ApplicationRecord
  validates :name, presence: true
end

```

---
C++++

```csharp
class Hello {
  // main method
  static void Main(string[] args)
  {
    // Output: Hello, world!
    Console.WriteLine("Hello, world!");
  }
}
```

---
PowerShell

```powershell
# Clock down
echo starting...
echo 'Please close manually if the windows no response.'
# Boot app
C:\Users\isri\AppData\Local\Microsoft\WindowsApps\MicrosoftCorporationII.WindowsSubsystemForAndroid_8wekyb3d8bbwe\WsaClient.exe /launch wsa://com.teslacoilsw.launcher
echo 'app started'
adb connect 127.0.0.1:58526

# Get host ipv4
echo 'getting host ipv4...'
$MyIpv4 = Get-netipAddress | Where-Object {
  $_.InterfaceAlias -eq 'Wi-Fi' -and $_.AddressFamily -eq 'IPv4'
} | Select-Object IPAddress | Format-Table -HideTableHeaders | Out-String
$MyIpv4 = $MyIpv4.Trim()

# Set port
$MyPort = 10809
# Set Porxyaddr
$Porxyaddr = $MyIpv4+':'+$MyPort
# Set following proxy
adb shell settings put global http_proxy $Porxyaddr

echo 'The following proxy is'
adb shell settings get global http_proxy
Timeout /T 3
exit
```

---
Cpp

```cpp
#include <iostream>
using namespace std;
int main()
{
    cout << "Hello, world!" << endl;
    return 0;
}
```

---
Golang

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

---
Haskell

```hs
"hello" == "hello world"
```

---
SQL

```sql
create database world;
use world;
create table hello (
    id int not null auto_increment,
    name varchar(255) not null,
    primary key (id)
);
```

---

# Another readme.md

[![npm](https://98badges.now.sh/api/version)](1)
[![gzip size](https://98badges.now.sh/api/size)](https://unpkg.com/98.css)
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Best-README-Template</h3>

  <p align="center">
    An awesome README template to jumpstart your projects!
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</div>

---

Blog page resource [repo](https://github.com/rainbowflesh/rainbowflesh.github.io).

## Dev

I recommend use `pnpm` to manage package.

### Initialization

```shell
pnpm i
```

---

### Run dev

```shell
pnpm dev
```

### Build

```shell
pnpm build
```

### Deploy

```shell
bash ../.github/workflows/deploy.sh
```

> note: You need change username to yours.
---

## WIP

## TODO

TODO: blog add kismet deploy

TODO: blog add blog creation

TODO: import 7.css, xp.css, 98.css, ios7.css

TODO: import suanming
