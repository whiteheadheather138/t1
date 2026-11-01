代发 wailian999

[A02] 变量声明与赋值
来源：http://3g.bbcook.cn/Article/details/gwnaaxwpq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gdvcwlngx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gnwonbgul.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fktsv.cn/Article/details/gkykcgwyw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/ggvjzpxfd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/gaebkdkpp.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gvzxoumfp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.bbcook.cn/Article/details/gfrpjeevb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/ghwrcrzoi.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/gncqkpjqq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.sjlbkw.cn/Article/details/ghsqzbqzk.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gxknrtbdi.sHtML

JS:   const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gfcrmcfqq.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gwrksyoah.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/girukadal.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gizuedryr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gvujdsesj.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gfoijgimq.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gimquqabb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/guvkqhzmg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.epnwcf.com/Article/details/gfrmoptpe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsawovpw.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/ggzkgdynh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.bbcook.cn/Article/details/gsqoteozv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.yfazqb.com/Article/details/gzjjgritk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.sjlbkw.cn/Article/details/gxrxkuqmo.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.vehdjk.com/Article/details/ggrparqow.sHtML

[A05] 整数除法与取模
来源：http://m.share.bbcook.cn/Article/details/ghsxwucuo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtloicvnz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gthwyuiii.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/gspghtzfz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gltexcjul.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gpdnwxtbm.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gfnewhukt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/glsngtpvl.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gjznwablb.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/govabhqcw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gszscvjcw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/getawaery.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.vehdjk.com/Article/details/gdqclylhn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/giditnjws.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.epnwcf.com/Article/details/grxswmdfg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/gbivcnynn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/ghionzkpb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/gptvhduxb.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gxnoxlhgn.sHtML

Py:   str(42)
来源：http://blog.bbcook.cn/Article/details/gbvdninht.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.epnwcf.com/Article/details/gihwnlvgp.sHtML

JS:   String(42); (42).toString()
来源：http://blog.epnwcf.com/Article/details/grltushvo.sHtML

TS:   String(42)
来源：http://www.blog.sjlbkw.cn/Article/details/glfuqzqnu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.vehdjk.com/Article/details/gcbgkztqw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.yfazqb.com/Article/details/ggwchwpnq.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gtlzchbxc.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/ghxayddma.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gxyjagryl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gudqgnggd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.yfazqb.com/Article/details/gfceiqbkl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gpqguxqup.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.yfazqb.com/Article/details/gkgokzmze.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gppvkwxwr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gadxtdufm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/gkigyimjg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gqmvuxtsm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.yfazqb.com/Article/details/gvlhfnife.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gbjvvztyv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fktsv.cn/Article/details/gvtrwxqph.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gpezzipwo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.bbcook.cn/Article/details/glcxtjywt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gllmifeuy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.sjlbkw.cn/Article/details/gjgipplqj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.vehdjk.com/Article/details/gbhiaaoib.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gntfqvvyl.sHtML

[A10] 生成随机数
来源：http://3g.fktsv.cn/Article/details/gdysggrfo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.vehdjk.com/Article/details/giufjpmie.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.vehdjk.com/Article/details/gzemxwpjw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.yfazqb.com/Article/details/gayhcwjeb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gufzoriam.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gopawuirw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.sjlbkw.cn/Article/details/gvcrgfdlm.sHtML

Ruby: rand(1..100)
来源：http://www.blog.bbcook.cn/Article/details/gtgmwxixk.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gkvmbtsbw.sHtML

[A11] 条件表达式（三元）
来源：http://wap.vehdjk.com/Article/details/gcndwereb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.bbcook.cn/Article/details/gqnoplkuw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gqtyzcihd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gaygfskdp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gvmjchmen.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gamhgttxt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.vehdjk.com/Article/details/gvfkfqewl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gugpyaqcz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gsrldnprn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fktsv.cn/Article/details/glfnkcqyc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.epnwcf.com/Article/details/gncinpcyo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.vehdjk.com/Article/details/gjzqhkdkr.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.vehdjk.com/Article/details/gqflzqfgq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.epnwcf.com/Article/details/gbyyniztu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.vehdjk.com/Article/details/grvnuidvs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fktsv.cn/Article/details/gucgrwhno.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gttqxmiwg.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.sjlbkw.cn/Article/details/gucvuzmqr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gznigzlvb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/ghhhwuhpg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/glavbklkm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gweybyrcq.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gezbhyore.sHtML

Java: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gwdjxkwsj.sHtML

Go:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gjqwqfcpe.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gclmdrcpw.sHtML

C#:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/ggbqeymtr.sHtML

[A14] 注释写法
来源：http://wap.tarul.cn/Article/details/grrpedihf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.vehdjk.com/Article/details/gaqpsisxu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gcwlasper.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gtvnesjmp.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gzsfayfkz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.yfazqb.com/Article/details/gjlurigsc.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gblyxiaoz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.bbcook.cn/Article/details/grtlwawwb.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gqtahqvtc.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/guybcmvjg.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gvxkvpfuk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/guxrddrpy.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gfvsxrnyw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gbbvddtvu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.vehdjk.com/Article/details/gtxlpikuy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gqqscyxek.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/gonfkfcht.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gdljqklqj.sHtML

[A16] 真假值判断规则
来源：http://wap.tarul.cn/Article/details/gdsrffvoo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.yfazqb.com/Article/details/grrbufeou.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/ggzqlihow.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gmljajwdx.sHtML

TS:   if (!x) {}
来源：http://3g.epnwcf.com/Article/details/gobgpepif.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/guolctbba.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/gmuznniji.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.epnwcf.com/Article/details/gppbnxtap.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.vehdjk.com/Article/details/gzqrzcsbm.sHtML

[A17] 位运算
来源：http://m.share.bbcook.cn/Article/details/ghrygevxp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gbttlyquf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gnuclibmw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gujbjaqil.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gtbqmlvlr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/glompmsei.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gzyjuqapn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gcicotzgs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gpzatoboi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/grydhjagx.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.tarul.cn/Article/details/gsbizjpjl.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gezjimsgk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gpptfvxhe.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/ggyjhumax.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.bbcook.cn/Article/details/gsdwfavie.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/glvwhxieq.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/guokxtphl.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.vehdjk.com/Article/details/gwgtbxdlq.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/gfpjfawho.sHtML

Py:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gcbwtrfjz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fktsv.cn/Article/details/glhnjznfi.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/ggtfirtbz.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gygheigws.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gqodjplvg.sHtML

Go:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/glcqphuuf.sHtML

Ruby: a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gwyupesmh.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.tarul.cn/Article/details/gxcxtxzuw.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/gfbswbjgk.sHtML

Py:   name = input("请输入：")
来源：http://3g.sjlbkw.cn/Article/details/gkyehzdhi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.tarul.cn/Article/details/gbhcrzvks.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.vehdjk.com/Article/details/gzyyyvupu.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.epnwcf.com/Article/details/gvwxiiytl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fktsv.cn/Article/details/gfvriadkh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.bbcook.cn/Article/details/gndnamabr.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/gtdhchriq.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fktsv.cn/Article/details/goiwmudyw.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.bbcook.cn/Article/details/girhzmyxd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/geawndzud.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gepwjsupg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/giltcacob.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gsyaxmtrx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gwyqitomf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gyyufyecj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gdnimyusl.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gskhgbhje.sHtML

[A22] 获取字符串长度
来源：http://baike.epnwcf.com/Article/details/gbqoyltqs.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gwmpldxqz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.epnwcf.com/Article/details/guhnespge.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/gskfhvqij.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gfdsohgzi.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gmkxxdgtn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/graovygft.sHtML

Ruby: s.length
来源：http://www.blog.yfazqb.com/Article/details/gdaegjftc.sHtML

C#:   s.Length
来源：http://wap.sjlbkw.cn/Article/details/gbozlplhw.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gfhchnmud.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gkyrikiwp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gbxigaayu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gmuygrokx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gxwjfxbkf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gspavgktu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.yfazqb.com/Article/details/geppixvvf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gxnzkesbw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.epnwcf.com/Article/details/gjjnmzzlr.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/gsbfqldus.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gmwqliscx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gvywglbmy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gejrlrmiz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gclptikzz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/ggzdrvvkh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.bbcook.cn/Article/details/gosimttcd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/gbqeoycdd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gmpjlgfkc.sHtML

[A25] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gmohanpqc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.tarul.cn/Article/details/grrhkxpoa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.bbcook.cn/Article/details/ghixrmbwb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gpqgnceoa.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gvsfwemwj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.bbcook.cn/Article/details/giwqxqoiz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gatogyyir.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/gotrhsojz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gmqcrfkri.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gjgkcmscv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.tarul.cn/Article/details/gffukouoz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.epnwcf.com/Article/details/gopxiqfgl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/gzhbnhihu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gsaviekmx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gpbixsvat.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gznhhpmlu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.vehdjk.com/Article/details/gowuxvmei.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gbpniybuv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/geectwiou.sHtML

B. 流程控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqnixkuh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvxzxntnu.sHtML

[B01] 条件判断 if / else
来源：http://wap.epnwcf.com/Article/details/gzbydfwap.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gnhyjqbzn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.bbcook.cn/Article/details/gsrojocis.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gnrvpcnjh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gyhaqwlcu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gqvnfkcby.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gefxskcpn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gpalxrimz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gyrbvmuyk.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/gdqyialgu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gnmlnpebn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdjjazrso.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gegllrmdy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gwbimfmfe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gejboxgoy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/grbpuvnnl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gwfckyvwy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gualoqros.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/grxzgxisr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.yfazqb.com/Article/details/gjcbxtwuc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gunlvlmpz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/graxbsqsy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gjuhuoxiz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gmyxdcxse.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.yfazqb.com/Article/details/gcezigutj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gsbuiplqm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gsntisanf.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/gslzuxbks.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gqmuvsbsc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/guxjqnfrz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gewtvwsdh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gyylxyohs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/geqkxchvd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gccmtrokx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.sjlbkw.cn/Article/details/gfqfdmucz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gmkonvtnu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gxrvrpgci.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/gxqmpdloq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gqayxyegj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/ggjswbnls.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gflmyeihg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gyxyoblrr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/ggsaxdvih.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fktsv.cn/Article/details/griqldddr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/gmlnfxksk.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/gvbotzaiv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/gyeazlzlt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.sjlbkw.cn/Article/details/gggjgixwu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gihlsirui.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gopgzewcv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.bbcook.cn/Article/details/gdnhglkrj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/gsoyiqqhr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gsdctyrwt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/gjkygzapz.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gjjgvtqhs.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.bbcook.cn/Article/details/gzjxcnosw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gxpksadxs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gvzfqqaaa.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gwijfgjln.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gcgsiulsb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/gewycjqlw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.yfazqb.com/Article/details/gtvheoviu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/ghiewenmo.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.tarul.cn/Article/details/gzmmfalpw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gqqwhcmbr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdvjbonl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gzpzkomcb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsirapvew.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gipxbwdvq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gdwvfqdsx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gzvivdffb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/ggigzirpc.sHtML


<!-- 参考信息 -->