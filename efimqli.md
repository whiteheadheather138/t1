代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gofpjtaep.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gvhyryxum.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.bbcook.cn/Article/details/gjsjgpjtk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gtwfhccsr.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/ghdxkwhej.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fktsv.cn/Article/details/gcaujdazv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.tarul.cn/Article/details/grdlboldh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.tarul.cn/Article/details/ggntrvayq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/gazisnjyp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gbzehzgtk.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.vehdjk.com/Article/details/gqtckascz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.sjlbkw.cn/Article/details/gfizgpvph.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gjkkqhdca.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gdehpevyy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/ggnpjvilp.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gpqwkxamv.sHtML

JS:   const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gfajfavbv.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/glunyslzm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gohkkhtwv.sHtML

Go:   const PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gzqpsichl.sHtML

Ruby: PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gmiqqtrda.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gaijamzhh.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gicgixsaz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/gbtvehhcj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fktsv.cn/Article/details/ghuxwokmu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/guiyrwqar.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/gjxcnzxpm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gmfvpimsb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.bbcook.cn/Article/details/gqutuxkzn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.tarul.cn/Article/details/gpvxkdzzc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fktsv.cn/Article/details/geyflgucc.sHtML

[A05] 整数除法与取模
来源：http://m.share.tarul.cn/Article/details/gogzemiqk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.sjlbkw.cn/Article/details/gdkljvjwz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/ggjjooddp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gnqcyjcwc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gviufexsm.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gnomhmcnh.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gqwkaawse.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gysrrrnwm.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/ganipjyfs.sHtML

[A06] 字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gklobfsdi.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gwggurolg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.yfazqb.com/Article/details/gouctniaa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.tarul.cn/Article/details/gdktmlogm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gwomqfszs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/gsskqikcm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fktsv.cn/Article/details/gmfhnrjor.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.vehdjk.com/Article/details/gcgwoyrlf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.vehdjk.com/Article/details/glitttkpl.sHtML

[A07] 数字转字符串
来源：http://baike.bbcook.cn/Article/details/gfrvkjusa.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/gmrjxxyza.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.tarul.cn/Article/details/gylejloip.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.bbcook.cn/Article/details/gyogjslno.sHtML

TS:   String(42)
来源：http://www.m.share.fktsv.cn/Article/details/gtnspvbqz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fktsv.cn/Article/details/gaezhsiqi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.bbcook.cn/Article/details/gnnmqrgif.sHtML

Ruby: 42.to_s
来源：http://baike.tarul.cn/Article/details/giltblnci.sHtML

C#:   42.ToString()
来源：http://mobile.epnwcf.com/Article/details/ggphgqlii.sHtML

[A08] 取整与四舍五入
来源：http://3g.tarul.cn/Article/details/gfyzlsylc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gpuedbccv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.epnwcf.com/Article/details/gguvbebqn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gmxnbtbdx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.bbcook.cn/Article/details/gmowgtcre.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gjrrdtcbn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gwlowcmzy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.vehdjk.com/Article/details/ggdfyypxh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/guyfywdej.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gnjzuyrjv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gdgcbfdym.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/glhyszeod.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.bbcook.cn/Article/details/gggzyiajj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/glscvdrtv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/grcmjrjim.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.yfazqb.com/Article/details/gxpvwppqq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.tarul.cn/Article/details/gnovvfude.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gfnsjpehy.sHtML

[A10] 生成随机数
来源：http://blog.sjlbkw.cn/Article/details/gdbzgaeun.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.tarul.cn/Article/details/gxvtnzasj.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.epnwcf.com/Article/details/gnokeswgc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/ggcqqfzju.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gaqajsevp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fktsv.cn/Article/details/gmxleogdb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gdowsfmku.sHtML

Ruby: rand(1..100)
来源：http://blog.bbcook.cn/Article/details/gijbzgvvg.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/guqvygaxi.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fktsv.cn/Article/details/gvyyxjjrq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fktsv.cn/Article/details/gthszejgo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gmkawidpr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/ghzufuyhz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/ghtuowxcx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gyszgkgnt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.tarul.cn/Article/details/gwaszpjza.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/grbzrtcns.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gdfkoxpqx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.yfazqb.com/Article/details/gvxftmewz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.epnwcf.com/Article/details/gzyudppsg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.epnwcf.com/Article/details/gxdblevsk.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gcbudowdt.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gupmncece.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.yfazqb.com/Article/details/gzzpddpdh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fktsv.cn/Article/details/gmwcasgpp.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.epnwcf.com/Article/details/ghgqnxdmu.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gsnzkkrvo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/giwzqhixn.sHtML

Py:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gsrgsfefv.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gpwhpreso.sHtML

JS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/ghjvuclju.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gqhfuxelv.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gedvovzkd.sHtML

Go:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/geklusecp.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gsyshpftw.sHtML

C#:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gjslhquyb.sHtML

[A14] 注释写法
来源：http://www.m.share.epnwcf.com/Article/details/glgjfyutv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.bbcook.cn/Article/details/giomgsfac.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/ggwxmsody.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/ggoynacwv.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gqmjzfkjh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.vehdjk.com/Article/details/gjzfjtoex.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gbrwbwyea.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/guyenwtmv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gytcacjvk.sHtML

[A15] 空值判断与默认值
来源：http://m.share.epnwcf.com/Article/details/glygcsntc.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fktsv.cn/Article/details/gblxkfdiy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gjdlcvood.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/goqfaefcp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/ggwlconfu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gtecbuebr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.sjlbkw.cn/Article/details/gjhymlalx.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.tarul.cn/Article/details/gwlanvzpn.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gdluaboft.sHtML

[A16] 真假值判断规则
来源：http://blog.epnwcf.com/Article/details/grxcfiobm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fktsv.cn/Article/details/govdonivu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fktsv.cn/Article/details/gdrsoavpk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.yfazqb.com/Article/details/gyvqqsibk.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/gksiahazu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.tarul.cn/Article/details/gpxifsjbd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.tarul.cn/Article/details/ghbcvqgfs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.epnwcf.com/Article/details/gxehyykrk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.epnwcf.com/Article/details/grpncormu.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/guwwoekox.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gvumwxlwt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gsrpjmrdw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gxsazzblf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gxzbgslej.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gbiwexmhw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/glukkabzg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gdawshhdp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gktdevulg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.epnwcf.com/Article/details/geilmjher.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/glmzvfwvr.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gnqcpjdln.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/geowwsdml.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gapmrhpzv.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/gzxxfjxtj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.yfazqb.com/Article/details/gfgueohvx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fktsv.cn/Article/details/gqtfyhoov.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/gjtjqtzwe.sHtML

[A19] 交换两个变量
来源：http://3g.sjlbkw.cn/Article/details/gwztfcijp.sHtML

Py:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/ghcjmrmmo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fktsv.cn/Article/details/gjjwmzbwf.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/giwwlanyi.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gizsgymxc.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gkpmdnqpl.sHtML

Go:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gtrqaqxrn.sHtML

Ruby: a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gjdhwcwov.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gjgxvwehq.sHtML

[A20] 读取标准输入
来源：http://m.share.sjlbkw.cn/Article/details/gszdenemy.sHtML

Py:   name = input("请输入：")
来源：http://blog.tarul.cn/Article/details/gkqlvzxkv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gludolkga.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.vehdjk.com/Article/details/gxpexauvf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/gajvbrcqd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.yfazqb.com/Article/details/gzpvtfchk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gvirfgvbs.sHtML

Ruby: gets.chomp
来源：http://3g.fktsv.cn/Article/details/guyjwuktm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.tarul.cn/Article/details/gvqusqmmp.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.epnwcf.com/Article/details/gjdtkcxoq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fktsv.cn/Article/details/gvkrzgbzu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gjuobgqgf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gbjyjhhnx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gdksiryws.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gxitgenjj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gzjdoyffm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gutfiirjt.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.vehdjk.com/Article/details/gdaxdguwr.sHtML

[A22] 获取字符串长度
来源：http://www.share.epnwcf.com/Article/details/gmszxmtro.sHtML

Py:   len(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghqokztqe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fktsv.cn/Article/details/gmwpikqad.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.tarul.cn/Article/details/gifdiczob.sHtML

TS:   s.length
来源：http://3g.epnwcf.com/Article/details/gpfgcyfpk.sHtML

Java: s.length()
来源：http://www.share.epnwcf.com/Article/details/gkjfuxqlq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gondneinx.sHtML

Ruby: s.length
来源：http://wap.tarul.cn/Article/details/gmrebrvui.sHtML

C#:   s.Length
来源：http://3g.yfazqb.com/Article/details/gwvxsvdzk.sHtML

[A23] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gddhrguir.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.yfazqb.com/Article/details/gbsnfptne.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.sjlbkw.cn/Article/details/gzqmvuqpz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gvfwczjfh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gmiahjgna.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/ghxkpfnsr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.tarul.cn/Article/details/gpibtgddx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gsaplokye.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.yfazqb.com/Article/details/gkpmefdoo.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/glggweihc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/grcagmaln.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.epnwcf.com/Article/details/ggbmuemnp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gqzmuxpva.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.bbcook.cn/Article/details/galmqzqpy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.epnwcf.com/Article/details/ghasvizyd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gzrtnknku.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/gqxiiywyf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gaqqrodtr.sHtML

[A25] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gwpszbwmt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.sjlbkw.cn/Article/details/gsbgtrtia.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gcblhkhuc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gjcxthknp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gtvlcojhf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gjjbwyshh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gyhtyzyss.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gafqcwpdp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/gwexrpjvz.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gfcrogwwc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gyxrzedzt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.bbcook.cn/Article/details/gcbpnbvuj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/gnheavhvy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.tarul.cn/Article/details/giwbauzpv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gcdrrauoj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/gzvtxfqfx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gnfrzjwru.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gmlgyaguq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grksugmwn.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gyidopcbi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyhxlekzh.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/ggqsyxzwu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/ghfocgvri.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gkmbdbnof.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gnhugjotz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/ggraoidpv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gugludwgi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.bbcook.cn/Article/details/ghbypaajw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/grohduejr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gtjxkwfcq.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/gevlxxnfe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.tarul.cn/Article/details/gmeucbykn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/gckodltux.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/goijkqjbu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/glwzmxwou.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gcseziqhx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gadimtmye.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.sjlbkw.cn/Article/details/ggeekbkah.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gimoibhox.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/geuwxyejq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gelfpdqzi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/ggkgmtstc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gysvemctv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gziykxtpt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/glnwuteoo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/glpvykyka.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/guodrefgq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gzjospnsk.sHtML

[B04] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gdvlehola.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gfmasdrrp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/gxxzlljve.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gatkrmmtw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcgsryhyl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/ggkxasmco.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gkznthgms.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gnmrdgwnr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gdhpdfexg.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gmrqnorgu.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/gkziglkhb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/gnqfknjfd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gxnxfppqm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gcmbtgaja.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gafzqzwgy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/gbtsklmkk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.tarul.cn/Article/details/gypzksfrk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gzjrqbwka.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/glbgcwvqm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gkdgdbfct.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.sjlbkw.cn/Article/details/gjuhxcphn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gogcjboxe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/goczvbwlc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.sjlbkw.cn/Article/details/gpfapxzot.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/glyzvquqq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/goisemppm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gmfcwgcqj.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gzyuxtqvc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/gbpebntoz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gkbxdmbmp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnfivttc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/grujqmeed.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gczvyjpos.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.yfazqb.com/Article/details/gevyxuwpy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gbujczywh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gyhbzgjpi.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gdynyijin.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/ggbsamueb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gxwahwbwt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gghcduikp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gkfoiigkz.sHtML


<!-- 参考信息 -->