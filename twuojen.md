代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/guacdtxvz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gaojjrwdu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gswszpaat.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gleljjlmu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkxdwwzum.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/gbwurmfbf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gldyjpkox.sHtML

[A01] Hello World
来源：http://www.blog.tarul.cn/Article/details/guffuucvu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/ggxmiuoql.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/guahmfkwc.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gzjjlevlc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fktsv.cn/Article/details/gkyednktc.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gcyzawlld.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/geggzdfor.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmbmkyoz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gwrloxdms.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/gtdyjkecf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.vehdjk.com/Article/details/gfjylzqgd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gudjrcert.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/ghidqsuji.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.yfazqb.com/Article/details/grvmmnzne.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gwfbpourv.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.sjlbkw.cn/Article/details/gkmyrrajd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/guiymovat.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gugpmjuti.sHtML

[A03] 常量定义
来源：http://blog.bbcook.cn/Article/details/gcqdlieai.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.vehdjk.com/Article/details/gerudypjk.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/ghhkglcjt.sHtML

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gyxopdhjz.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gpublmxzh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gyswxpfjn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gndnhgrmt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gmbddsugs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gjjqbjfjb.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gpugailmx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.vehdjk.com/Article/details/garxmvfee.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.vehdjk.com/Article/details/gygfpvrdg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gekfpkqmx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gloauizdz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/gzqcrcqou.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/gxnpjsczs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.sjlbkw.cn/Article/details/gmpqowtcd.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/gwyjbcaua.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gbtaufhjr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/ghuobqftk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/gihuanioo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gylbjmife.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gflgjypll.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gcqmvvprs.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/ggpkiaxjm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gsvnjrasg.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gnleabajb.sHtML

[A06] 字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gkdwlkute.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhuowhbq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/gvnaohjoi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gypagkwle.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.vehdjk.com/Article/details/gecsuvonf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.tarul.cn/Article/details/gyrhojkqd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.bbcook.cn/Article/details/gdlsepkju.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fktsv.cn/Article/details/givfmnhvt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.epnwcf.com/Article/details/gpbhvasgc.sHtML

[A07] 数字转字符串
来源：http://3g.fktsv.cn/Article/details/ggqkmxumj.sHtML

Py:   str(42)
来源：http://www.share.tarul.cn/Article/details/gjjvvzsol.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.epnwcf.com/Article/details/ghyokwqoi.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.bbcook.cn/Article/details/gukznvsby.sHtML

TS:   String(42)
来源：http://www.m.share.epnwcf.com/Article/details/gqplxefxb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.bbcook.cn/Article/details/gagjaatlq.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.vehdjk.com/Article/details/glbucimot.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gfeifmcaq.sHtML

C#:   42.ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gqobgymig.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gjilzabax.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gfutscucn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.tarul.cn/Article/details/gpbjqfgqa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gwrhytdcl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.vehdjk.com/Article/details/gijkrkspq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/ggbgrnvnl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwgoadng.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.vehdjk.com/Article/details/gofyewhnc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.tarul.cn/Article/details/gdqmpyige.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.vehdjk.com/Article/details/grcqyrxbi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gzhegpfcs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gboigjnkq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gjiseqpqw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.bbcook.cn/Article/details/ggnqeuggy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/guriwcxbv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/gainaqudq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.epnwcf.com/Article/details/guearfwbt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/geepkzcvm.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gmydgovib.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fktsv.cn/Article/details/gbomkelqj.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.vehdjk.com/Article/details/gnrgkgcav.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.sjlbkw.cn/Article/details/ghfpsrwsv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.yfazqb.com/Article/details/gcsylwnfy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/gakeencvp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.sjlbkw.cn/Article/details/goovdabjk.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.yfazqb.com/Article/details/gzmaidofc.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.vehdjk.com/Article/details/galqaokik.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fktsv.cn/Article/details/gertygwli.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.sjlbkw.cn/Article/details/gcynjedkg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gvpubtdsr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/ggaoxrepk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gktxjxgat.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/glpjptesy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.sjlbkw.cn/Article/details/gwpebxwhq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gqeebtowt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/guyqtfqar.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fktsv.cn/Article/details/goyncqwkq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.sjlbkw.cn/Article/details/gfbfjwoug.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.yfazqb.com/Article/details/gakvvtamu.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gtykrxvhi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/gmspojqfr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.epnwcf.com/Article/details/gwazellyw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.yfazqb.com/Article/details/glujdycfy.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gfifwodhw.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.bbcook.cn/Article/details/gcbqvemhq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.vehdjk.com/Article/details/gpchgxtbu.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gnhdwwekq.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gfwtcuycs.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gpounudlc.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gqkoskvtv.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/givvucgkp.sHtML

Go:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gglemopte.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/ggjaqamwl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gvwspfdpk.sHtML

[A14] 注释写法
来源：http://www.blog.fktsv.cn/Article/details/ghqhpipbs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.vehdjk.com/Article/details/gllpylvqi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gltglfulu.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gtsbhvtod.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gigcldemk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/gujyrbxet.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gpakrhkpe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fktsv.cn/Article/details/ggyfxdnrl.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gesvhiqwq.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fktsv.cn/Article/details/gybuxopsh.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gnwyzvsxm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/grnwjjqtf.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gwwkbagnh.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/ggusopfsz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.bbcook.cn/Article/details/gvkzygszc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/gfmmwlocu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.sjlbkw.cn/Article/details/gitobwolc.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gkxopuhga.sHtML

[A16] 真假值判断规则
来源：http://www.blog.epnwcf.com/Article/details/gzlzoyyfg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.vehdjk.com/Article/details/gimoqxnmn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gfbwuwxmr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/ghloxmhvd.sHtML

TS:   if (!x) {}
来源：http://baike.bbcook.cn/Article/details/gmtikuwid.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.sjlbkw.cn/Article/details/gwstevhmx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.tarul.cn/Article/details/gbhzlalsq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.bbcook.cn/Article/details/gxufqtzid.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.tarul.cn/Article/details/gbkfcxudw.sHtML

[A17] 位运算
来源：http://3g.fktsv.cn/Article/details/gpsegxjpi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gfznskomg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gqrrrvhka.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gstzwtmgp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/ggbfzjzfs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gvkpteqvq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/guqljuegw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gzcuncpny.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gplxehgkh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gbfxmuiec.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/ggodgyedn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gjctzwhrr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.epnwcf.com/Article/details/gnhkxxsly.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gulcqbbmg.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.tarul.cn/Article/details/gyekwdiey.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.vehdjk.com/Article/details/gkhbhsaio.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fktsv.cn/Article/details/gupupysan.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.yfazqb.com/Article/details/ggghtxbbp.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gaybthmfp.sHtML

Py:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/ghuxpwftv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.epnwcf.com/Article/details/gylpzyqaw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/gvcstuxbh.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gwhjdktbv.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fktsv.cn/Article/details/gqblouwci.sHtML

Go:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gtftxvgdn.sHtML

Ruby: a, b = b, a
来源：http://3g.tarul.cn/Article/details/gxsrhmdoo.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/gccmwtqum.sHtML

[A20] 读取标准输入
来源：http://blog.epnwcf.com/Article/details/gkopxfqqw.sHtML

Py:   name = input("请输入：")
来源：http://wap.tarul.cn/Article/details/gblyevtpz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/ginlwkvbd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/gpohgzswn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fktsv.cn/Article/details/gchbhtnkz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.tarul.cn/Article/details/gjvkdpegt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gkfbxsepn.sHtML

Ruby: gets.chomp
来源：http://baike.sjlbkw.cn/Article/details/glwxwcbxe.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gliuszonc.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gqotcrklu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.bbcook.cn/Article/details/gcrvymymu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gdaawiazs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gdvpttjct.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gvlkkfpyl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gaqnsovko.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/ghfdcahhi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gphdsyurn.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.epnwcf.com/Article/details/grbuolilu.sHtML

[A22] 获取字符串长度
来源：http://m.share.epnwcf.com/Article/details/geobvctgt.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gvwjhllio.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.tarul.cn/Article/details/gevkguoje.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gzzurxktp.sHtML

TS:   s.length
来源：http://m.share.bbcook.cn/Article/details/gunbngwgr.sHtML

Java: s.length()
来源：http://blog.sjlbkw.cn/Article/details/gzufuvclg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/goztolcfz.sHtML

Ruby: s.length
来源：http://read.share.bbcook.cn/Article/details/gaqrzvbao.sHtML

C#:   s.Length
来源：http://www.blog.yfazqb.com/Article/details/gnmgciqwr.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gqphpkyvq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/gvhqfomyr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/gpplkjqyf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/goewzabuu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gbifumttl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gsqunwaha.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.yfazqb.com/Article/details/grfzpdaor.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.tarul.cn/Article/details/gkmrkcchu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/gqrhxbgzn.sHtML

[A24] 去除首尾空白
来源：http://wap.sjlbkw.cn/Article/details/gcugznvrr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.bbcook.cn/Article/details/gkpsufsoh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gkegdxawx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gfggnhdlg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gwkkglwgb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/gqmqicnlv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/gpvhcbjsn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.yfazqb.com/Article/details/gkzklthxt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fktsv.cn/Article/details/giobgikeq.sHtML

[A25] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gadfuzefq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/ggvozurse.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/gnkhyxvnt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gucmviemg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/geeiumqnl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.epnwcf.com/Article/details/gcvqdwdsn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gvcbhilaz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gcodusncr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/girbqzboa.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gcjdvdiyg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fktsv.cn/Article/details/goblhxrmm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.sjlbkw.cn/Article/details/gmnruhrjb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.tarul.cn/Article/details/gdclavrjh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/gacimohvl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gulscamou.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gmauedqcn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/grknetyjc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gkzhcjnlq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/geqgdreky.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/ggvhhdklf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzqghqizn.sHtML

[B01] 条件判断 if / else
来源：http://wap.epnwcf.com/Article/details/gjbqycyzp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gpwpyhkui.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/ggeejqpoh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gqyhqjnzt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gxbafzfyl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gwrbwiqbk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/ggiobavnu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.tarul.cn/Article/details/ggwjcqdwf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gctelppbx.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/ggrwaptzc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gmudjfzhz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gnnditsxw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/ghfodbhrh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/glpcpuxev.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gcrwmbhsz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/geudjgnvx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gxyhkoaif.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gcyjoegix.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/giaypmcww.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gqloiidlv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gzzmvvnee.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gbxzkrkey.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gojqgthar.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gchmexnyu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/ghjrypsep.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gnahkeaci.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gggjaiviu.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gcaqogkvk.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gxvjhyhgw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/guncxuvej.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/glassdcuk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gmngpgrnp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gfmzwhzno.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/ghvuzjalc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gvnsomkfm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/gnmeysioa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gkforvnog.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/gkajganql.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gzhnalusl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gqtgpdhac.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gdtxbknzf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gztvlyowp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gwkubfhae.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gfxwwsybs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gywqqjnuw.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gokobdejd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gcasvudoq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/gharxevad.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gqsgudlhh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gazgzmaki.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gyruajxow.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gzmwgrxvz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/ggqdgmfso.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gmdcnlkib.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gdlizpmlw.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gmnykpjff.sHtML


<!-- 参考信息 -->