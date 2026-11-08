代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://af.zhonguo2118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://rw.zhonguo6118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://lc.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://ns.zhonguo1118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://gg.zhonguo8118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://cz.zhonguo7118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://cd.zhonguo7118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://of.zhonguo1118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://jo.zhonguo2118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ij.zhonguo1118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://nh.zhonguo8118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://gf.zhonguo1118.cn

================================================================================
来源：https://ck.zhonguo4118.cn

A. 基础语法与类型
来源：https://wb.zhonguo1118.cn

================================================================================
来源：https://yx.zhonguo2118.cn

[A01] Hello World
来源：https://il.zhonguo7118.cn

Py:   print("Hello, World!")
来源：https://vf.zhonguo6118.cn

PHP:  echo "Hello, World!";
来源：https://qj.zhonguo4118.cn

JS:   console.log("Hello, World!");
来源：https://km.zhonguo8118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://jw.zhonguo4118.cn

Java: System.out.println("Hello, World!");
来源：https://rh.zhonguo6118.cn

Go:   fmt.Println("Hello, World!")
来源：https://dx.zhonguo1118.cn

Ruby: puts "Hello, World!"
来源：https://lz.zhonguo7118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://lk.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://oz.zhonguo8118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://hx.zhonguo1118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://bc.zhonguo4118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://ii.zhonguo3118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://bl.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://yq.zhonguo4118.cn

Go:   name := "Alex"; age := 20
来源：https://ta.zhonguo1118.cn

Ruby: name = "Alex"; age = 20
来源：https://uy.zhonguo4118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://qc.zhonguo6118.cn

[A03] 常量定义
来源：https://il.zhonguo3118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ba.zhonguo2118.cn

PHP:  const PI = 3.14159;
来源：https://oh.zhonguo7118.cn

JS:   const PI = 3.14159;
来源：https://kv.zhonguo1118.cn

TS:   const PI: number = 3.14159;
来源：https://hi.zhonguo4118.cn

Java: static final double PI = 3.14159;
来源：https://nv.zhonguo2118.cn

Go:   const PI = 3.14159
来源：https://eo.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://ss.zhonguo3118.cn

C#:   const double PI = 3.14159;
来源：https://bm.zhonguo6118.cn

[A04] 判断变量类型
来源：https://gz.zhonguo8118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://xy.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://ez.zhonguo7118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://yg.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://lq.zhonguo4118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://zw.zhonguo3118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://vz.zhonguo4118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://cr.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://xk.zhonguo7118.cn

[A05] 整数除法与取模
来源：https://en.zhonguo2118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://gj.zhonguo2118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://qs.zhonguo7118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://pt.zhonguo1118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://uy.zhonguo8118.cn

Java: 7 / 2; 7 % 2
来源：https://km.zhonguo8118.cn

Go:   7 / 2; 7 % 2
来源：https://my.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://yx.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://ga.zhonguo6118.cn

[A06] 字符串转数字
来源：https://ew.zhonguo6118.cn

Py:   int("42"); float("3.14")
来源：https://tf.zhonguo5118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://nu.zhonguo6118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://cj.zhonguo2118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://mm.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://as.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://an.zhonguo2118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://li.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://yb.zhonguo4118.cn

[A07] 数字转字符串
来源：https://mp.zhonguo6118.cn

Py:   str(42)
来源：https://wr.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://la.zhonguo7118.cn

JS:   String(42); (42).toString()
来源：https://qc.zhonguo8118.cn

TS:   String(42)
来源：https://eh.zhonguo2118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://sj.zhonguo7118.cn

Go:   strconv.Itoa(42)
来源：https://dt.zhonguo1118.cn

Ruby: 42.to_s
来源：https://wp.zhonguo5118.cn

C#:   42.ToString()
来源：https://mh.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://ek.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ju.zhonguo6118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://cn.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://rw.zhonguo6118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://ib.zhonguo6118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://nr.zhonguo8118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://bj.zhonguo7118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://px.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://te.zhonguo2118.cn

[A09] 绝对值与最大最小值
来源：https://zm.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ue.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://al.zhonguo7118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://mg.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ko.zhonguo1118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://oo.zhonguo4118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://yj.zhonguo3118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://yu.zhonguo6118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://fs.zhonguo3118.cn

[A10] 生成随机数
来源：https://zo.zhonguo8118.cn

Py:   import random; random.randint(1, 100)
来源：https://vp.zhonguo2118.cn

PHP:  random_int(1, 100);
来源：https://ec.zhonguo2118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://xf.zhonguo7118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://gx.zhonguo6118.cn

Java: new Random().nextInt(100) + 1
来源：https://sm.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://mo.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://mq.zhonguo4118.cn

C#:   new Random().Next(1, 101)
来源：https://ad.zhonguo1118.cn

[A11] 条件表达式（三元）
来源：https://hm.zhonguo7118.cn

Py:   "yes" if x > 0 else "no"
来源：https://il.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://hf.zhonguo2118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ma.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://wz.zhonguo7118.cn

Java: x > 0 ? "yes" : "no"
来源：https://cz.zhonguo8118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://jz.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://mz.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://zu.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://kx.zhonguo5118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://cw.zhonguo4118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://av.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://dq.zhonguo7118.cn

TS:   `Hello, ${name}!`
来源：https://qr.zhonguo4118.cn

Java: "Hello, %s!".formatted(name)
来源：https://iu.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://it.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://gq.zhonguo8118.cn

C#:   $"Hello, {name}!"
来源：https://hq.zhonguo2118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://je.zhonguo5118.cn

Py:   "第一行\n第二行"
来源：https://hr.zhonguo3118.cn

PHP:  "第一行\n第二行"
来源：https://ik.zhonguo2118.cn

JS:   "第一行\n第二行"
来源：https://zf.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://cb.zhonguo5118.cn

Java: "第一行\n第二行"
来源：https://ti.zhonguo2118.cn

Go:   "第一行\n第二行"
来源：https://vu.zhonguo7118.cn

Ruby: "第一行\n第二行"
来源：https://dh.zhonguo4118.cn

C#:   "第一行\n第二行"
来源：https://vn.zhonguo1118.cn

[A14] 注释写法
来源：https://nc.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ry.zhonguo4118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ew.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://vo.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://zy.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://wk.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://vk.zhonguo2118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ma.zhonguo7118.cn

C#:   // 单行；/* 多行 */
来源：https://pu.zhonguo5118.cn

[A15] 空值判断与默认值
来源：https://yh.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://ds.zhonguo3118.cn

PHP:  $value = $data ?? "默认值";
来源：https://nv.zhonguo1118.cn

JS:   const value = data ?? "默认值";
来源：https://kw.zhonguo7118.cn

TS:   const value = data ?? "默认值";
来源：https://nc.zhonguo4118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://yq.zhonguo7118.cn

Go:   if data == "" { data = "默认值" }
来源：https://nq.zhonguo3118.cn

Ruby: value = data || "默认值"
来源：https://el.zhonguo8118.cn

C#:   var value = data ?? "默认值";
来源：https://uf.zhonguo7118.cn

[A16] 真假值判断规则
来源：https://kt.zhonguo2118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://bx.zhonguo8118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://ag.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://fy.zhonguo6118.cn

TS:   if (!x) {}
来源：https://lb.zhonguo1118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ak.zhonguo4118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://ke.zhonguo5118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://cy.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://gz.zhonguo8118.cn

[A17] 位运算
来源：https://gg.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://uz.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://lx.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vx.zhonguo8118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://dv.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jn.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ck.zhonguo8118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jo.zhonguo5118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://of.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://hd.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://lx.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://ix.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://gf.zhonguo6118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://lt.zhonguo2118.cn

Java: (int) 'A'; (char) 65
来源：https://os.zhonguo1118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://md.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://tc.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://de.zhonguo7118.cn

[A19] 交换两个变量
来源：https://ze.zhonguo2118.cn

Py:   a, b = b, a
来源：https://ug.zhonguo4118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://et.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://ra.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://ko.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://xe.zhonguo5118.cn

Go:   a, b = b, a
来源：https://vx.zhonguo8118.cn

Ruby: a, b = b, a
来源：https://hn.zhonguo1118.cn

C#:   (a, b) = (b, a);
来源：https://tc.zhonguo4118.cn

[A20] 读取标准输入
来源：https://gv.zhonguo7118.cn

Py:   name = input("请输入：")
来源：https://ii.zhonguo6118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://nl.zhonguo7118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://uk.zhonguo2118.cn

TS:   // Node.js：readline 模块
来源：https://sl.zhonguo3118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ec.zhonguo2118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://rg.zhonguo7118.cn

Ruby: gets.chomp
来源：https://rd.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://kt.zhonguo1118.cn

[A21] 保留指定小数位输出
来源：https://ds.zhonguo2118.cn

Py:   f"{3.14159:.2f}"
来源：https://kp.zhonguo6118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://gh.zhonguo2118.cn

JS:   (3.14159).toFixed(2)
来源：https://tk.zhonguo1118.cn

TS:   (3.14159).toFixed(2)
来源：https://it.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://nl.zhonguo2118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ll.zhonguo6118.cn

Ruby: format("%.2f", 3.14159)
来源：https://rq.zhonguo2118.cn

C#:   3.14159.ToString("F2")
来源：https://lm.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://ft.zhonguo4118.cn

Py:   len(s)
来源：https://ak.zhonguo3118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://yg.zhonguo2118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://kd.zhonguo4118.cn

TS:   s.length
来源：https://su.zhonguo1118.cn

Java: s.length()
来源：https://wj.zhonguo8118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://ti.zhonguo7118.cn

Ruby: s.length
来源：https://zh.zhonguo6118.cn

C#:   s.Length
来源：https://qb.zhonguo8118.cn

[A23] 大小写转换
来源：https://ub.zhonguo3118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://vi.zhonguo1118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://zk.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://fp.zhonguo7118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://hm.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://sj.zhonguo2118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://np.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://qo.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ad.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://xd.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ym.zhonguo4118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://xl.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://wg.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ul.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://gz.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://cm.zhonguo3118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://hx.zhonguo6118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://kr.zhonguo5118.cn

[A25] 字符串比较
来源：https://si.zhonguo3118.cn

Py:   s1 == s2; s1 != s2
来源：https://bh.zhonguo7118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://qh.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://nq.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://uy.zhonguo8118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://uc.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ir.zhonguo5118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ad.zhonguo8118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ci.zhonguo7118.cn

[A26] 类型转换总览
来源：https://mw.zhonguo4118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://lo.zhonguo6118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://mg.zhonguo6118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://sr.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://yf.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://mz.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://mt.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://tz.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://lq.zhonguo2118.cn

================================================================================
来源：https://ua.zhonguo4118.cn

B. 流程控制
来源：https://io.zhonguo5118.cn

================================================================================
来源：https://xd.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://wm.zhonguo1118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://yv.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://br.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://fx.zhonguo5118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://og.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://go.zhonguo5118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://qw.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://jl.zhonguo7118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://wy.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://xi.zhonguo4118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://dr.zhonguo8118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://af.zhonguo8118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://rj.zhonguo2118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zu.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zc.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://kk.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://wa.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gd.zhonguo8118.cn

[B03] switch / match / case
来源：https://wx.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://fn.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://lh.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://el.zhonguo8118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://hu.zhonguo2118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://uk.zhonguo1118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://lj.zhonguo4118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://dk.zhonguo1118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://zh.zhonguo4118.cn

[B04] for 计数循环
来源：https://an.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://wf.zhonguo6118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://zp.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://du.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xj.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://mm.zhonguo4118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://qh.zhonguo7118.cn

Ruby: 10.times { |i| puts i }
来源：https://ai.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ux.zhonguo7118.cn

[B05] 遍历数组 / 列表
来源：https://cp.zhonguo8118.cn

Py:   for item in arr: print(item)
来源：https://te.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://vl.zhonguo2118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://pl.zhonguo3118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://oo.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://gi.zhonguo2118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://gu.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://eo.zhonguo1118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://xn.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://zf.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ub.zhonguo6118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://xa.zhonguo2118.cn


<!-- 参考信息 -->