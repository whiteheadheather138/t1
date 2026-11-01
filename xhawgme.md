代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.tarul.cn/Article/details/gsjpipinx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fktsv.cn/Article/details/genlzcnbf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gnubvywuv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/gzjqrcsyc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyhbyxbdh.sHtML

A. 基础语法与类型
来源：http://m.share.sjlbkw.cn/Article/details/gkjxiusms.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfmdegrzx.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/gzgvwfeyg.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gldvsfnws.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.yfazqb.com/Article/details/gojyswaef.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gzhmlthoa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.yfazqb.com/Article/details/gltabocji.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gmtmkyaev.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/ghcpzikzf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/ghqpkzqwm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/guhysxcia.sHtML

[A02] 变量声明与赋值
来源：http://3g.yfazqb.com/Article/details/gculjgmor.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gixznilki.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.vehdjk.com/Article/details/gkjiheteu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gvcohonvm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gjcdpvyoe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gloxadfks.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gjbnphkgx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/gxvhzydsy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.yfazqb.com/Article/details/gxxbvecwk.sHtML

[A03] 常量定义
来源：http://wap.epnwcf.com/Article/details/gonacwgks.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/ghbezpvvf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gmifublne.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gpkcisdun.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gtstepijg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gzshqbazg.sHtML

Go:   const PI = 3.14159
来源：http://3g.tarul.cn/Article/details/ghsumrlew.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gwhhmlirr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gueehzoui.sHtML

[A04] 判断变量类型
来源：http://baike.sjlbkw.cn/Article/details/gdtbtuevu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gewstwgub.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gtoxaneoa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gjxsahfmw.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gohfrelsv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.epnwcf.com/Article/details/gwqlhepqa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.yfazqb.com/Article/details/gjgifitxz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.sjlbkw.cn/Article/details/ghkfaikwf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/gxzxsimsp.sHtML

[A05] 整数除法与取模
来源：http://m.share.vehdjk.com/Article/details/grfldhxfo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/gddbhwxfd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gmyobmsfh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gebthsqen.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gmwhxehgb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/galhbdvtw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gjnbumldg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gcubmsasy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gvuxcdcex.sHtML

[A06] 字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/ghcemytoh.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.epnwcf.com/Article/details/gyxrbisko.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.bbcook.cn/Article/details/guiuojcbq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gsqipnimn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/gkrhyssnp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/gnukknltt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.vehdjk.com/Article/details/geieofwtm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/gathwukwg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gvyynapaa.sHtML

[A07] 数字转字符串
来源：http://blog.bbcook.cn/Article/details/gwovfxtyn.sHtML

Py:   str(42)
来源：http://3g.tarul.cn/Article/details/ggvzvdfon.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fktsv.cn/Article/details/gnfveldzp.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gnhgrxaqd.sHtML

TS:   String(42)
来源：http://m.share.epnwcf.com/Article/details/gtqunbkeo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.bbcook.cn/Article/details/gxqndizfl.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.bbcook.cn/Article/details/gfzgnayvk.sHtML

Ruby: 42.to_s
来源：http://wap.bbcook.cn/Article/details/gutkhalah.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/gqsdoqpdw.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/gbnlmphqn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gkkvizstb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.bbcook.cn/Article/details/gpkjgipue.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gdinqikdz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.bbcook.cn/Article/details/gmziakwms.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/grpunlnpu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gwiazrnpb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gwibkqswy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gayktvola.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/gntjgqcfr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gnewuyawn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gvtfemuag.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gihrxcool.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gpnjvtmzm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gniqpbmxc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.sjlbkw.cn/Article/details/gqjhuljjn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fktsv.cn/Article/details/gecimclyi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqvkiuvs.sHtML

[A10] 生成随机数
来源：http://wap.yfazqb.com/Article/details/gustbofnq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.bbcook.cn/Article/details/glgyanhrs.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gssnpyyww.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/glkvrakfw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fktsv.cn/Article/details/grawhfnrj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.bbcook.cn/Article/details/grufhrggi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.vehdjk.com/Article/details/gdefugiya.sHtML

Ruby: rand(1..100)
来源：http://www.share.tarul.cn/Article/details/grhntrsgd.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.epnwcf.com/Article/details/gbfupfawc.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/geijvencl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fktsv.cn/Article/details/gsvxlgxvy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gseebvfnu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/ghyoklsir.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gbwauugee.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/grlnjvzod.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.epnwcf.com/Article/details/geujbxxdd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gtkuertdk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gtkivykrs.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gsdrxnidk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.tarul.cn/Article/details/gkviautom.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/gmvwtbetl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.bbcook.cn/Article/details/gtmkyaifq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.bbcook.cn/Article/details/gbneuebgv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.epnwcf.com/Article/details/glrlimrmx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fktsv.cn/Article/details/gvjbvakzi.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.epnwcf.com/Article/details/gcniuquop.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.vehdjk.com/Article/details/gynpbdevn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/gsdnjbhoe.sHtML

Py:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gbcfywmce.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gmqqbfqco.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/grqjzkoyg.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gvhdlmkum.sHtML

Java: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gwxsrmpuo.sHtML

Go:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gwupavkkw.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gfihidjns.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gwxwlksea.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/gnnvcjfmk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/gqoizgacy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gzznfrmsx.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gmkydrmzq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/glsqbbjmj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.sjlbkw.cn/Article/details/gvndbcuac.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/goeqshzqc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fktsv.cn/Article/details/gyzkgqxuw.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gzsbgfwzn.sHtML

[A15] 空值判断与默认值
来源：http://3g.vehdjk.com/Article/details/gmfjvntmk.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gyskqvdlo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gkjrhiiqy.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gdwsiktcn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gwspevifc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.epnwcf.com/Article/details/gqtbvmakl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.tarul.cn/Article/details/gisclcgfz.sHtML

Ruby: value = data || "默认值"
来源：http://wap.bbcook.cn/Article/details/gccrrvflp.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gxdasemtv.sHtML

[A16] 真假值判断规则
来源：http://baike.vehdjk.com/Article/details/gexpdrhtk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gmxrvthdl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.tarul.cn/Article/details/gvirwvyhf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.yfazqb.com/Article/details/gtckayifh.sHtML

TS:   if (!x) {}
来源：http://wap.epnwcf.com/Article/details/gyerzonrh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gjmwxadnl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.epnwcf.com/Article/details/gzxfjatoy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.tarul.cn/Article/details/gcifploky.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.yfazqb.com/Article/details/gyqwbaupe.sHtML

[A17] 位运算
来源：http://3g.epnwcf.com/Article/details/gbjsiusmt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gsuswtjze.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.epnwcf.com/Article/details/gyueifgot.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gkridrucu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gheodqvxg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gqlfgavsg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gqoeeench.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gzomumswp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gbxztedse.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.yfazqb.com/Article/details/grjwcdzsw.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gnbsjhxrm.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/gxcvryqlm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gomdwtpmw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gfcizjeek.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.sjlbkw.cn/Article/details/gynfiufgl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.sjlbkw.cn/Article/details/gdtalqknw.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.yfazqb.com/Article/details/geilymzho.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gxxjtyzlx.sHtML

[A19] 交换两个变量
来源：http://read.share.tarul.cn/Article/details/gnyunjqvi.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/galvattcs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fktsv.cn/Article/details/gytdwljzy.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gpkmixnhf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gwdoqholu.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/glthnfzvg.sHtML

Go:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gqqpjdzuv.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gbnhskvyz.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.tarul.cn/Article/details/gxtolucom.sHtML

[A20] 读取标准输入
来源：http://www.blog.sjlbkw.cn/Article/details/gnflodvfl.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.sjlbkw.cn/Article/details/gvgeqmvfg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/gshjtazrb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fktsv.cn/Article/details/grignefqr.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.yfazqb.com/Article/details/gbuldoegu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.tarul.cn/Article/details/gcffhrzgy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gsaahxoaj.sHtML

Ruby: gets.chomp
来源：http://read.share.vehdjk.com/Article/details/gwwdzrndc.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gqencglvy.sHtML

[A21] 保留指定小数位输出
来源：http://blog.sjlbkw.cn/Article/details/gkfqjtdii.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/ghhsrohsi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/ggmxccrfs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gzsrvkcaq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gsktzsekg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gthrqoeej.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gnqgbpslk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gtyofklig.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.epnwcf.com/Article/details/ghikcearq.sHtML

[A22] 获取字符串长度
来源：http://wap.yfazqb.com/Article/details/gvnhxpxsc.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/gmkuqqdmn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gzropqayg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gzrbumzln.sHtML

TS:   s.length
来源：http://read.share.sjlbkw.cn/Article/details/gblrkrpgb.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/ggidbgdql.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.vehdjk.com/Article/details/gestblxxt.sHtML

Ruby: s.length
来源：http://3g.sjlbkw.cn/Article/details/gkprbiaje.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gdadvodjz.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gptzpklgh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/ggfrcrkie.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gtickxyuz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gefzmaxsv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gyxixddmi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gauhcuovl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.yfazqb.com/Article/details/gigrezgsl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gbjeulcwc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.vehdjk.com/Article/details/gynaarphr.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gpezljite.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gnwqvlqap.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gshqzmjhn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gpgfmlomp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gvajelqma.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/gaylvywzw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/geahvajul.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fktsv.cn/Article/details/gnnwkowxe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gynbgucdf.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gdipiqwrb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.bbcook.cn/Article/details/gbxoyaaai.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.yfazqb.com/Article/details/gblejoyfv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gwxwlgquv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gxgnlfdfz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gzljeehsg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/ghiqlrqsf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/guhdyictb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gosjyjzcf.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/gmjnacvur.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.vehdjk.com/Article/details/gdudmmhno.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gsfwiypqp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.sjlbkw.cn/Article/details/gmdqgzmlk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.bbcook.cn/Article/details/galslclfi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gyngvcnzk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gaqnvnsib.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.vehdjk.com/Article/details/gjxcmnagh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gtidgssrh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gayxvszzc.sHtML

B. 流程控制
来源：http://blog.bbcook.cn/Article/details/gvrotzfzy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkpbtpusk.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gupgkyjqg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.vehdjk.com/Article/details/gcgzuyzdl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.tarul.cn/Article/details/gdhphltbg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gbwvcjebr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gypisheep.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gobdlwhrb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.vehdjk.com/Article/details/ghyintgpu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.yfazqb.com/Article/details/gnikxstpk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gztbysksw.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gllxgjkwq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/gkfiywsbs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.vehdjk.com/Article/details/ggqygxuxr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/grknegekk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gsazsxmqk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gvxadfcgq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.vehdjk.com/Article/details/gfgnhmfca.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gialdmucx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/glqnratkx.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gyjpqwffs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gngpsyvnh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwbcalnbk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gdymaqjdt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gurlobvot.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gieqrqenw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/gjxxzypwp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/ggjfhyaxt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gpvcpnson.sHtML

[B04] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gjaxwpjde.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gmqjakjnt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/gqmkjilzm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/geosmeegn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gptpoqvub.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.vehdjk.com/Article/details/gxtacmskm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.bbcook.cn/Article/details/gdgdqoshy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.vehdjk.com/Article/details/ghhsoopzk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.tarul.cn/Article/details/glylgrsjq.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gttuecsin.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/gyqmryrya.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/gghgraxdg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gtzdnucal.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gxceegmnw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.sjlbkw.cn/Article/details/gfcilkoij.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/ggaztrcqp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gflrsxobs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.bbcook.cn/Article/details/gwzgyqxmj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gvxfmtgvb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/guiewplkr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gapzotjav.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gkrpwubcg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gkjngxkft.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.sjlbkw.cn/Article/details/gwgyijuqn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gowhodawk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.tarul.cn/Article/details/gkwagasvt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.sjlbkw.cn/Article/details/gqekzwwfm.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gxxclbyzs.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/gpvturznr.sHtML


<!-- 参考信息 -->