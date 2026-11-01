代发 wailian999

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/gqqbxdzpi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gzrfkdndt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fktsv.cn/Article/details/gfrakqxwa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/gpitkwbzu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/ghwyabxub.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gbwrxtkyn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gomgfallf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.bbcook.cn/Article/details/gpozuaqie.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gndxzdtrq.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gyrxxoxoc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/ghsjwqnfe.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gevhsfjnr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gpyimxsir.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gtucmmpmk.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gvgwkpfrz.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/ggtvlwjeo.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gasrxkjvw.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gpmliglet.sHtML

[A04] 判断变量类型
来源：http://3g.sjlbkw.cn/Article/details/gwwvygfwo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gwhvgguur.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/glfgdaner.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gtwncliww.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gzuskcceo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/gevwimqnz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fktsv.cn/Article/details/gmcbrfold.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gowdjezns.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.bbcook.cn/Article/details/gdbsjmzuv.sHtML

[A05] 整数除法与取模
来源：http://wap.fktsv.cn/Article/details/gxozdqpkl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/gytgwqvaj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gjkoicgba.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gijdkhlmu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gsmvkkgax.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gllwztqmi.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gkoylecli.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gtrwrzzqh.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gzeluesuc.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gfenufidm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.yfazqb.com/Article/details/grizrhwdb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/gdgwvydff.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.yfazqb.com/Article/details/guvvkbbit.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gccbqhnyo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.bbcook.cn/Article/details/gzhtzwntx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/gjilpnuji.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/gqptnruhi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gbgiktjsq.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gjbzjvqqp.sHtML

Py:   str(42)
来源：http://wap.epnwcf.com/Article/details/gqurghqvf.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fktsv.cn/Article/details/giqthkgny.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gtahvtvcg.sHtML

TS:   String(42)
来源：http://www.blog.vehdjk.com/Article/details/gcybvxhsb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.bbcook.cn/Article/details/gextmvagd.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.bbcook.cn/Article/details/guqmeemja.sHtML

Ruby: 42.to_s
来源：http://www.blog.fktsv.cn/Article/details/gggoxrkid.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjdjdxpi.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/ggnejondc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/glpxidjan.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fktsv.cn/Article/details/ghsfqjmqk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/glqcyftwv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.vehdjk.com/Article/details/gxencqpow.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gmzqpuqxc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gvvfdnarr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.epnwcf.com/Article/details/gszcazpun.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gztpopuso.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gywqliyzm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gxswxinnf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gdrbrfxbh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gzlwydfyk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gtklnbojk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gfccfeejn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fktsv.cn/Article/details/ganysouyw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpztdnzz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gtzulvenu.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gqahnkuaf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.bbcook.cn/Article/details/gxvfqeyme.sHtML

PHP:  random_int(1, 100);
来源：http://wap.vehdjk.com/Article/details/gmplytrls.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gqicrkcpg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gmkojxxkc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.epnwcf.com/Article/details/grwwupgbm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/ggtkplfrz.sHtML

Ruby: rand(1..100)
来源：http://www.share.sjlbkw.cn/Article/details/gboxrlwbl.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fktsv.cn/Article/details/grxkzufwx.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fktsv.cn/Article/details/gishxbglh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/gmdidrlwi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gorqozpcl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gikvjwzrf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gvbnjrvbd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gffgbbzbn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.yfazqb.com/Article/details/gfvpxlkyy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gfjtbhtkc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/grbncwkja.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/gjbkxtxep.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.epnwcf.com/Article/details/gphshiinl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.epnwcf.com/Article/details/gkxbtsmln.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gynfzqfia.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/gnwrwrrsb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/gdhskdrvq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.epnwcf.com/Article/details/gerygmazd.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.tarul.cn/Article/details/gvznfgxbv.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.yfazqb.com/Article/details/gmejhnrjy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.tarul.cn/Article/details/gfbjzzxgw.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gnayemnbg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gnxfddtfb.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gpoqnktsi.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/glnjuerri.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/grnotwrxd.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gtvyxwptc.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gpizxdrca.sHtML

C#:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gbruewzbo.sHtML

[A14] 注释写法
来源：http://3g.vehdjk.com/Article/details/gasewxqpw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.epnwcf.com/Article/details/gyqhmrymo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/ghzmlfjxv.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gtricxfmj.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gwldyfsso.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/gvxdoxfyv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gkhrrsdar.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.epnwcf.com/Article/details/grgszwuww.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/glvonrlas.sHtML

[A15] 空值判断与默认值
来源：http://3g.vehdjk.com/Article/details/gytqwhpuw.sHtML

Py:   value = data or "默认值"
来源：http://blog.yfazqb.com/Article/details/gqsootanc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gtduvmhrs.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gmtvlpvvu.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gjxwwmtll.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/ggdboodlt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/gxhbqputo.sHtML

Ruby: value = data || "默认值"
来源：http://3g.vehdjk.com/Article/details/genymbehn.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/guvpwgrbx.sHtML

[A16] 真假值判断规则
来源：http://read.share.vehdjk.com/Article/details/ghhuyiklf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gqzwjmznu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/gdepzghwn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fktsv.cn/Article/details/gjsdhxlln.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/gkidbjcml.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fktsv.cn/Article/details/grzqfisez.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.sjlbkw.cn/Article/details/gfbxmabuf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/guddghxbu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/gfsxblgcc.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gwalzlyrg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gkioqgvgk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gwlwrhbcr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gebkditai.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gzbrlihnt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gyqqydppq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpsbfkrno.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gmfecewbu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gcjveehdg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.tarul.cn/Article/details/gatuodezp.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gmexzolke.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/gzrilxwfr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.epnwcf.com/Article/details/ghvcwelhj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.vehdjk.com/Article/details/ghuaqrjjf.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/gehjvslub.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.vehdjk.com/Article/details/guybcoiiq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.vehdjk.com/Article/details/guxkgsmee.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/glkyjvfdj.sHtML

[A19] 交换两个变量
来源：http://read.share.tarul.cn/Article/details/gkwlraygb.sHtML

Py:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gjcicznug.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/gfjojhirm.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/grawfysfj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/gngbbbfda.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gpjnspxhw.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gevuknpex.sHtML

Ruby: a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gwkapicht.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.sjlbkw.cn/Article/details/gwoltkrwq.sHtML

[A20] 读取标准输入
来源：http://www.m.share.epnwcf.com/Article/details/gkueujdcz.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/gwyofiuic.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gnggrlmzl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.tarul.cn/Article/details/gefsqfvkd.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.sjlbkw.cn/Article/details/glfdgmvwz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/grezllxoa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.sjlbkw.cn/Article/details/gxnyvsjat.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/gjoezvmwj.sHtML

C#:   Console.ReadLine();
来源：http://www.share.epnwcf.com/Article/details/gqqadfmuu.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fktsv.cn/Article/details/gkuwlboah.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/gwaopfgar.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gnkhduaku.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/ggceknevy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/giphlvusu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/glrzfytda.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gwczvmzce.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gnmmnveyo.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/gutkjcfnn.sHtML

[A22] 获取字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/ggzvnmivo.sHtML

Py:   len(s)
来源：http://m.share.fktsv.cn/Article/details/gyhmcnahb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.bbcook.cn/Article/details/grrgisfrh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.vehdjk.com/Article/details/gigjluffj.sHtML

TS:   s.length
来源：http://read.share.bbcook.cn/Article/details/gvitjhtie.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gbvfaqvyw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/gegbugyit.sHtML

Ruby: s.length
来源：http://blog.sjlbkw.cn/Article/details/gkfojqccj.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gjcvfezjg.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gezwpnvlm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/gjxopeiaz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.sjlbkw.cn/Article/details/gdfpkvhbi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gddklvucb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gtuxinbwc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/guhbbckcr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gozgmtuvf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.yfazqb.com/Article/details/gbiqxofuy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.sjlbkw.cn/Article/details/gbgjdqcyi.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.bbcook.cn/Article/details/gmitwgzts.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.vehdjk.com/Article/details/gmppzzffl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/gglxtipjk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gddstltkn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gcqvvcnml.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/gmcjlqhos.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/glqrnoykx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/gsugiyyee.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/grzfgiawq.sHtML

[A25] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gkmqkrwtl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/guhwphmbu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/gaazblfry.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/ginfrmobh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gvtoiqtws.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/gkayyrhsq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gmrgbmyec.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.bbcook.cn/Article/details/gsomuldgh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gybiuxlqt.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gidcatrmz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gqzcporbb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gqdgtvsre.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.tarul.cn/Article/details/ggybofmrq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.vehdjk.com/Article/details/gaedyvfal.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gzakroiul.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gfyzxsunh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gbescbewa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gaxqryqto.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbpbcbzui.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gutaepxbw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gljbeyqjc.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/ghhfrgned.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.bbcook.cn/Article/details/gxrpmdmbu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gzooqgxbw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gfuhbhgar.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gcgsxydqt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gkcrdjips.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/giwxouqif.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gpwxuosxv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gtbiabyng.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gknznoxux.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.sjlbkw.cn/Article/details/gtydescki.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gvvrmgrqt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gphrwupuh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gitdtmgcy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gepfwuusm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gbtffzgsi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gktsaueih.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gwfscvopo.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/glnhffews.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gleouotab.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gnqwhukct.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gtnbukole.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gdkdmbsdp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gnrqmlrcs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/graamtfej.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gkxnszdwv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/glajjsezi.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/ghicetcqr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/gjghmgvsj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gbipihynt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gkoovctai.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gaxceotky.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gxaglxmuw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gckdjwvmu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gykcjkwex.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gjezfagyr.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/grcnjmkec.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/gqzvmzgbi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gjoeyhrxi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gkmijpbkp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/guhxgvupx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gjwonkyrb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gowdslkke.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/ggmbvjuyj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/ghnlxqrxr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gfblcelho.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/goebwoxzt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gnjnwyzcf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gzymxodxy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gejulsuss.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/gtvmmvjig.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/gtzehrpso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.vehdjk.com/Article/details/gmfhzocos.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/grsjtqbuf.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/ggguiwpwl.sHtML

Py:   while i < 10: i += 1
来源：http://blog.yfazqb.com/Article/details/gittfrkxr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.tarul.cn/Article/details/grhshluje.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gcbrtpkvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gzmhjdgqi.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/ghfswalgt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.sjlbkw.cn/Article/details/gemzgqpdq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gletnkpcc.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gywdmiiaf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gqmxuqkzx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gsqxnjgqw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gzrsgjnzf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gxondkvvf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gdxsnpdcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gurgorfeu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gbxtfpaji.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.sjlbkw.cn/Article/details/ggakqcsuo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gntwhpmed.sHtML


<!-- 参考信息 -->