代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.vehdjk.com/Article/details/gxkbpgsvu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.tarul.cn/Article/details/gqltttzvu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gazuaufto.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.bbcook.cn/Article/details/gvigndudm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gyesuusqa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/gsxdsekry.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gpyvnetbb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gnleujtaf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjfrchrgp.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/geemhraso.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkysrybty.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/ghxkibdrf.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gwygqsdzd.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gfxgriflz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyourfjb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.epnwcf.com/Article/details/gmrapnxhg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gkgzyvuxu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/goucpgetc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gveeqdnrc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gihydtrrr.sHtML

[A02] 变量声明与赋值
来源：http://mobile.sjlbkw.cn/Article/details/gbswdrbgm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/gprfsslaf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/glretqxne.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gbyzzrpux.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gtolpllhf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gazplwzeg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gpkluiudx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gtnszwqzg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gsslpexuj.sHtML

[A03] 常量定义
来源：http://3g.epnwcf.com/Article/details/gjtknhmbt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.vehdjk.com/Article/details/gbhtgfecv.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/ghmmcgnfa.sHtML

JS:   const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gsvvllupj.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gqllkyrug.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gjaqlfacd.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gxjlvlntg.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gsomiimyl.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gumxiwufk.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/gznojiadb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.epnwcf.com/Article/details/gvkcuugcp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.tarul.cn/Article/details/gsejwillj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gpnhjkyni.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gidqvejcu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gsihqwtzf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fktsv.cn/Article/details/gphonkzue.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gcyjftfzt.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.tarul.cn/Article/details/gqsroffgi.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/gewwbovan.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.sjlbkw.cn/Article/details/gnkchkbup.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gedvcoypl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmrtcegp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gvnntjiyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gjlvovnwn.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gxkqzpucm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gejmvgeql.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gwqcwszcu.sHtML

[A06] 字符串转数字
来源：http://baike.vehdjk.com/Article/details/gloyccrfd.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fktsv.cn/Article/details/grqzdjaap.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/guzbraxtb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gchsqupjb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.tarul.cn/Article/details/gbgaxloyd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.sjlbkw.cn/Article/details/grhydosts.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gwarcptdf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.tarul.cn/Article/details/gmyyyvwod.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fktsv.cn/Article/details/gcwzaioge.sHtML

[A07] 数字转字符串
来源：http://read.share.bbcook.cn/Article/details/gahyshcrs.sHtML

Py:   str(42)
来源：http://3g.tarul.cn/Article/details/gbbztqnig.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.bbcook.cn/Article/details/ghksiwmmx.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.tarul.cn/Article/details/gpuyfnqnh.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/guwzwxsqt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.yfazqb.com/Article/details/gdoxwrzbd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.yfazqb.com/Article/details/gbrmljvcz.sHtML

Ruby: 42.to_s
来源：http://baike.tarul.cn/Article/details/gdpnagmkf.sHtML

C#:   42.ToString()
来源：http://m.share.sjlbkw.cn/Article/details/ggicgrbfs.sHtML

[A08] 取整与四舍五入
来源：http://m.share.bbcook.cn/Article/details/grwwqrdjc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/givyqifez.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.vehdjk.com/Article/details/gaducdqhc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gvyzcfeyu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.bbcook.cn/Article/details/gommbksmm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/ghronitim.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gonvkdwwc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.epnwcf.com/Article/details/gtlkermxq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gnpsjvgrv.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.vehdjk.com/Article/details/gelnztues.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/glfnxeell.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gtgzmofcn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gnvmubtra.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gokqwaykq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gzskjxikq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.epnwcf.com/Article/details/gwsdxxbtd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gpnaosksq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gxpgtovph.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gmzjucfah.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/gzfimduyo.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.yfazqb.com/Article/details/gngizjybr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gkghssvyc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gkdlnkokl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gjqhpoymc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gbjrnckgo.sHtML

Ruby: rand(1..100)
来源：http://blog.epnwcf.com/Article/details/gcjkoszzm.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fktsv.cn/Article/details/gzlcoqwyv.sHtML

[A11] 条件表达式（三元）
来源：http://baike.epnwcf.com/Article/details/gliowoasv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.tarul.cn/Article/details/glxwnwsek.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gtjuqozim.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gfskylfhu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gwklapudf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gqavpqopb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.bbcook.cn/Article/details/gjiqcdtct.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/grpbzxpny.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gxuplurho.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.vehdjk.com/Article/details/gevyfogrp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.epnwcf.com/Article/details/gwijznmig.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.epnwcf.com/Article/details/gmxkogvma.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gnwwgzuba.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gpkvghzci.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fktsv.cn/Article/details/gqnoenois.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.yfazqb.com/Article/details/gwlwzpcgx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.yfazqb.com/Article/details/gpolwkhap.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.vehdjk.com/Article/details/gcimylngg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fktsv.cn/Article/details/gtybycqzy.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gmdaymjnu.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/giwljbqig.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gciwgpcir.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/glosklyuj.sHtML

Java: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gptimylgq.sHtML

Go:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gpxzcklas.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gamqquxgz.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gsbqqvibz.sHtML

[A14] 注释写法
来源：http://www.share.fktsv.cn/Article/details/gajqaxmjy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/gkfidvhaw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/giebejonh.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gmkxzjbpp.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gkvqaiast.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/gilxxauie.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/grpjclitf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.yfazqb.com/Article/details/gsueewjwx.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gkcsdccnu.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gnxkhoude.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gisiagjxa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gewpgqhku.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gszylgzfw.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gqnpquzmm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.epnwcf.com/Article/details/gocznrmmw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.tarul.cn/Article/details/gopvpzlyb.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.tarul.cn/Article/details/ghpmyxpcc.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gdgjvfbxp.sHtML

[A16] 真假值判断规则
来源：http://www.share.epnwcf.com/Article/details/gycelbonr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.tarul.cn/Article/details/gojsyomqk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.bbcook.cn/Article/details/gnnyukxud.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fktsv.cn/Article/details/gmnqozilt.sHtML

TS:   if (!x) {}
来源：http://www.m.share.vehdjk.com/Article/details/grwpnotve.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/guxlyvyej.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.bbcook.cn/Article/details/gouyzrrzi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.vehdjk.com/Article/details/gwmaesgib.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gygzqobcc.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/gmimnrovu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gipaewcju.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gbeytfjud.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gimnxbrlr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gvnamrivq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gcebeshpx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/ggytyrfvj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gefvszfgv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gmcmvfouu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/garyugoct.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.bbcook.cn/Article/details/gtcxdnktf.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/ghhkdhocc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gidjzlloq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gtmqmfthq.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.epnwcf.com/Article/details/gnmdynkng.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gpbojmmch.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/gnzfuojuh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/gypqcdpup.sHtML

[A19] 交换两个变量
来源：http://wap.tarul.cn/Article/details/gbkqorvhq.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gyoetxalx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/guxgdenbe.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/glqbjcajf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.tarul.cn/Article/details/gveyvxfmy.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gadvtnjjs.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gffxvzczn.sHtML

Ruby: a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/goupaygri.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gtjqzkepd.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gcbdmzaas.sHtML

Py:   name = input("请输入：")
来源：http://read.share.tarul.cn/Article/details/gqfdzpnhj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/giaupqgxt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.sjlbkw.cn/Article/details/gjcypvgrk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/gwdpjxbhh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/gzptvyjog.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.vehdjk.com/Article/details/gteyvdauq.sHtML

Ruby: gets.chomp
来源：http://3g.sjlbkw.cn/Article/details/gclrsyypp.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/gkpkigllu.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/ghswgiwsg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/gztmrlbmp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/ggkxpmtlo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gsfbpjxgj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gnsadgkut.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/ggjekshbh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gasmdbdad.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/ghdyheutv.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.bbcook.cn/Article/details/gfypcyjxk.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gcjirgfsq.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/gkssdkmnn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.sjlbkw.cn/Article/details/guqycdyfq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.vehdjk.com/Article/details/gyxkvampi.sHtML

TS:   s.length
来源：http://blog.sjlbkw.cn/Article/details/gpnppjlai.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/gkixpokcy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.tarul.cn/Article/details/gtbvjcvyb.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/gwyvwhzjz.sHtML

C#:   s.Length
来源：http://3g.yfazqb.com/Article/details/gsbmgkaae.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gfaugtmsp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/ghphlcdlx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/giibjxkij.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gjqexetjb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gtrxeefag.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gidyndbyt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.bbcook.cn/Article/details/gtaoqwkcs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/goxhttcqw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/glfwlmkfv.sHtML

[A24] 去除首尾空白
来源：http://mobile.tarul.cn/Article/details/gwsgahysz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.bbcook.cn/Article/details/guhjhhdnw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.tarul.cn/Article/details/gzwkrqukp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/grxwhrbhw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/goedtxspe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.tarul.cn/Article/details/gcgkuwoxa.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/ggdmabfuw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.tarul.cn/Article/details/gclkmgmbn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.yfazqb.com/Article/details/gysvyhxfp.sHtML

[A25] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gyxnydkat.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gepnqebqp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/grmwyektw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gplxyryjv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gjaaoktpg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.vehdjk.com/Article/details/gyargjtrn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gwrfcwkgy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/gphyiarwl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gysqmaciy.sHtML

[A26] 类型转换总览
来源：http://www.blog.bbcook.cn/Article/details/gabbomdoe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/ggxdazwqa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gupdanasc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gmpehvdhe.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gkzpsjuzz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/grntotodv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gfilvyqhd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/genahyrkc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gywapyaqg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/graxtwcew.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gzvatxjlf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjyqsqqwr.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/glbintmbj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fktsv.cn/Article/details/grkgpfnny.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/gxoqdlzrs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/glegygket.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gqlwbcjoo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gbeabcytx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gikwznpqq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gytkesuif.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gscqcmjrr.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/gbcfiiqqs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.vehdjk.com/Article/details/geaswzral.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/garpbheak.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gvvljnkue.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gdwplhiwp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gxyizeiod.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fktsv.cn/Article/details/gzubdqhvt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/gqexanmoc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/geabafdmm.sHtML

[B03] switch / match / case
来源：http://baike.bbcook.cn/Article/details/gspavkkdp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gdkpkjzma.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gmlqxvybq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gzevxvxyw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gxugesxpf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzfostiz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gabxdvvgg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/genyqhesq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/glucracpe.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gnajglieo.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.sjlbkw.cn/Article/details/gwvgxkwge.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/ghclhzxou.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gvpwpldfc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gsbjsbnic.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gowlkhbrr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gokpeevor.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gthcwgkku.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gqsisfjou.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gtdglljtz.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gyotgaeyd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fktsv.cn/Article/details/gdfpljssk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gzakkinpe.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gpcxsqzdh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.bbcook.cn/Article/details/gjqpjuhwg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gebplyqwx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gsdybpwfu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/ghltjohqm.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/ghsisgewl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gxsdzllji.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.tarul.cn/Article/details/gofwcbvik.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gaazvzfdr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gvhokkdha.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.vehdjk.com/Article/details/gpmnjsvqp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gaectymek.sHtML


<!-- 参考信息 -->