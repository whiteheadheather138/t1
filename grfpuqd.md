代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://cu.zhonguo4118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://my.zhonguo5118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://uk.zhonguo3118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://gw.zhonguo3118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://zy.zhonguo3118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://fg.zhonguo2118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://dy.zhonguo5118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ul.zhonguo8118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://qb.zhonguo1118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://sk.zhonguo3118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://dk.zhonguo3118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://zl.zhonguo8118.cn

================================================================================
来源：https://fm.zhonguo2118.cn

A. 基础语法与类型
来源：https://ij.zhonguo7118.cn

================================================================================
来源：https://zn.zhonguo6118.cn

[A01] Hello World
来源：https://ia.zhonguo3118.cn

Py:   print("Hello, World!")
来源：https://dp.zhonguo6118.cn

PHP:  echo "Hello, World!";
来源：https://gs.zhonguo7118.cn

JS:   console.log("Hello, World!");
来源：https://eg.zhonguo1118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://lh.zhonguo6118.cn

Java: System.out.println("Hello, World!");
来源：https://by.zhonguo2118.cn

Go:   fmt.Println("Hello, World!")
来源：https://rs.zhonguo4118.cn

Ruby: puts "Hello, World!"
来源：https://ss.zhonguo7118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://gj.zhonguo4118.cn

[A02] 变量声明与赋值
来源：https://hr.zhonguo1118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://ff.zhonguo5118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://xx.zhonguo8118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://tw.zhonguo4118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://at.zhonguo1118.cn

Java: String name = "Alex"; int age = 20;
来源：https://yh.zhonguo6118.cn

Go:   name := "Alex"; age := 20
来源：https://al.zhonguo3118.cn

Ruby: name = "Alex"; age = 20
来源：https://lh.zhonguo6118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://sm.zhonguo5118.cn

[A03] 常量定义
来源：https://yo.zhonguo8118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://xa.zhonguo8118.cn

PHP:  const PI = 3.14159;
来源：https://gl.zhonguo2118.cn

JS:   const PI = 3.14159;
来源：https://so.zhonguo1118.cn

TS:   const PI: number = 3.14159;
来源：https://jv.zhonguo7118.cn

Java: static final double PI = 3.14159;
来源：https://mp.zhonguo4118.cn

Go:   const PI = 3.14159
来源：https://lr.zhonguo5118.cn

Ruby: PI = 3.14159
来源：https://dp.zhonguo3118.cn

C#:   const double PI = 3.14159;
来源：https://nl.zhonguo2118.cn

[A04] 判断变量类型
来源：https://za.zhonguo7118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://bz.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://vr.zhonguo1118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://qd.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://mb.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://ox.zhonguo2118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://jf.zhonguo3118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://ns.zhonguo5118.cn

C#:   x.GetType().Name; x is int
来源：https://ul.zhonguo8118.cn

[A05] 整数除法与取模
来源：https://hf.zhonguo8118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://cz.zhonguo1118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://fw.zhonguo5118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://qf.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://sm.zhonguo3118.cn

Java: 7 / 2; 7 % 2
来源：https://il.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://yk.zhonguo4118.cn

Ruby: 7 / 2; 7 % 2
来源：https://av.zhonguo6118.cn

C#:   7 / 2; 7 % 2
来源：https://ug.zhonguo2118.cn

[A06] 字符串转数字
来源：https://ro.zhonguo1118.cn

Py:   int("42"); float("3.14")
来源：https://au.zhonguo3118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://wl.zhonguo3118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://qw.zhonguo2118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://or.zhonguo4118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://zb.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://xx.zhonguo2118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://mo.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://wx.zhonguo7118.cn

[A07] 数字转字符串
来源：https://jo.zhonguo6118.cn

Py:   str(42)
来源：https://go.zhonguo2118.cn

PHP:  (string) 42; strval(42)
来源：https://ie.zhonguo3118.cn

JS:   String(42); (42).toString()
来源：https://tb.zhonguo1118.cn

TS:   String(42)
来源：https://la.zhonguo4118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://ns.zhonguo2118.cn

Go:   strconv.Itoa(42)
来源：https://sb.zhonguo1118.cn

Ruby: 42.to_s
来源：https://wf.zhonguo1118.cn

C#:   42.ToString()
来源：https://qi.zhonguo7118.cn

[A08] 取整与四舍五入
来源：https://vx.zhonguo6118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://rz.zhonguo3118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://sm.zhonguo6118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://uz.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://va.zhonguo5118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://cv.zhonguo4118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://xa.zhonguo1118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://db.zhonguo7118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://xu.zhonguo2118.cn

[A09] 绝对值与最大最小值
来源：https://ee.zhonguo1118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ib.zhonguo1118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://zp.zhonguo3118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://nw.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ga.zhonguo8118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://ku.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://ut.zhonguo5118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://jg.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ru.zhonguo2118.cn

[A10] 生成随机数
来源：https://km.zhonguo4118.cn

Py:   import random; random.randint(1, 100)
来源：https://og.zhonguo5118.cn

PHP:  random_int(1, 100);
来源：https://uh.zhonguo3118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://nn.zhonguo2118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://xs.zhonguo4118.cn

Java: new Random().nextInt(100) + 1
来源：https://gl.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://hf.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://iu.zhonguo2118.cn

C#:   new Random().Next(1, 101)
来源：https://jw.zhonguo2118.cn

[A11] 条件表达式（三元）
来源：https://af.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ui.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://gy.zhonguo8118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://pd.zhonguo1118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://at.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://xu.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ua.zhonguo6118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://pe.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://dz.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://kr.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://pr.zhonguo5118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://qm.zhonguo6118.cn

JS:   `Hello, ${name}!`
来源：https://eu.zhonguo7118.cn

TS:   `Hello, ${name}!`
来源：https://hk.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://mj.zhonguo6118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://nw.zhonguo2118.cn

Ruby: "Hello, #{name}!"
来源：https://uy.zhonguo5118.cn

C#:   $"Hello, {name}!"
来源：https://es.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://zs.zhonguo1118.cn

Py:   "第一行\n第二行"
来源：https://qv.zhonguo3118.cn

PHP:  "第一行\n第二行"
来源：https://ei.zhonguo1118.cn

JS:   "第一行\n第二行"
来源：https://mk.zhonguo6118.cn

TS:   "第一行\n第二行"
来源：https://nc.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://vl.zhonguo4118.cn

Go:   "第一行\n第二行"
来源：https://js.zhonguo5118.cn

Ruby: "第一行\n第二行"
来源：https://mi.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://gu.zhonguo8118.cn

[A14] 注释写法
来源：https://yn.zhonguo5118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ki.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://im.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://dd.zhonguo5118.cn

TS:   // 单行；/* 多行 */
来源：https://lf.zhonguo5118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ws.zhonguo1118.cn

Go:   // 单行；/* 多行 */
来源：https://xd.zhonguo3118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://dj.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://ug.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://iu.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://ly.zhonguo4118.cn

PHP:  $value = $data ?? "默认值";
来源：https://vc.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://za.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://au.zhonguo2118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://em.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://am.zhonguo3118.cn

Ruby: value = data || "默认值"
来源：https://eq.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://ie.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://ow.zhonguo1118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://yg.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://yd.zhonguo4118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://rr.zhonguo6118.cn

TS:   if (!x) {}
来源：https://oo.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://nl.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://ad.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ib.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://xg.zhonguo2118.cn

[A17] 位运算
来源：https://nx.zhonguo7118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://oy.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ny.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://bq.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ty.zhonguo5118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://th.zhonguo1118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://dw.zhonguo1118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zd.zhonguo1118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wj.zhonguo2118.cn

[A18] 字符与 ASCII 码互转
来源：https://mi.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://ey.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://ep.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://wt.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://cw.zhonguo1118.cn

Java: (int) 'A'; (char) 65
来源：https://qi.zhonguo3118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://gf.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://ec.zhonguo8118.cn

C#:   (int)'A'; (char)65
来源：https://be.zhonguo8118.cn

[A19] 交换两个变量
来源：https://do.zhonguo3118.cn

Py:   a, b = b, a
来源：https://ki.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ac.zhonguo1118.cn

JS:   [a, b] = [b, a];
来源：https://vk.zhonguo4118.cn

TS:   [a, b] = [b, a];
来源：https://xl.zhonguo3118.cn

Java: int t = a; a = b; b = t;
来源：https://dm.zhonguo5118.cn

Go:   a, b = b, a
来源：https://mf.zhonguo6118.cn

Ruby: a, b = b, a
来源：https://ri.zhonguo2118.cn

C#:   (a, b) = (b, a);
来源：https://ni.zhonguo1118.cn

[A20] 读取标准输入
来源：https://dn.zhonguo2118.cn

Py:   name = input("请输入：")
来源：https://os.zhonguo8118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://em.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://dp.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://ew.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://cm.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ia.zhonguo2118.cn

Ruby: gets.chomp
来源：https://ny.zhonguo6118.cn

C#:   Console.ReadLine();
来源：https://qm.zhonguo1118.cn

[A21] 保留指定小数位输出
来源：https://bj.zhonguo5118.cn

Py:   f"{3.14159:.2f}"
来源：https://xa.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://tp.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://zy.zhonguo6118.cn

TS:   (3.14159).toFixed(2)
来源：https://on.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ky.zhonguo5118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://jp.zhonguo1118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ug.zhonguo2118.cn

C#:   3.14159.ToString("F2")
来源：https://us.zhonguo6118.cn

[A22] 获取字符串长度
来源：https://gs.zhonguo1118.cn

Py:   len(s)
来源：https://hv.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://qb.zhonguo1118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://sm.zhonguo8118.cn

TS:   s.length
来源：https://yq.zhonguo1118.cn

Java: s.length()
来源：https://gt.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://ca.zhonguo8118.cn

Ruby: s.length
来源：https://pa.zhonguo3118.cn

C#:   s.Length
来源：https://tc.zhonguo4118.cn

[A23] 大小写转换
来源：https://gv.zhonguo6118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://sd.zhonguo3118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://cx.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://qd.zhonguo6118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://xx.zhonguo5118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ke.zhonguo1118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://fl.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://vm.zhonguo6118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://bx.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://ht.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://yb.zhonguo2118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://mi.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://yr.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://zs.zhonguo6118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://hu.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://kk.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://xc.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://kn.zhonguo1118.cn

[A25] 字符串比较
来源：https://yk.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://ni.zhonguo3118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://gx.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ce.zhonguo3118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://mo.zhonguo8118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://io.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://yk.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://vm.zhonguo7118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://js.zhonguo6118.cn

[A26] 类型转换总览
来源：https://ga.zhonguo8118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://pi.zhonguo7118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://pb.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://gs.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://tp.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://ou.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://fx.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://kg.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://sv.zhonguo3118.cn

================================================================================
来源：https://ko.zhonguo2118.cn

B. 流程控制
来源：https://id.zhonguo2118.cn

================================================================================
来源：https://ve.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://mh.zhonguo1118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://nb.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://nl.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://zr.zhonguo5118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://bx.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://pz.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://oy.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://un.zhonguo6118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://jw.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://lz.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://qy.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://fo.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://yh.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://my.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cg.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://mx.zhonguo3118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://vo.zhonguo8118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://st.zhonguo1118.cn

[B03] switch / match / case
来源：https://zh.zhonguo3118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://hx.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://xc.zhonguo4118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://xj.zhonguo3118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://uv.zhonguo5118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://oz.zhonguo7118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ny.zhonguo7118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://vx.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://cq.zhonguo7118.cn

[B04] for 计数循环
来源：https://jx.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://dh.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://rl.zhonguo1118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://uj.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://kj.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ly.zhonguo6118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://lx.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://ev.zhonguo2118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://de.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://rf.zhonguo7118.cn

Py:   for item in arr: print(item)
来源：https://nc.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://vt.zhonguo4118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://bw.zhonguo1118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://uz.zhonguo3118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://vu.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://lf.zhonguo6118.cn

Ruby: arr.each { |item| puts item }
来源：https://mx.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://zw.zhonguo6118.cn

[B06] 遍历字典 / 对象
来源：https://wf.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ir.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://el.zhonguo3118.cn


<!-- 参考信息 -->