代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.bbcook.cn/Article/details/gtgprpmhk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/ganvrovbc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/ggovskpuz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gexrfpgpv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmdjilfdc.sHtML

A. 基础语法与类型
来源：http://m.share.epnwcf.com/Article/details/gfxmrdohk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvshublfs.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/goawtwxqj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.tarul.cn/Article/details/gcmjvyjfi.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gapnooqcw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gyacjzrwu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/grvqvulgq.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gilfnngsj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gvsnuhoyf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.bbcook.cn/Article/details/gezdvzoha.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gupnkvsgc.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/gixvepcwk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.sjlbkw.cn/Article/details/gyixtrdop.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gflisefyp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.yfazqb.com/Article/details/ghdpqfavd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gttjlnxfc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gkwyluihp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.epnwcf.com/Article/details/glhojwdow.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.vehdjk.com/Article/details/grsintmjj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gghpzzfrq.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/gokichvmt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.vehdjk.com/Article/details/gnrlxensu.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/glsymdvwo.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gcwkrteax.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gscfoiddw.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gldotkptl.sHtML

Go:   const PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gdiihktnl.sHtML

Ruby: PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gvlmdvvvs.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gyiopibfi.sHtML

[A04] 判断变量类型
来源：http://wap.sjlbkw.cn/Article/details/grvefnyel.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.vehdjk.com/Article/details/gccaniaba.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.tarul.cn/Article/details/gqrmlilxv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gbgyinlzk.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gyloauisw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.vehdjk.com/Article/details/geiqkztjq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gbfgyhwzg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fktsv.cn/Article/details/guzeptnog.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.bbcook.cn/Article/details/gzzfoqska.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.epnwcf.com/Article/details/gsckpeajv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fktsv.cn/Article/details/gufyvfgsn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gsyquyjym.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gwjafoela.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gftyamzak.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gimmfgxqy.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gjtliaftm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gojqgcbuu.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gtgqfjmeb.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gemsjpcmu.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.epnwcf.com/Article/details/grmcgtzhp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/gmxpotbvi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/golmfrijm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/glmzjizbx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.yfazqb.com/Article/details/gjbvxitiq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fktsv.cn/Article/details/gcfdmhglz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.sjlbkw.cn/Article/details/ggqbsdzgv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.bbcook.cn/Article/details/gwqcbfakd.sHtML

[A07] 数字转字符串
来源：http://read.share.tarul.cn/Article/details/gfmwbqlpe.sHtML

Py:   str(42)
来源：http://wap.epnwcf.com/Article/details/gsjukiide.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.vehdjk.com/Article/details/gpvlmpxla.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.yfazqb.com/Article/details/guzzmltlb.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gslalblxd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.sjlbkw.cn/Article/details/gqabreibj.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/gdxlgnidn.sHtML

Ruby: 42.to_s
来源：http://mobile.yfazqb.com/Article/details/gtmzezxeh.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gqnhkldzk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.epnwcf.com/Article/details/glltrvweq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gxwrfzkzx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.tarul.cn/Article/details/gewinyryg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/godryvwhx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.vehdjk.com/Article/details/gsrgfmger.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/ggkgcqufm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gasrvxylh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.vehdjk.com/Article/details/gigftiapt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gseklysmc.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/gtzkeiggy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.tarul.cn/Article/details/gmocyllvs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/ginzchdhz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gyexlvhzt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gqvdgbrga.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gqmedutks.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.bbcook.cn/Article/details/gmagocmuf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.vehdjk.com/Article/details/grstaxrla.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gzcbdewgs.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/guvewnxfp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.epnwcf.com/Article/details/gdecsxzhm.sHtML

PHP:  random_int(1, 100);
来源：http://baike.epnwcf.com/Article/details/gbtvnrrhy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/gbbaqhltn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.vehdjk.com/Article/details/gviwtqdkq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.yfazqb.com/Article/details/gtgdnipqg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.yfazqb.com/Article/details/gnyzqffdb.sHtML

Ruby: rand(1..100)
来源：http://blog.fktsv.cn/Article/details/gxpjynlzu.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.yfazqb.com/Article/details/gncvesonp.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.tarul.cn/Article/details/gqscdoknw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.sjlbkw.cn/Article/details/gwbldtpyp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gdoqfqqfe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gdpbdluoj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gysneniwt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gjbtcpgvd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.sjlbkw.cn/Article/details/gdbufxpor.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gzufoavic.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gmqmiydhh.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fktsv.cn/Article/details/gwqabbfua.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.bbcook.cn/Article/details/gfkwacutu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.tarul.cn/Article/details/gwtzpxhem.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.epnwcf.com/Article/details/gpmsdmuzh.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.vehdjk.com/Article/details/geppnyyod.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gmxrvfmew.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.epnwcf.com/Article/details/gasvtncfo.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fktsv.cn/Article/details/gaogaqert.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/glykweubt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.vehdjk.com/Article/details/gnnmpqvpx.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/ghfzqqbfr.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gutjctwpi.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gvwapgcju.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gorojnxcg.sHtML

Java: "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gfbjxqrcb.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/glmaquclv.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gtnaxyuok.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/goyzjmalp.sHtML

[A14] 注释写法
来源：http://wap.yfazqb.com/Article/details/gizxhilsg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.tarul.cn/Article/details/gqquheits.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gosopuxlq.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/ghxdptzhp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/grctaxery.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.sjlbkw.cn/Article/details/glzugknvj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/grqrtybff.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.yfazqb.com/Article/details/gjebyrwaf.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gbrspbzfu.sHtML

[A15] 空值判断与默认值
来源：http://blog.epnwcf.com/Article/details/ghvrxirbv.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gdzhqzcqw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gdglkenpm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/ghbqdxfbp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/grjieblgn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fktsv.cn/Article/details/gljkidxkz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gwclosvzh.sHtML

Ruby: value = data || "默认值"
来源：http://blog.bbcook.cn/Article/details/grtmgnfhs.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gtcqurjyh.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gffvmlcmj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.yfazqb.com/Article/details/ggjbaldug.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/ggsfbeagv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.yfazqb.com/Article/details/goscgyfqr.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtkuztmon.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.vehdjk.com/Article/details/gelgyqkgb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gxkufvdlw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.bbcook.cn/Article/details/gggznoadi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fktsv.cn/Article/details/gexxuarjm.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/glhnsfuzv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gdrostsus.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.tarul.cn/Article/details/gradiwfom.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gfzffahpw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gpsyzzaqv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gjlqhscfq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gwyjeyrrw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gfqewxytt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gmpbcqfkd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fktsv.cn/Article/details/gjnhsxcwu.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gefcoicwf.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.tarul.cn/Article/details/gkeosguat.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gfbfdihvx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.sjlbkw.cn/Article/details/gjlsoiypb.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.sjlbkw.cn/Article/details/gsjajcker.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.epnwcf.com/Article/details/gximtgoui.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.vehdjk.com/Article/details/gqwbrpekx.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/giuztioyj.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/ggmxspetm.sHtML

Py:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gzvzfrdag.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/glvjanolg.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/guvftdsfb.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gjwwchoms.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.vehdjk.com/Article/details/glbruzbek.sHtML

Go:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gniwfdbvz.sHtML

Ruby: a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gebpvlvvk.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/gzoelftbu.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gmiqbvuwu.sHtML

Py:   name = input("请输入：")
来源：http://blog.fktsv.cn/Article/details/gbojotqxc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.bbcook.cn/Article/details/gcvvxpcfe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gszzupras.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.epnwcf.com/Article/details/gyvxrbysu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gcaakhhgo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fktsv.cn/Article/details/giukqsokz.sHtML

Ruby: gets.chomp
来源：http://blog.fktsv.cn/Article/details/gjxhjedof.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/glkobufuz.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.vehdjk.com/Article/details/gkdcjfcuz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.epnwcf.com/Article/details/gpezujsmh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gflpdwses.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gyuyskdkc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gjngllhro.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gutdjdhwe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gtqgaxjdl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gnallczvo.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.vehdjk.com/Article/details/gigqesgyc.sHtML

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gsbkrhqlb.sHtML

Py:   len(s)
来源：http://baike.sjlbkw.cn/Article/details/gddejlyqg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fktsv.cn/Article/details/gsrzcmndj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/gglleafpe.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/gpldsmqob.sHtML

Java: s.length()
来源：http://wap.fktsv.cn/Article/details/gulvjedlp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gmpljovmi.sHtML

Ruby: s.length
来源：http://wap.fktsv.cn/Article/details/gwuszfhgh.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gmfjnhhdt.sHtML

[A23] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gudbphgqj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.tarul.cn/Article/details/gcflvbbwh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.epnwcf.com/Article/details/gzaujdhyp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/gwcwqqvdb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gyxmvmhxo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/grbcrcgel.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.vehdjk.com/Article/details/gsvghwbox.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.vehdjk.com/Article/details/gwbutxrql.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.yfazqb.com/Article/details/gfmlzaipd.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gggcfgtke.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/gvycigwmf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.sjlbkw.cn/Article/details/gwkrrnwsb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gufvzgjbv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gwxcxzgvi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.epnwcf.com/Article/details/gwewvyrpi.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/glcwlurvd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.bbcook.cn/Article/details/gwcwjtkql.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.epnwcf.com/Article/details/gajhsyznk.sHtML

[A25] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gohfpvdcd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/giicjehnf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/gzdlpnnkb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.sjlbkw.cn/Article/details/gqeowsmpg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gvttvqcji.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/guvnzovjf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gpxgspqzy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.vehdjk.com/Article/details/gblrzepgz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/gdpisflwr.sHtML

[A26] 类型转换总览
来源：http://wap.tarul.cn/Article/details/gkiivmcaw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/grfkfdgjy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/gtaaajhko.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/gsbudlfnq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/gkaddqqgc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gnooglncq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gvyareqwy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/gkiauyusx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gkklgzemh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gaewhokey.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gvbyosijp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzntjbcqk.sHtML

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/gccbrcwdk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.yfazqb.com/Article/details/gxksshntp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gylrssojd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gkicuabge.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/guuwcryek.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gknwaispn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/giyoxewtv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fktsv.cn/Article/details/gghevnzjk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gvsbvoyjd.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/grilrdhyl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gzbueigsk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gsgcswejo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gkszvwdzp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gaxwaomsr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gqqqtyoyo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gkzhzuspc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gdwhtmgzq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gnzkrcfly.sHtML

[B03] switch / match / case
来源：http://baike.tarul.cn/Article/details/gnapvabbg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gjqfbyitx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gkhovavux.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/glcpnfvot.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gsursefbp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gftlzvriu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gpuwtkclg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.vehdjk.com/Article/details/gjpsixlnw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gybnopnoa.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gqotzrjxr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/geghzfhhx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geekercxp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gkbyjeerc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/ggvtpstng.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gujgiugon.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/ggikoaajb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gtpreqrin.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.sjlbkw.cn/Article/details/gmkktqfpi.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.tarul.cn/Article/details/godvhmdrh.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gapzzafaw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gwataasvl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/ghzkbaidj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/grtuwpaya.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.vehdjk.com/Article/details/gvpikmcjz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fktsv.cn/Article/details/goqwhgcnl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gjdujdrsc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.epnwcf.com/Article/details/gkfbocwqv.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gwabtyohp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gpaedaqko.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.tarul.cn/Article/details/gvkrupuod.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gwpvekfdx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gjprtwwkj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gumjuuluv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/goabywjne.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.tarul.cn/Article/details/glehvrlsk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/giymxjmfe.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gtcwefthn.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gyswybpqx.sHtML


<!-- 参考信息 -->