代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://wr.zhonguo2118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://bw.zhonguo6118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://cb.zhonguo5118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://by.zhonguo2118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://wf.zhonguo6118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://bz.zhonguo5118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://pb.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://vw.zhonguo8118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://ir.zhonguo8118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://pi.zhonguo2118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://uz.zhonguo2118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ls.zhonguo8118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://mu.zhonguo3118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://lt.zhonguo8118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://ye.zhonguo6118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://uk.zhonguo4118.cn

================================================================================
来源：https://ve.zhonguo4118.cn

A. 基础语法与类型
来源：https://ic.zhonguo3118.cn

================================================================================
来源：https://jk.zhonguo2118.cn

[A01] Hello World
来源：https://li.zhonguo5118.cn

Py:   print("Hello, World!")
来源：https://li.zhonguo6118.cn

PHP:  echo "Hello, World!";
来源：https://tq.zhonguo7118.cn

JS:   console.log("Hello, World!");
来源：https://nr.zhonguo4118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://ig.zhonguo7118.cn

Java: System.out.println("Hello, World!");
来源：https://yw.zhonguo1118.cn

Go:   fmt.Println("Hello, World!")
来源：https://xt.zhonguo6118.cn

Ruby: puts "Hello, World!"
来源：https://zt.zhonguo8118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://bv.zhonguo4118.cn

[A02] 变量声明与赋值
来源：https://ev.zhonguo4118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://wk.zhonguo5118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://aq.zhonguo6118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://nd.zhonguo7118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://dc.zhonguo5118.cn

Java: String name = "Alex"; int age = 20;
来源：https://sf.zhonguo7118.cn

Go:   name := "Alex"; age := 20
来源：https://bt.zhonguo3118.cn

Ruby: name = "Alex"; age = 20
来源：https://ik.zhonguo1118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://au.zhonguo5118.cn

[A03] 常量定义
来源：https://vh.zhonguo2118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://na.zhonguo6118.cn

PHP:  const PI = 3.14159;
来源：https://vj.zhonguo2118.cn

JS:   const PI = 3.14159;
来源：https://vm.zhonguo8118.cn

TS:   const PI: number = 3.14159;
来源：https://pe.zhonguo4118.cn

Java: static final double PI = 3.14159;
来源：https://hd.zhonguo5118.cn

Go:   const PI = 3.14159
来源：https://pm.zhonguo1118.cn

Ruby: PI = 3.14159
来源：https://kz.zhonguo4118.cn

C#:   const double PI = 3.14159;
来源：https://dt.zhonguo1118.cn

[A04] 判断变量类型
来源：https://rn.zhonguo1118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://ay.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://ds.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://vg.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://cm.zhonguo6118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://pp.zhonguo7118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://ws.zhonguo2118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://xy.zhonguo6118.cn

C#:   x.GetType().Name; x is int
来源：https://ep.zhonguo7118.cn

[A05] 整数除法与取模
来源：https://nt.zhonguo3118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://pt.zhonguo8118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://fz.zhonguo1118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://qc.zhonguo8118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://pt.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://zl.zhonguo4118.cn

Go:   7 / 2; 7 % 2
来源：https://mb.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://kf.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://ny.zhonguo1118.cn

[A06] 字符串转数字
来源：https://ot.zhonguo7118.cn

Py:   int("42"); float("3.14")
来源：https://bq.zhonguo3118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://qf.zhonguo1118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://ip.zhonguo1118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://kp.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://sv.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://rr.zhonguo8118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://ww.zhonguo6118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://zn.zhonguo3118.cn

[A07] 数字转字符串
来源：https://fa.zhonguo7118.cn

Py:   str(42)
来源：https://rk.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://dw.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://lv.zhonguo8118.cn

TS:   String(42)
来源：https://zm.zhonguo6118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://it.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://pv.zhonguo1118.cn

Ruby: 42.to_s
来源：https://qt.zhonguo1118.cn

C#:   42.ToString()
来源：https://dx.zhonguo6118.cn

[A08] 取整与四舍五入
来源：https://qk.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://cd.zhonguo5118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://nl.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://vn.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://wy.zhonguo3118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ds.zhonguo2118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://yk.zhonguo2118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://qt.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://bo.zhonguo8118.cn

[A09] 绝对值与最大最小值
来源：https://za.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://nb.zhonguo7118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://fu.zhonguo7118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://bn.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://bz.zhonguo1118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://rw.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://qa.zhonguo4118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://ha.zhonguo8118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://oh.zhonguo8118.cn

[A10] 生成随机数
来源：https://vs.zhonguo5118.cn

Py:   import random; random.randint(1, 100)
来源：https://yv.zhonguo3118.cn

PHP:  random_int(1, 100);
来源：https://mt.zhonguo4118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://yb.zhonguo5118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://xt.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://vw.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://hl.zhonguo5118.cn

Ruby: rand(1..100)
来源：https://tn.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://uv.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://zt.zhonguo3118.cn

Py:   "yes" if x > 0 else "no"
来源：https://lq.zhonguo2118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://yd.zhonguo1118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://gk.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://fg.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://ea.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://kc.zhonguo3118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ei.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://uh.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://xy.zhonguo1118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://os.zhonguo6118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://rf.zhonguo3118.cn

JS:   `Hello, ${name}!`
来源：https://yq.zhonguo5118.cn

TS:   `Hello, ${name}!`
来源：https://zj.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://qp.zhonguo8118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ad.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://lw.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://jm.zhonguo6118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://bj.zhonguo8118.cn

Py:   "第一行\n第二行"
来源：https://bb.zhonguo2118.cn

PHP:  "第一行\n第二行"
来源：https://lv.zhonguo4118.cn

JS:   "第一行\n第二行"
来源：https://tc.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://ku.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://hj.zhonguo7118.cn

Go:   "第一行\n第二行"
来源：https://ir.zhonguo5118.cn

Ruby: "第一行\n第二行"
来源：https://hq.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://wl.zhonguo5118.cn

[A14] 注释写法
来源：https://lu.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://dp.zhonguo4118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ct.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://gg.zhonguo8118.cn

TS:   // 单行；/* 多行 */
来源：https://tx.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://px.zhonguo8118.cn

Go:   // 单行；/* 多行 */
来源：https://tp.zhonguo5118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://qy.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://rs.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://gr.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://hi.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://ex.zhonguo5118.cn

JS:   const value = data ?? "默认值";
来源：https://ng.zhonguo3118.cn

TS:   const value = data ?? "默认值";
来源：https://dk.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://bo.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://jz.zhonguo4118.cn

Ruby: value = data || "默认值"
来源：https://aj.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://cu.zhonguo1118.cn

[A16] 真假值判断规则
来源：https://jm.zhonguo7118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://oc.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://db.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://tk.zhonguo6118.cn

TS:   if (!x) {}
来源：https://eu.zhonguo6118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://bh.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://cq.zhonguo2118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://gc.zhonguo8118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://bs.zhonguo2118.cn

[A17] 位运算
来源：https://ao.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://gz.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://lo.zhonguo6118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://no.zhonguo2118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://gl.zhonguo6118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jy.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://gd.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pv.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://eo.zhonguo7118.cn

[A18] 字符与 ASCII 码互转
来源：https://vc.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://mj.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://do.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://cw.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://zz.zhonguo4118.cn

Java: (int) 'A'; (char) 65
来源：https://jr.zhonguo1118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://wl.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://yg.zhonguo5118.cn

C#:   (int)'A'; (char)65
来源：https://ch.zhonguo1118.cn

[A19] 交换两个变量
来源：https://yr.zhonguo5118.cn

Py:   a, b = b, a
来源：https://mi.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://st.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://dg.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://mz.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://zy.zhonguo7118.cn

Go:   a, b = b, a
来源：https://zf.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://ei.zhonguo6118.cn

C#:   (a, b) = (b, a);
来源：https://ij.zhonguo6118.cn

[A20] 读取标准输入
来源：https://tt.zhonguo4118.cn

Py:   name = input("请输入：")
来源：https://oz.zhonguo8118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://hr.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://sn.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://td.zhonguo3118.cn

Java: new Scanner(System.in).nextLine()
来源：https://pm.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://tf.zhonguo3118.cn

Ruby: gets.chomp
来源：https://ng.zhonguo3118.cn

C#:   Console.ReadLine();
来源：https://ms.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://nc.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://bf.zhonguo4118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://su.zhonguo8118.cn

JS:   (3.14159).toFixed(2)
来源：https://tz.zhonguo5118.cn

TS:   (3.14159).toFixed(2)
来源：https://fi.zhonguo2118.cn

Java: String.format("%.2f", 3.14159)
来源：https://fc.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://oe.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ni.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://ms.zhonguo6118.cn

[A22] 获取字符串长度
来源：https://ua.zhonguo5118.cn

Py:   len(s)
来源：https://hl.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://xw.zhonguo6118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://fn.zhonguo6118.cn

TS:   s.length
来源：https://iy.zhonguo3118.cn

Java: s.length()
来源：https://xt.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://zm.zhonguo5118.cn

Ruby: s.length
来源：https://km.zhonguo7118.cn

C#:   s.Length
来源：https://jy.zhonguo7118.cn

[A23] 大小写转换
来源：https://it.zhonguo7118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://np.zhonguo3118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://bk.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ql.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://yt.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://vr.zhonguo1118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://iy.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://qk.zhonguo3118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://da.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://gf.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://jj.zhonguo2118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://bd.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://bn.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://zy.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://we.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://jf.zhonguo6118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://pe.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ct.zhonguo8118.cn

[A25] 字符串比较
来源：https://rb.zhonguo8118.cn

Py:   s1 == s2; s1 != s2
来源：https://ci.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://ip.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://gn.zhonguo8118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://pg.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://vp.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://kc.zhonguo2118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ba.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://sd.zhonguo7118.cn

[A26] 类型转换总览
来源：https://iv.zhonguo4118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://rk.zhonguo3118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://mu.zhonguo4118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://mf.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://qx.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://pq.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://hf.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://vu.zhonguo2118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://us.zhonguo5118.cn

================================================================================
来源：https://go.zhonguo8118.cn

B. 流程控制
来源：https://ql.zhonguo6118.cn

================================================================================
来源：https://sj.zhonguo6118.cn

[B01] 条件判断 if / else
来源：https://yv.zhonguo8118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ff.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://fd.zhonguo6118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://bl.zhonguo4118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://sg.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://sq.zhonguo5118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ua.zhonguo5118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://xt.zhonguo3118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://wa.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://ya.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://qk.zhonguo3118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://kx.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bk.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://la.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cz.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://gs.zhonguo5118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://uj.zhonguo4118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://yp.zhonguo2118.cn

[B03] switch / match / case
来源：https://as.zhonguo4118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://sw.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ss.zhonguo3118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://um.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://nr.zhonguo2118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://cu.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://co.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://pp.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://yh.zhonguo7118.cn

[B04] for 计数循环
来源：https://yy.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://wn.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://vl.zhonguo1118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://qy.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://nt.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://qv.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://pk.zhonguo1118.cn

Ruby: 10.times { |i| puts i }
来源：https://fr.zhonguo3118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ds.zhonguo6118.cn

[B05] 遍历数组 / 列表
来源：https://sd.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://ck.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://vo.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://dn.zhonguo8118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://dk.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://in.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://we.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://sz.zhonguo6118.cn


<!-- 参考信息 -->