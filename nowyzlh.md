代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://ys.zhonguo3118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://qw.zhonguo7118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://al.zhonguo4118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://yu.zhonguo6118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://go.zhonguo6118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://fc.zhonguo8118.cn

【文件统计】
来源：https://jt.zhonguo3118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://zs.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://uq.zhonguo4118.cn

目  录
来源：https://oe.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://wx.zhonguo5118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://sm.zhonguo1118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://za.zhonguo6118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://ij.zhonguo5118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://hh.zhonguo1118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://uz.zhonguo4118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://pb.zhonguo6118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://ha.zhonguo5118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://mj.zhonguo6118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://uz.zhonguo6118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://sq.zhonguo4118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://ti.zhonguo2118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://ou.zhonguo7118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://nn.zhonguo6118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://zz.zhonguo5118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://sr.zhonguo3118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://zc.zhonguo4118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://lj.zhonguo1118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://gr.zhonguo4118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ir.zhonguo5118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://vl.zhonguo7118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://ww.zhonguo7118.cn

================================================================================
来源：https://zp.zhonguo7118.cn

A. 基础语法与类型
来源：https://yt.zhonguo3118.cn

================================================================================
来源：https://jx.zhonguo8118.cn

[A01] Hello World
来源：https://uc.zhonguo1118.cn

Py:   print("Hello, World!")
来源：https://wx.zhonguo3118.cn

PHP:  echo "Hello, World!";
来源：https://ab.zhonguo8118.cn

JS:   console.log("Hello, World!");
来源：https://pp.zhonguo5118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://qv.zhonguo7118.cn

Java: System.out.println("Hello, World!");
来源：https://at.zhonguo7118.cn

Go:   fmt.Println("Hello, World!")
来源：https://iu.zhonguo6118.cn

Ruby: puts "Hello, World!"
来源：https://mm.zhonguo2118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://cw.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://pu.zhonguo6118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://qv.zhonguo1118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://rl.zhonguo1118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://tb.zhonguo1118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://on.zhonguo3118.cn

Java: String name = "Alex"; int age = 20;
来源：https://ce.zhonguo4118.cn

Go:   name := "Alex"; age := 20
来源：https://ne.zhonguo6118.cn

Ruby: name = "Alex"; age = 20
来源：https://xa.zhonguo2118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://jh.zhonguo5118.cn

[A03] 常量定义
来源：https://lh.zhonguo1118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://gg.zhonguo3118.cn

PHP:  const PI = 3.14159;
来源：https://fw.zhonguo7118.cn

JS:   const PI = 3.14159;
来源：https://mh.zhonguo8118.cn

TS:   const PI: number = 3.14159;
来源：https://at.zhonguo4118.cn

Java: static final double PI = 3.14159;
来源：https://qd.zhonguo1118.cn

Go:   const PI = 3.14159
来源：https://cg.zhonguo6118.cn

Ruby: PI = 3.14159
来源：https://gv.zhonguo8118.cn

C#:   const double PI = 3.14159;
来源：https://hn.zhonguo6118.cn

[A04] 判断变量类型
来源：https://qs.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://yz.zhonguo3118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://gc.zhonguo2118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://re.zhonguo5118.cn

TS:   typeof x; x instanceof Date
来源：https://hk.zhonguo7118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://vw.zhonguo2118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://gh.zhonguo2118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://uu.zhonguo7118.cn

C#:   x.GetType().Name; x is int
来源：https://ec.zhonguo6118.cn

[A05] 整数除法与取模
来源：https://zq.zhonguo7118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://bl.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://az.zhonguo1118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://zu.zhonguo2118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://rq.zhonguo6118.cn

Java: 7 / 2; 7 % 2
来源：https://sc.zhonguo2118.cn

Go:   7 / 2; 7 % 2
来源：https://vi.zhonguo7118.cn

Ruby: 7 / 2; 7 % 2
来源：https://jw.zhonguo4118.cn

C#:   7 / 2; 7 % 2
来源：https://gh.zhonguo8118.cn

[A06] 字符串转数字
来源：https://eu.zhonguo6118.cn

Py:   int("42"); float("3.14")
来源：https://gt.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://xz.zhonguo2118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://wv.zhonguo6118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://mq.zhonguo8118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://fr.zhonguo4118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://sr.zhonguo1118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://rm.zhonguo4118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://og.zhonguo1118.cn

[A07] 数字转字符串
来源：https://zm.zhonguo3118.cn

Py:   str(42)
来源：https://jr.zhonguo6118.cn

PHP:  (string) 42; strval(42)
来源：https://lv.zhonguo4118.cn

JS:   String(42); (42).toString()
来源：https://re.zhonguo3118.cn

TS:   String(42)
来源：https://co.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://pq.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://yo.zhonguo7118.cn

Ruby: 42.to_s
来源：https://dv.zhonguo8118.cn

C#:   42.ToString()
来源：https://jg.zhonguo8118.cn

[A08] 取整与四舍五入
来源：https://qv.zhonguo1118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://vh.zhonguo5118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://fq.zhonguo6118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ow.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://us.zhonguo1118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://hk.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://ny.zhonguo6118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://uz.zhonguo8118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://mm.zhonguo1118.cn

[A09] 绝对值与最大最小值
来源：https://px.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://pp.zhonguo3118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://sk.zhonguo5118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://sx.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ve.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://en.zhonguo8118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://wy.zhonguo4118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://uo.zhonguo2118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://yv.zhonguo5118.cn

[A10] 生成随机数
来源：https://ql.zhonguo6118.cn

Py:   import random; random.randint(1, 100)
来源：https://as.zhonguo2118.cn

PHP:  random_int(1, 100);
来源：https://dy.zhonguo7118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://nf.zhonguo5118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://xs.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://it.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://oc.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://vh.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://mt.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://nj.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://rk.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://cw.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://mj.zhonguo4118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://fi.zhonguo1118.cn

Java: x > 0 ? "yes" : "no"
来源：https://ae.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://jf.zhonguo7118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ux.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://pd.zhonguo7118.cn

[A12] 字符串插值 / 格式化
来源：https://fx.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://ql.zhonguo7118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ib.zhonguo8118.cn

JS:   `Hello, ${name}!`
来源：https://hg.zhonguo6118.cn

TS:   `Hello, ${name}!`
来源：https://qj.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://rc.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://zs.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://mc.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://zv.zhonguo4118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://rj.zhonguo2118.cn

Py:   "第一行\n第二行"
来源：https://sl.zhonguo5118.cn

PHP:  "第一行\n第二行"
来源：https://jb.zhonguo6118.cn

JS:   "第一行\n第二行"
来源：https://ab.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://tg.zhonguo1118.cn

Java: "第一行\n第二行"
来源：https://il.zhonguo2118.cn

Go:   "第一行\n第二行"
来源：https://um.zhonguo4118.cn

Ruby: "第一行\n第二行"
来源：https://ua.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://nc.zhonguo4118.cn

[A14] 注释写法
来源：https://ot.zhonguo6118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ps.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ic.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://jw.zhonguo7118.cn

TS:   // 单行；/* 多行 */
来源：https://ry.zhonguo5118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://fm.zhonguo2118.cn

Go:   // 单行；/* 多行 */
来源：https://qw.zhonguo1118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://no.zhonguo7118.cn

C#:   // 单行；/* 多行 */
来源：https://fy.zhonguo4118.cn

[A15] 空值判断与默认值
来源：https://qe.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://yo.zhonguo8118.cn

PHP:  $value = $data ?? "默认值";
来源：https://ac.zhonguo5118.cn

JS:   const value = data ?? "默认值";
来源：https://pc.zhonguo4118.cn

TS:   const value = data ?? "默认值";
来源：https://mk.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://oo.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://xb.zhonguo7118.cn

Ruby: value = data || "默认值"
来源：https://tu.zhonguo8118.cn

C#:   var value = data ?? "默认值";
来源：https://mo.zhonguo7118.cn

[A16] 真假值判断规则
来源：https://lm.zhonguo8118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://pp.zhonguo2118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fc.zhonguo5118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://kn.zhonguo5118.cn

TS:   if (!x) {}
来源：https://pp.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://fb.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://cm.zhonguo2118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://nf.zhonguo8118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://fy.zhonguo6118.cn

[A17] 位运算
来源：https://ww.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://et.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://de.zhonguo4118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pf.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ml.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wy.zhonguo1118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://je.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ok.zhonguo6118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rm.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://kh.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://nr.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://dh.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://bp.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mv.zhonguo6118.cn

Java: (int) 'A'; (char) 65
来源：https://og.zhonguo7118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://nu.zhonguo6118.cn

Ruby: "A".ord; 65.chr
来源：https://xw.zhonguo8118.cn

C#:   (int)'A'; (char)65
来源：https://tm.zhonguo1118.cn

[A19] 交换两个变量
来源：https://hl.zhonguo2118.cn

Py:   a, b = b, a
来源：https://mo.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://cs.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://mn.zhonguo2118.cn

TS:   [a, b] = [b, a];
来源：https://iu.zhonguo6118.cn

Java: int t = a; a = b; b = t;
来源：https://ch.zhonguo2118.cn

Go:   a, b = b, a
来源：https://qc.zhonguo7118.cn

Ruby: a, b = b, a
来源：https://ar.zhonguo4118.cn

C#:   (a, b) = (b, a);
来源：https://dx.zhonguo2118.cn

[A20] 读取标准输入
来源：https://zb.zhonguo1118.cn

Py:   name = input("请输入：")
来源：https://td.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://uy.zhonguo6118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://vv.zhonguo4118.cn

TS:   // Node.js：readline 模块
来源：https://dk.zhonguo3118.cn

Java: new Scanner(System.in).nextLine()
来源：https://vy.zhonguo3118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://wk.zhonguo2118.cn

Ruby: gets.chomp
来源：https://vn.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://uw.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://xs.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://xn.zhonguo6118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://uk.zhonguo8118.cn

JS:   (3.14159).toFixed(2)
来源：https://fh.zhonguo7118.cn

TS:   (3.14159).toFixed(2)
来源：https://ge.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://om.zhonguo8118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://dj.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ds.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://ml.zhonguo1118.cn

[A22] 获取字符串长度
来源：https://ze.zhonguo8118.cn

Py:   len(s)
来源：https://ef.zhonguo3118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://xp.zhonguo6118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://ca.zhonguo3118.cn

TS:   s.length
来源：https://wh.zhonguo5118.cn

Java: s.length()
来源：https://pk.zhonguo2118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://kd.zhonguo2118.cn

Ruby: s.length
来源：https://fq.zhonguo1118.cn

C#:   s.Length
来源：https://dv.zhonguo7118.cn

[A23] 大小写转换
来源：https://pd.zhonguo7118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://os.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://xd.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://jc.zhonguo1118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://jm.zhonguo2118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://eb.zhonguo8118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ko.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://xt.zhonguo3118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://qs.zhonguo1118.cn

[A24] 去除首尾空白
来源：https://nb.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ry.zhonguo8118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://oa.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://km.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://vx.zhonguo7118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://il.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://wz.zhonguo4118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ed.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://fk.zhonguo7118.cn

[A25] 字符串比较
来源：https://sn.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://ig.zhonguo4118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://ov.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ho.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://hh.zhonguo5118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ga.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://li.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ro.zhonguo5118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://gj.zhonguo6118.cn

[A26] 类型转换总览
来源：https://ug.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ug.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://gx.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://tb.zhonguo3118.cn

TS:   Number() String() Boolean() x as number
来源：https://ah.zhonguo7118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://uk.zhonguo2118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://mw.zhonguo2118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://dd.zhonguo4118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://wq.zhonguo8118.cn

================================================================================
来源：https://uo.zhonguo2118.cn

B. 流程控制
来源：https://ae.zhonguo4118.cn

================================================================================
来源：https://um.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://mp.zhonguo1118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://xf.zhonguo2118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://pe.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://aa.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://qh.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://hk.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://le.zhonguo8118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://hc.zhonguo2118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://kq.zhonguo6118.cn

[B02] 多分支 else if / elif
来源：https://nf.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://mf.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ei.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://go.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pf.zhonguo8118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zz.zhonguo3118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://pb.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://cl.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ma.zhonguo8118.cn

[B03] switch / match / case
来源：https://af.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://uv.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://dy.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://vq.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://tw.zhonguo2118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://nc.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://wz.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://up.zhonguo3118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://hq.zhonguo7118.cn

[B04] for 计数循环
来源：https://oa.zhonguo6118.cn


<!-- 参考信息 -->