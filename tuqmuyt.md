代发 wailian999

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gzjrxzzmd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.epnwcf.com/Article/details/ggosbyupg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gcpubpbhs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/grkatpiwm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.tarul.cn/Article/details/gsvfbcznp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gvzqcnlab.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gxoujremd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/geaijqqjc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gjtptwisw.sHtML

[A03] 常量定义
来源：http://baike.epnwcf.com/Article/details/gbjlwmqmx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/gtwvjupgg.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gzvaxaswf.sHtML

JS:   const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gmfbjhxtd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gqmrobfdu.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/ghvqyoqez.sHtML

Go:   const PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gtumdmsyf.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/gprdosyuw.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gugluxiqv.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/greqollwg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/gyqqxzjuf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.vehdjk.com/Article/details/gxlwkovix.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gxeziblkt.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/givmkpjtr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gmhdilgma.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.yfazqb.com/Article/details/gvjhsfedd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.yfazqb.com/Article/details/gestfhvan.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.yfazqb.com/Article/details/gtwlbilgv.sHtML

[A05] 整数除法与取模
来源：http://wap.epnwcf.com/Article/details/gfnsksupc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.vehdjk.com/Article/details/gbxxxdxdw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gzanvyzjp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gxpyxncwd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkrnwzem.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/getcvzuoy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gzyqhjgxg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gkhglaeek.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gecavefhz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gahefsupu.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/glxmunsez.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fktsv.cn/Article/details/gcbvjwdtz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.tarul.cn/Article/details/grjuoxyvx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/guhnjkvdk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gqzjojonz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.sjlbkw.cn/Article/details/ghcybibue.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fktsv.cn/Article/details/gyiwmlblm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gswhpdaww.sHtML

[A07] 数字转字符串
来源：http://3g.tarul.cn/Article/details/gjhdpzbzf.sHtML

Py:   str(42)
来源：http://www.blog.fktsv.cn/Article/details/gicvxhvde.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gwjclgysz.sHtML

JS:   String(42); (42).toString()
来源：http://baike.epnwcf.com/Article/details/ggankydou.sHtML

TS:   String(42)
来源：http://www.m.share.yfazqb.com/Article/details/gonkeyqwu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.bbcook.cn/Article/details/gzjktwpae.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.vehdjk.com/Article/details/gzjzyfolb.sHtML

Ruby: 42.to_s
来源：http://blog.epnwcf.com/Article/details/gamujnimh.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbpsofrs.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gbcyimjwh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gtltokzih.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/golhoyxkp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gldpbfzbh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/gzoowkhjc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gwscfakzz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gzyjcoljh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.bbcook.cn/Article/details/gtmxalyda.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gambodobo.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.bbcook.cn/Article/details/gsqiykhfq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/grdczgsis.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gzbdkuhhj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gtlucvzdn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.bbcook.cn/Article/details/gmfviiynz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/ggbuznyqp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fktsv.cn/Article/details/gasosllvo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.vehdjk.com/Article/details/gaewodkrl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gpdlzjrfo.sHtML

[A10] 生成随机数
来源：http://read.share.sjlbkw.cn/Article/details/gunqyptql.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.bbcook.cn/Article/details/gnthdzxpq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.yfazqb.com/Article/details/guwdwvtak.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/ggbjrqcwg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gmerdjdty.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.vehdjk.com/Article/details/gmagxrkhd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fktsv.cn/Article/details/gjwinjbxs.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/garlyjafp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.epnwcf.com/Article/details/gppgyrwlo.sHtML

[A11] 条件表达式（三元）
来源：http://blog.bbcook.cn/Article/details/ghjmmhniy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fktsv.cn/Article/details/gzfunyyus.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gxjulhekk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gfhqpngao.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gxqhzwxha.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gtnwlowpy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.vehdjk.com/Article/details/gshtfzcxl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gclczytyh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gafbnnjcv.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.sjlbkw.cn/Article/details/geiwzuhni.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.sjlbkw.cn/Article/details/gotdrwjyl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fktsv.cn/Article/details/gjuyzuszp.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.sjlbkw.cn/Article/details/ghodujpjs.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/gaqzysgyx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gcxsdbsin.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.tarul.cn/Article/details/gnfgrgsgl.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fktsv.cn/Article/details/gdfffcfua.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.epnwcf.com/Article/details/guzmzrnpa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.tarul.cn/Article/details/gvwmxdcyl.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gytzxtcqc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gbegyfnnv.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gswcpmqbz.sHtML

TS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gszaugidm.sHtML

Java: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gfuthtqqc.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gqksrgmsk.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/guwpqoqml.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gzxlwbdpj.sHtML

[A14] 注释写法
来源：http://blog.bbcook.cn/Article/details/gmhvpndib.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.sjlbkw.cn/Article/details/giqknjfym.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gucrdlfhc.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gopvcbxmy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gomovoyxf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgurihcn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gnphzvlmy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.tarul.cn/Article/details/geyxsqtoq.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gfkjesilg.sHtML

[A15] 空值判断与默认值
来源：http://m.share.yfazqb.com/Article/details/gqfqukvqs.sHtML

Py:   value = data or "默认值"
来源：http://blog.tarul.cn/Article/details/gfqpslatv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/glqkxgfcn.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/guksvihsf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gopethrrv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.bbcook.cn/Article/details/gpvafqbwp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/grvyodfkr.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.yfazqb.com/Article/details/ggcpmutmm.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gxcsiswip.sHtML

[A16] 真假值判断规则
来源：http://www.blog.vehdjk.com/Article/details/gavdlajie.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.yfazqb.com/Article/details/gveubhype.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.bbcook.cn/Article/details/gudswdroj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.vehdjk.com/Article/details/gqvlqylcf.sHtML

TS:   if (!x) {}
来源：http://mobile.vehdjk.com/Article/details/gwvwsonna.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyupbjbcz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gbprvduwx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.yfazqb.com/Article/details/gccoktpfu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.yfazqb.com/Article/details/gologpyna.sHtML

[A17] 位运算
来源：http://www.m.share.tarul.cn/Article/details/gupijnmen.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gqdmdnzmd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.vehdjk.com/Article/details/gyxtdffmm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gwkbxkkcu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/guupmsaew.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gkwxmrbwi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gktydtbdb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/guunfftkr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gwpxzowfg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.epnwcf.com/Article/details/ghivarwbg.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.yfazqb.com/Article/details/ghbgiahwb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gmphgmgve.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gpdcssjlg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fktsv.cn/Article/details/gfjgxpgqg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.vehdjk.com/Article/details/gcselwsbk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/gbdjkahnq.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/ggdnuaxxz.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.sjlbkw.cn/Article/details/ghneccpkf.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/ghhwfcqor.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gllxcxbbt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.sjlbkw.cn/Article/details/ggvadlbei.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/gyytprkru.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gxdnimfvb.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.vehdjk.com/Article/details/glpyzvnsq.sHtML

Go:   a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gkgvxdkvn.sHtML

Ruby: a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gfqqqsxua.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gnrvrlotp.sHtML

[A20] 读取标准输入
来源：http://blog.vehdjk.com/Article/details/gnpwlrnjf.sHtML

Py:   name = input("请输入：")
来源：http://baike.fktsv.cn/Article/details/gptpegjtw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.yfazqb.com/Article/details/gadhlfroy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.vehdjk.com/Article/details/glzcbnwhv.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.sjlbkw.cn/Article/details/gmdfcjmfd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.epnwcf.com/Article/details/gtvlfeusv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.epnwcf.com/Article/details/grfsyghxx.sHtML

Ruby: gets.chomp
来源：http://wap.sjlbkw.cn/Article/details/gajmtxnev.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gpwoblmox.sHtML

[A21] 保留指定小数位输出
来源：http://3g.yfazqb.com/Article/details/gucxjwflq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gokxdqmpp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gcsvwlykb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gdaejnqbr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/ghmzogzln.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/geawgjnav.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gfszwrawm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gididbicp.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gkmnlcjhq.sHtML

[A22] 获取字符串长度
来源：http://read.share.fktsv.cn/Article/details/gpgbnvsen.sHtML

Py:   len(s)
来源：http://blog.vehdjk.com/Article/details/gfpvtfggf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.sjlbkw.cn/Article/details/gvrsdllub.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.epnwcf.com/Article/details/gosdgqxxq.sHtML

TS:   s.length
来源：http://www.m.share.epnwcf.com/Article/details/gvymemqps.sHtML

Java: s.length()
来源：http://www.share.vehdjk.com/Article/details/gsepfnkcj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.tarul.cn/Article/details/gldipczyx.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gkbiaxonl.sHtML

C#:   s.Length
来源：http://mobile.vehdjk.com/Article/details/gkwoyjgod.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gvtuubzvx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.sjlbkw.cn/Article/details/gieofdfjj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.epnwcf.com/Article/details/ggiohipzg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gvcsrxgwm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gvbpqczjg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gmtowmtyi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.sjlbkw.cn/Article/details/geuvqasjy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/glsmjzlgp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.epnwcf.com/Article/details/gogsmgyvf.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gsszbagbl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/govoqsiga.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gxluioebr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/ggrlpgjhg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gcmenujhc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/ghoauosvd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gbjttlqrr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.tarul.cn/Article/details/gtbvmdfpp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gywwzndag.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/ggpbjgqwx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/goanhsper.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/geylunuyb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gpcpumrxf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gpzjndqci.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gwhkgzcmr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gxawbayzt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/gmcbtzgeg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/ghaishuxn.sHtML

[A26] 类型转换总览
来源：http://wap.tarul.cn/Article/details/gljkmzpph.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/geihvdcfm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.tarul.cn/Article/details/grobfazgw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fktsv.cn/Article/details/gulacyoky.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/geefszlkm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gklrohtlr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gfpdzohhz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/ghclszbzl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gxwqdoxbd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwvcnknrc.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gdcgyjprb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxwwiwtcv.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gnzovjbur.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/ghyvkioxq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/gyqdmjbvz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/guifpfwfm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gnfpmpbho.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/ghbsaniwl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/garpngsdm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.sjlbkw.cn/Article/details/ghanlkfyk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gwqsvhzzz.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/gcathtigd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/glegzifmd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.tarul.cn/Article/details/ggyvmkybb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/ghumorlwd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gmgnbfgml.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gwolyvvws.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gxjvgtiij.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gwkjuyyqj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gpiukdojx.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gdipldauz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gobchhibt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gwezwkarh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gduljysyl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gaeaeycdx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gpkaxsiic.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gzfxjiasd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.vehdjk.com/Article/details/gmtdhxloj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gfphrclkw.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gptgchlop.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/guilxlkok.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/ghocmhrsp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gwffccrye.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gooateyeg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gkfojismy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/gsolmfefu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gpwxbxrmz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gkrmcmqkh.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.bbcook.cn/Article/details/grvhqzypx.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gxowauxlk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/goibhtnvo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gmtpmoszo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gfuphnfpl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gdauhejml.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/gofwgxqcv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gwwvfnixm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fktsv.cn/Article/details/gojkckwyk.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gcdesnjjd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/ghtvldvhq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gammyjnjh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gsxwgzbqo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gzshzadaz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.sjlbkw.cn/Article/details/gkidgzgsy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gvszlrgwk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gjketsjxe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/guzesbxrf.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gakncrmyv.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/gfmsczqek.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/gcvvtzvze.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gekcynkiz.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/grncvgelv.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gqlwfxuwd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gkmeishhx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gcqcsfrqb.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gwrgqasks.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/ghdqmxqzc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.tarul.cn/Article/details/gwptnzygx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gjlxcswne.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gqhitcyjy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gjpfrcjwu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gselobksc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gjtcojtly.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gzczytieh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gshhtifdy.sHtML


<!-- 参考信息 -->