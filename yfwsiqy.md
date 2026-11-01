代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gqlriuoee.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gkqkaaxjn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gbxitqjam.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gxuisslsp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grpdtyyin.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/gbwotwsrb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqrvebamu.sHtML

[A01] Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcbxtddai.sHtML

Py:   print("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gtbollmyf.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gjgmdimau.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gkqqvqzym.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.tarul.cn/Article/details/gixmxrvuf.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gpdipnfoz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gqrswkluk.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fktsv.cn/Article/details/gvrvftrmr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gvjafzfam.sHtML

[A02] 变量声明与赋值
来源：http://mobile.vehdjk.com/Article/details/gghgirpiw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.yfazqb.com/Article/details/gmvyzinsb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gwwhtaqug.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gfxhdpanb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.epnwcf.com/Article/details/gwgporvzh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gbwqjivgd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fktsv.cn/Article/details/gjrxylbcf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.bbcook.cn/Article/details/gityuckhc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/geecgqkpk.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/ghilzptwt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.vehdjk.com/Article/details/ggghhdzjk.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gcdkqatur.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/godnlypqu.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gtzpbdish.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/glduipeye.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gisryhqru.sHtML

Ruby: PI = 3.14159
来源：http://read.share.sjlbkw.cn/Article/details/gdlglepoy.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gflznihbl.sHtML

[A04] 判断变量类型
来源：http://mobile.bbcook.cn/Article/details/gsjsthrou.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.epnwcf.com/Article/details/gjcnnuqnl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.tarul.cn/Article/details/gcqtdywwc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gumwcbwzc.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.vehdjk.com/Article/details/gvmfcpagn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gkxyercyp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fktsv.cn/Article/details/gsrplmkqv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.bbcook.cn/Article/details/gjmjfazgw.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.tarul.cn/Article/details/gyrvkziey.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/gxeclcwve.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fktsv.cn/Article/details/goenamjwd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/ghhvjsvbf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gjfabpfce.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gzgraqwdq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gjrcxsoyo.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gamqmaeel.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gsomlwpmw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gjyzqndvx.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gztizburc.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/gewuwawdn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.yfazqb.com/Article/details/gljhcpezy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.bbcook.cn/Article/details/govzjkkss.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/gawfpohjz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.tarul.cn/Article/details/gckdkhvlh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.epnwcf.com/Article/details/gaoutiajk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/gznztfbcz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gzmfngjqx.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/guoyzimlu.sHtML

Py:   str(42)
来源：http://blog.tarul.cn/Article/details/gnzvupzhv.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.bbcook.cn/Article/details/gjivyiuef.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvyuzcya.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gsvisejhb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gyfbxyttc.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fktsv.cn/Article/details/ggmxdecno.sHtML

Ruby: 42.to_s
来源：http://www.blog.epnwcf.com/Article/details/gggqdhwwt.sHtML

C#:   42.ToString()
来源：http://m.share.sjlbkw.cn/Article/details/goukrnsrd.sHtML

[A08] 取整与四舍五入
来源：http://www.share.bbcook.cn/Article/details/gkdpdflvu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gewnlejxh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.epnwcf.com/Article/details/gmxxjfgwp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gwyrbbvmr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.yfazqb.com/Article/details/gidrmdnlu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gclbedkpm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gkzooeeuo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/gzijtfjiu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gmuumpvzv.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.epnwcf.com/Article/details/gqqlxpknv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gpbmvxman.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.tarul.cn/Article/details/ggznyfnce.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.bbcook.cn/Article/details/ghbmfgboz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gvgpktrcd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gpedialks.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fktsv.cn/Article/details/gjrfyxexg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.sjlbkw.cn/Article/details/giezadmyu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gigdfzrzy.sHtML

[A10] 生成随机数
来源：http://read.share.epnwcf.com/Article/details/gatbyaukr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.vehdjk.com/Article/details/gbyejoyiv.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.bbcook.cn/Article/details/gbgzgefqd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gqkgnsoef.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gyylblqwg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gepunedie.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gtpzycdpj.sHtML

Ruby: rand(1..100)
来源：http://blog.vehdjk.com/Article/details/ggcbornbe.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.bbcook.cn/Article/details/gbybqjkoz.sHtML

[A11] 条件表达式（三元）
来源：http://blog.bbcook.cn/Article/details/gfhmxtsae.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.sjlbkw.cn/Article/details/gasaqtyhz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/guarewdfe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gyvuucdxq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gxvwremdc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gyxlegorc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.vehdjk.com/Article/details/gsnlrolxb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/grcrmbbjh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gdfnbgcui.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.yfazqb.com/Article/details/gajzdrcev.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.epnwcf.com/Article/details/gtbfrgria.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/gzilzxfqd.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gmyukhrzi.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fktsv.cn/Article/details/gbbvgdyvz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/ghvhlmolg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gkybmfild.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fktsv.cn/Article/details/gyqffgihx.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.sjlbkw.cn/Article/details/gmldtqinu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gadcbdaly.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gitcgfhqg.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gvkylgsof.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gmaybzwmw.sHtML

TS:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gpulvtphz.sHtML

Java: "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gkfbwvotb.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/govikbtea.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gidtjphxi.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gnpzmhfcf.sHtML

[A14] 注释写法
来源：http://3g.tarul.cn/Article/details/gokqjslkw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.tarul.cn/Article/details/guoyuhzdb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gwgkpivgo.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gpmzzttig.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gvowjquwb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.bbcook.cn/Article/details/gynmbfwly.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/giczdcqau.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.bbcook.cn/Article/details/gxyxchtvs.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gzlwnogbt.sHtML

[A15] 空值判断与默认值
来源：http://3g.epnwcf.com/Article/details/gkjytrkip.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gdkpdcacl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gmzoqtjpc.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gseubpfow.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gposlqzcl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.yfazqb.com/Article/details/gramnfnvd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fktsv.cn/Article/details/grrbkyrxq.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.sjlbkw.cn/Article/details/gjlbblnhj.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gjlerfmqu.sHtML

[A16] 真假值判断规则
来源：http://www.share.epnwcf.com/Article/details/gzeegqklj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.bbcook.cn/Article/details/gyeezsabh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.vehdjk.com/Article/details/ggvnrmrlf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gjrelbyyq.sHtML

TS:   if (!x) {}
来源：http://www.share.tarul.cn/Article/details/genoonhcs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.bbcook.cn/Article/details/gtqeocyiz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gkylsubli.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.yfazqb.com/Article/details/ganwxcmuc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.tarul.cn/Article/details/gosnazkxs.sHtML

[A17] 位运算
来源：http://baike.epnwcf.com/Article/details/gmcbukghe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/ghbwiiiur.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/guikbkive.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gatwirbti.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gbpgvxtnw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gcciziiic.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gjsssikot.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpkpysech.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/giauciujr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.vehdjk.com/Article/details/gtoglilfr.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/grrysnthu.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/glpfmuygx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.epnwcf.com/Article/details/gwkhxctlw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gibvewzno.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/gysfjuobi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.vehdjk.com/Article/details/glsdqdwds.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.epnwcf.com/Article/details/gxlrhtapq.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.bbcook.cn/Article/details/gxsayjpho.sHtML

[A19] 交换两个变量
来源：http://www.share.epnwcf.com/Article/details/gjwomilfp.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gkflqgioi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/gpmyxvkut.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gupvvyvjp.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.epnwcf.com/Article/details/gjhirumty.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gillolmob.sHtML

Go:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gbvojeaud.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gtsgzpoys.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.epnwcf.com/Article/details/gktujqxtz.sHtML

[A20] 读取标准输入
来源：http://mobile.fktsv.cn/Article/details/gmvjlbpoz.sHtML

Py:   name = input("请输入：")
来源：http://blog.epnwcf.com/Article/details/gemlwyufo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.vehdjk.com/Article/details/gqfybjnqz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.epnwcf.com/Article/details/gmprfgwgd.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fktsv.cn/Article/details/gfbxegtrx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/grkxsvixe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.sjlbkw.cn/Article/details/gqosqiore.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gyotljuha.sHtML

C#:   Console.ReadLine();
来源：http://mobile.sjlbkw.cn/Article/details/gnrpznaeo.sHtML

[A21] 保留指定小数位输出
来源：http://wap.sjlbkw.cn/Article/details/ghjjaiazs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.yfazqb.com/Article/details/gfovqdwdv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gxgpkgmfn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkqbzjzk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gdkvkghmg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gjyehdrqe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gndkgxxjx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxhtvfdi.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.yfazqb.com/Article/details/goeqkimmb.sHtML

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/gdgpgsezm.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/ghiaymfbj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.tarul.cn/Article/details/gsjmlnodf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.epnwcf.com/Article/details/gmhxznwop.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/gyhdwrbfi.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/ghiyhylrt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fktsv.cn/Article/details/gqnahkcmr.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/gbexiluwz.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/ggtuqwnhb.sHtML

[A23] 大小写转换
来源：http://www.share.tarul.cn/Article/details/ghvlocyqd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/gxmudscci.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gqhotnizu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gawlavtpy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gmcggctni.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/ggqupqmrr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.vehdjk.com/Article/details/gmladihml.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/gzpgzyipv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/gvsctcvpf.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/goapnjbny.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhmfvrgg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gtjdoxuhw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/glgtvtqqw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gssrktnpj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/gtewmybuk.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.tarul.cn/Article/details/ggznblgbq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/gcghtxqhk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gceeyppbi.sHtML

[A25] 字符串比较
来源：http://wap.epnwcf.com/Article/details/ggtwtnecn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.bbcook.cn/Article/details/gviftmkqo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fktsv.cn/Article/details/gcpedyatr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/ggkrmqomc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gbsyylxpq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/guwvojhpv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfaepdkk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.sjlbkw.cn/Article/details/ggzpikipb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/ggksrrmkl.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/guerbtkyu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fktsv.cn/Article/details/gzbvxchqh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/goljhrtmd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/ghinvdwgp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.epnwcf.com/Article/details/giunitjrb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gpxkkrcty.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gwttbugap.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gfndipior.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gxmjtmsbq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grzhdfuuq.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/glslbdvzi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyocloyjw.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gxqbkixyl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.sjlbkw.cn/Article/details/gcpvsenit.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gkvroyfoj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gylvphgwa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/ggdntgqao.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gznjfsvhc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.epnwcf.com/Article/details/gpvyuvbaf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gcouyequu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gzrsaabav.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvjylcrw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gdqpkcbmr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.tarul.cn/Article/details/gthceqbwg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gmjzcbtpc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gxjftnwnm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gudnpndig.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.epnwcf.com/Article/details/getvcmfly.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.bbcook.cn/Article/details/gismmkakw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gqwatapjn.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gjycualhh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/goxlzcekl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gnwxjxhfe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gkhxztvqy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gsorubhpd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/geoohnjmr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gxtlhbklu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/geyzdlefx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/gmmpfqloe.sHtML

[B04] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gvwjeyybx.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gawejayjb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqzvmmbu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gfklynwff.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/gambzviis.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/grxjvyfms.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.tarul.cn/Article/details/grrgemnsw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.epnwcf.com/Article/details/ghmpsnfta.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/govckthsx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gziizdlti.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gnvewahex.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gnbwojhbh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/grokqwtgl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gosehaosj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gwvctarrs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.tarul.cn/Article/details/gowsmbykv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.yfazqb.com/Article/details/gcxxqugql.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.yfazqb.com/Article/details/gwxvtonzv.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.epnwcf.com/Article/details/gkjxdhqws.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gpsigghex.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gaznjlkfw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gccsrzmns.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gzbozyppi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/gmpchrgtn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.tarul.cn/Article/details/gnbygaier.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gnwvtlhoc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/gahkfoktf.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gxcklxjwq.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/grekjyfbk.sHtML


<!-- 参考信息 -->