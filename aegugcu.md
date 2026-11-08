代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://eh.zhonguo6118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://oc.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://qm.zhonguo8118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://tf.zhonguo1118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://hb.zhonguo3118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://yj.zhonguo5118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://xc.zhonguo2118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://fl.zhonguo3118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://vl.zhonguo1118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://he.zhonguo5118.cn

【文件统计】
来源：https://tn.zhonguo1118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://ce.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://rl.zhonguo1118.cn

目  录
来源：https://ff.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://sh.zhonguo1118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://ei.zhonguo6118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://mt.zhonguo3118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://ab.zhonguo5118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://zj.zhonguo2118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://ne.zhonguo5118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://ku.zhonguo6118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://on.zhonguo7118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://me.zhonguo4118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://gf.zhonguo3118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://mt.zhonguo6118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://pe.zhonguo5118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://wm.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://uh.zhonguo5118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://wp.zhonguo6118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://ip.zhonguo8118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://ap.zhonguo3118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ik.zhonguo4118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://fi.zhonguo5118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ap.zhonguo4118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://tj.zhonguo1118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://kf.zhonguo3118.cn

================================================================================
来源：https://kj.zhonguo7118.cn

A. 基础语法与类型
来源：https://la.zhonguo7118.cn

================================================================================
来源：https://ao.zhonguo5118.cn

[A01] Hello World
来源：https://bf.zhonguo8118.cn

Py:   print("Hello, World!")
来源：https://ob.zhonguo6118.cn

PHP:  echo "Hello, World!";
来源：https://ec.zhonguo5118.cn

JS:   console.log("Hello, World!");
来源：https://eq.zhonguo8118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://qu.zhonguo4118.cn

Java: System.out.println("Hello, World!");
来源：https://po.zhonguo5118.cn

Go:   fmt.Println("Hello, World!")
来源：https://am.zhonguo6118.cn

Ruby: puts "Hello, World!"
来源：https://wp.zhonguo5118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://le.zhonguo3118.cn

[A02] 变量声明与赋值
来源：https://nz.zhonguo8118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://ux.zhonguo1118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://dd.zhonguo5118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://fi.zhonguo2118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://sr.zhonguo1118.cn

Java: String name = "Alex"; int age = 20;
来源：https://pg.zhonguo1118.cn

Go:   name := "Alex"; age := 20
来源：https://tc.zhonguo6118.cn

Ruby: name = "Alex"; age = 20
来源：https://oa.zhonguo2118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://zl.zhonguo1118.cn

[A03] 常量定义
来源：https://mi.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://nu.zhonguo7118.cn

PHP:  const PI = 3.14159;
来源：https://sy.zhonguo6118.cn

JS:   const PI = 3.14159;
来源：https://ct.zhonguo3118.cn

TS:   const PI: number = 3.14159;
来源：https://es.zhonguo5118.cn

Java: static final double PI = 3.14159;
来源：https://ur.zhonguo3118.cn

Go:   const PI = 3.14159
来源：https://gs.zhonguo8118.cn

Ruby: PI = 3.14159
来源：https://hx.zhonguo7118.cn

C#:   const double PI = 3.14159;
来源：https://tk.zhonguo5118.cn

[A04] 判断变量类型
来源：https://al.zhonguo8118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://by.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://uj.zhonguo7118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://ps.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://dy.zhonguo3118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://xo.zhonguo2118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://gg.zhonguo2118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://vl.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://fm.zhonguo3118.cn

[A05] 整数除法与取模
来源：https://dg.zhonguo2118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ir.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://ei.zhonguo3118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://ae.zhonguo5118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ep.zhonguo1118.cn

Java: 7 / 2; 7 % 2
来源：https://iz.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://gv.zhonguo1118.cn

Ruby: 7 / 2; 7 % 2
来源：https://jh.zhonguo3118.cn

C#:   7 / 2; 7 % 2
来源：https://jt.zhonguo1118.cn

[A06] 字符串转数字
来源：https://rr.zhonguo5118.cn

Py:   int("42"); float("3.14")
来源：https://nw.zhonguo2118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://un.zhonguo5118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://ri.zhonguo1118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://mp.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://za.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://nj.zhonguo1118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://ci.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://tz.zhonguo5118.cn

[A07] 数字转字符串
来源：https://hq.zhonguo4118.cn

Py:   str(42)
来源：https://bx.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://pw.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://ud.zhonguo8118.cn

TS:   String(42)
来源：https://mu.zhonguo2118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://fg.zhonguo4118.cn

Go:   strconv.Itoa(42)
来源：https://td.zhonguo8118.cn

Ruby: 42.to_s
来源：https://zu.zhonguo8118.cn

C#:   42.ToString()
来源：https://js.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://tr.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://on.zhonguo8118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://uq.zhonguo4118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ha.zhonguo1118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://os.zhonguo6118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://rl.zhonguo3118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://zy.zhonguo5118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://wq.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://ru.zhonguo7118.cn

[A09] 绝对值与最大最小值
来源：https://mu.zhonguo8118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://oc.zhonguo6118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://kv.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://ed.zhonguo8118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://jz.zhonguo3118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://wx.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://ut.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://nv.zhonguo8118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://gg.zhonguo7118.cn

[A10] 生成随机数
来源：https://lx.zhonguo8118.cn

Py:   import random; random.randint(1, 100)
来源：https://kw.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://of.zhonguo6118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://zr.zhonguo3118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://bd.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://xk.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://sk.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://ai.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://iz.zhonguo2118.cn

[A11] 条件表达式（三元）
来源：https://ua.zhonguo3118.cn

Py:   "yes" if x > 0 else "no"
来源：https://uw.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://rf.zhonguo6118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://en.zhonguo7118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://zo.zhonguo8118.cn

Java: x > 0 ? "yes" : "no"
来源：https://po.zhonguo8118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://yq.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://by.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://pq.zhonguo6118.cn

[A12] 字符串插值 / 格式化
来源：https://qq.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://cq.zhonguo4118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ld.zhonguo7118.cn

JS:   `Hello, ${name}!`
来源：https://ve.zhonguo5118.cn

TS:   `Hello, ${name}!`
来源：https://ix.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://td.zhonguo1118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://hb.zhonguo6118.cn

Ruby: "Hello, #{name}!"
来源：https://nf.zhonguo7118.cn

C#:   $"Hello, {name}!"
来源：https://sw.zhonguo3118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://wz.zhonguo5118.cn

Py:   "第一行\n第二行"
来源：https://lw.zhonguo1118.cn

PHP:  "第一行\n第二行"
来源：https://ed.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://rt.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://be.zhonguo4118.cn

Java: "第一行\n第二行"
来源：https://vj.zhonguo5118.cn

Go:   "第一行\n第二行"
来源：https://zh.zhonguo8118.cn

Ruby: "第一行\n第二行"
来源：https://pt.zhonguo1118.cn

C#:   "第一行\n第二行"
来源：https://hu.zhonguo6118.cn

[A14] 注释写法
来源：https://xh.zhonguo5118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://fj.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://en.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://ey.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://og.zhonguo7118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://fi.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://ls.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://gy.zhonguo1118.cn

C#:   // 单行；/* 多行 */
来源：https://bl.zhonguo4118.cn

[A15] 空值判断与默认值
来源：https://af.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://qa.zhonguo5118.cn

PHP:  $value = $data ?? "默认值";
来源：https://lf.zhonguo2118.cn

JS:   const value = data ?? "默认值";
来源：https://rg.zhonguo8118.cn

TS:   const value = data ?? "默认值";
来源：https://ar.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://jx.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://eo.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://th.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://wq.zhonguo4118.cn

[A16] 真假值判断规则
来源：https://oi.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://oe.zhonguo8118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://uv.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://ir.zhonguo4118.cn

TS:   if (!x) {}
来源：https://bb.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://jb.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://db.zhonguo7118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://if.zhonguo8118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://zd.zhonguo5118.cn

[A17] 位运算
来源：https://mj.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://st.zhonguo5118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://eo.zhonguo8118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rw.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://gq.zhonguo1118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wu.zhonguo4118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qs.zhonguo4118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ry.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://xu.zhonguo4118.cn

[A18] 字符与 ASCII 码互转
来源：https://kb.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://jt.zhonguo3118.cn

PHP:  ord("A"); chr(65)
来源：https://gj.zhonguo7118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://zy.zhonguo1118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://rl.zhonguo5118.cn

Java: (int) 'A'; (char) 65
来源：https://fp.zhonguo4118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://cc.zhonguo8118.cn

Ruby: "A".ord; 65.chr
来源：https://fq.zhonguo6118.cn

C#:   (int)'A'; (char)65
来源：https://ku.zhonguo1118.cn

[A19] 交换两个变量
来源：https://my.zhonguo5118.cn

Py:   a, b = b, a
来源：https://pt.zhonguo8118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://sg.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://hn.zhonguo2118.cn

TS:   [a, b] = [b, a];
来源：https://ep.zhonguo2118.cn

Java: int t = a; a = b; b = t;
来源：https://wh.zhonguo7118.cn

Go:   a, b = b, a
来源：https://mb.zhonguo7118.cn

Ruby: a, b = b, a
来源：https://eq.zhonguo3118.cn

C#:   (a, b) = (b, a);
来源：https://qu.zhonguo4118.cn

[A20] 读取标准输入
来源：https://jo.zhonguo6118.cn

Py:   name = input("请输入：")
来源：https://zb.zhonguo4118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ov.zhonguo3118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://oo.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://pz.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://rf.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ej.zhonguo2118.cn

Ruby: gets.chomp
来源：https://dc.zhonguo5118.cn

C#:   Console.ReadLine();
来源：https://qf.zhonguo6118.cn

[A21] 保留指定小数位输出
来源：https://dt.zhonguo2118.cn

Py:   f"{3.14159:.2f}"
来源：https://pb.zhonguo1118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://su.zhonguo8118.cn

JS:   (3.14159).toFixed(2)
来源：https://qt.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://uv.zhonguo2118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ib.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://qk.zhonguo6118.cn

Ruby: format("%.2f", 3.14159)
来源：https://bv.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://bb.zhonguo1118.cn

[A22] 获取字符串长度
来源：https://xz.zhonguo1118.cn

Py:   len(s)
来源：https://ba.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://fg.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://fq.zhonguo4118.cn

TS:   s.length
来源：https://tt.zhonguo8118.cn

Java: s.length()
来源：https://xt.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://iy.zhonguo1118.cn

Ruby: s.length
来源：https://yj.zhonguo4118.cn

C#:   s.Length
来源：https://gf.zhonguo3118.cn

[A23] 大小写转换
来源：https://gy.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://jm.zhonguo1118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://am.zhonguo7118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ae.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ut.zhonguo5118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ia.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://xc.zhonguo8118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://kg.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ib.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://ey.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://dv.zhonguo4118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ij.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://gk.zhonguo1118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://al.zhonguo4118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://xj.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://op.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://st.zhonguo7118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://hf.zhonguo2118.cn

[A25] 字符串比较
来源：https://rb.zhonguo3118.cn

Py:   s1 == s2; s1 != s2
来源：https://yb.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://fj.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://em.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://sz.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://sb.zhonguo2118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://du.zhonguo1118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://lj.zhonguo6118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://qi.zhonguo2118.cn

[A26] 类型转换总览
来源：https://hy.zhonguo2118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://fu.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ax.zhonguo6118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://kv.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://xf.zhonguo4118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://za.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://aq.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://bh.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ho.zhonguo6118.cn

================================================================================
来源：https://da.zhonguo4118.cn

B. 流程控制
来源：https://tc.zhonguo4118.cn

================================================================================
来源：https://gi.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://im.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://wr.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://fs.zhonguo4118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://tf.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://an.zhonguo5118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://mq.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://rs.zhonguo4118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://tw.zhonguo7118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://br.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://jm.zhonguo1118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://wl.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://qq.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://yw.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fn.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bh.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://nl.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://xj.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pf.zhonguo1118.cn

[B03] switch / match / case
来源：https://ni.zhonguo4118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://wf.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://lw.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://cv.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ci.zhonguo3118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://gu.zhonguo7118.cn


<!-- 参考信息 -->