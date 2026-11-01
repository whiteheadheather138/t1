代发 wailian999

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gvscikklm.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/ghcpamvvu.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gwonelmkn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.epnwcf.com/Article/details/gdxybbtbl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.bbcook.cn/Article/details/guratgmad.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gispxdlgw.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gbkjwxhod.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.yfazqb.com/Article/details/gzdzcwoad.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gvyiccffa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.yfazqb.com/Article/details/grmjlilaw.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gjcdttchr.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/grvgcdzhi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.sjlbkw.cn/Article/details/gbqanelvk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gehotatug.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gldlhapwi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gjvbyciwe.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/grducfmbx.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/ghmwnnngp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gskltqrvy.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gvtflbyzs.sHtML

[A06] 字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gwnxsbmxn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gdwrnanwk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.sjlbkw.cn/Article/details/glnkevmnq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/gxuzzfcov.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gmceqswmn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.vehdjk.com/Article/details/gjxedhqwd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.yfazqb.com/Article/details/gfaotvtnw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gfyptynpc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gqhsalihd.sHtML

[A07] 数字转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gcvdxsbki.sHtML

Py:   str(42)
来源：http://m.share.epnwcf.com/Article/details/gsceumzpe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gzvbqfnog.sHtML

JS:   String(42); (42).toString()
来源：http://blog.bbcook.cn/Article/details/gunfcfuwp.sHtML

TS:   String(42)
来源：http://www.share.vehdjk.com/Article/details/gplocpqaz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.epnwcf.com/Article/details/gftcfcmlj.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.vehdjk.com/Article/details/glegjhgzd.sHtML

Ruby: 42.to_s
来源：http://wap.yfazqb.com/Article/details/ggbezuswp.sHtML

C#:   42.ToString()
来源：http://baike.tarul.cn/Article/details/gffyxkdqj.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fktsv.cn/Article/details/glrfiujnw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/givkzdyfm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fktsv.cn/Article/details/gwnoglogc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/ggwtdaooy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.epnwcf.com/Article/details/gshqfdlwc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gtopieyhr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.tarul.cn/Article/details/giqoobqhn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.tarul.cn/Article/details/gfdwcwfdi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/ghzvtvvdz.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.vehdjk.com/Article/details/gtdgqnhzm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gwbewpysq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/ggzigepjo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gbjvgerpq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gvplezkld.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gprullbzt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.yfazqb.com/Article/details/ggerjtjlx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.bbcook.cn/Article/details/geqmyhwhs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gyaxyestc.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/gcavjnjjn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.vehdjk.com/Article/details/gysrklryu.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gkeumlzvu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.tarul.cn/Article/details/girnwjrqr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/gdfvpgetu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.tarul.cn/Article/details/gnauointe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.yfazqb.com/Article/details/golapafyr.sHtML

Ruby: rand(1..100)
来源：http://m.share.sjlbkw.cn/Article/details/gswqaqrnx.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fktsv.cn/Article/details/gvinkpgyn.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.vehdjk.com/Article/details/gydeawxob.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.tarul.cn/Article/details/gxegddulr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/ggglgsnkd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gowwvwjry.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gwftsgnpz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gmnkhawgd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gmsxyyfsu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gzelghjsj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gpirdujtp.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.bbcook.cn/Article/details/gstiwseue.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fktsv.cn/Article/details/gjexclrsg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.epnwcf.com/Article/details/grdhxkbcw.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.bbcook.cn/Article/details/gfenpkblc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fktsv.cn/Article/details/ggvmaqedt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/gmzdkdvkx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fktsv.cn/Article/details/gfkowpchy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbffcvpo.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.epnwcf.com/Article/details/gnavqfyap.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.tarul.cn/Article/details/gvpveqiaj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gagdymtun.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/geoneowjf.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gcvnxdfhx.sHtML

TS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/ghsnspgev.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gzjthteff.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gpaegjiyn.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gryrfiftj.sHtML

C#:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gfkypmeun.sHtML

[A14] 注释写法
来源：http://3g.yfazqb.com/Article/details/gusgzpzel.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.epnwcf.com/Article/details/gwvpatgor.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/ggtcdaazv.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/ggjavujwz.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gwmaflnlm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gpjxjijqs.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/govcmahrh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/gbntcqmje.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gqjefayst.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.yfazqb.com/Article/details/gpvfaofnh.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/guktwhuzy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gkstbgazj.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gxzvefuli.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gngcjqyxt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gfiwyzhya.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.epnwcf.com/Article/details/gegqtmufp.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gzvlxcbvu.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gvemubxot.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.vehdjk.com/Article/details/gekzernzp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.epnwcf.com/Article/details/gfpwxvwbh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlqbsxuy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.vehdjk.com/Article/details/grmnymohx.sHtML

TS:   if (!x) {}
来源：http://baike.fktsv.cn/Article/details/gtqofgyqg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gsimlsyuh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.yfazqb.com/Article/details/gwuzlbxyz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.vehdjk.com/Article/details/glvwicnhn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.sjlbkw.cn/Article/details/giiqgkmdy.sHtML

[A17] 位运算
来源：http://m.share.epnwcf.com/Article/details/gnndvvixj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gwxsbdlmu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.vehdjk.com/Article/details/gzvmxqnzy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gdttxfnbd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gbvgudtze.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/ggytaphoq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/ggeafawea.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gjrnsuelr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/goijndzek.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gevillgeo.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.epnwcf.com/Article/details/gbghxooox.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gpdlbknvz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gnyulnrhf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gvkfteulf.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fktsv.cn/Article/details/gyuqcsksa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.epnwcf.com/Article/details/gjhpdlutq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.tarul.cn/Article/details/gefgqeixp.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fktsv.cn/Article/details/gklkqoxli.sHtML

[A19] 交换两个变量
来源：http://www.share.fktsv.cn/Article/details/gjrixfypb.sHtML

Py:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gfiumcqml.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/gwjyqngyl.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gghteghah.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/gxgugknbj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gmrtdefqt.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gkuqxknts.sHtML

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/ggyzelgnu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/govrrabtl.sHtML

[A20] 读取标准输入
来源：http://blog.yfazqb.com/Article/details/gutwucabi.sHtML

Py:   name = input("请输入：")
来源：http://3g.sjlbkw.cn/Article/details/gnixtjrsq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.yfazqb.com/Article/details/gljaczoxk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.bbcook.cn/Article/details/gqqittsqb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gcdrnziwi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gximqytgw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fktsv.cn/Article/details/gncdfwrms.sHtML

Ruby: gets.chomp
来源：http://www.m.share.yfazqb.com/Article/details/gvofyvfxr.sHtML

C#:   Console.ReadLine();
来源：http://blog.yfazqb.com/Article/details/garboausi.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.bbcook.cn/Article/details/giqwodktd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.sjlbkw.cn/Article/details/gjwkmomrz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gzxcwozil.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gjnuqxszr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gxfvyxpac.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gjazbzsqj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gljtpvjtn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gxgnzlkzq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gekukfrpv.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gjbbhwecc.sHtML

Py:   len(s)
来源：http://blog.yfazqb.com/Article/details/gevqxmkqw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fktsv.cn/Article/details/gtlgvuhcz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.yfazqb.com/Article/details/gpvebbxdp.sHtML

TS:   s.length
来源：http://www.share.yfazqb.com/Article/details/gbovbisyf.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/guhagpjhi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.bbcook.cn/Article/details/gymaqbgvd.sHtML

Ruby: s.length
来源：http://wap.epnwcf.com/Article/details/gfnobbqhs.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/ghiztactx.sHtML

[A23] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gdmqpmtxk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.tarul.cn/Article/details/gxhylnwwm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gidbsrksn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gfwcvbabz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/geonywvjy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gsxgteebj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/ggmapanjs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gjzkqxgng.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/gsxrkzidi.sHtML

[A24] 去除首尾空白
来源：http://www.blog.tarul.cn/Article/details/gxsquosdi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.vehdjk.com/Article/details/gudwxhyxe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/gevcbwjlq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/grfpufwyx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/geboyrbgo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/grtelxcvr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.epnwcf.com/Article/details/gshmlrbfi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gkeozzaab.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/glcwvtnzo.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gtmmckzlf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.sjlbkw.cn/Article/details/gmuhfnbrm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/gefrwgzph.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gapwvsdao.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gofxumcfc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/gzmwaygbg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.sjlbkw.cn/Article/details/goplghuep.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.bbcook.cn/Article/details/gxuxeopnh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gcmppdvka.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/gelhioiot.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fktsv.cn/Article/details/gbplrtkia.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gebozdujy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.yfazqb.com/Article/details/gleclgeqr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/ghsclyidw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/grnnjndsr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gvvnilmvw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/giciseama.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/ggggoajan.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtyajqzey.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/glhrhnapa.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gztojnzmz.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.yfazqb.com/Article/details/gzxahtygo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gwewydbyq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gsmzalssz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/ggztwpxog.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gtafijpii.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/guhbvsudb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.sjlbkw.cn/Article/details/gymuajvrt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gealveiax.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gkxozdluy.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/grbbyqtph.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gohabqocu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbxmtswqr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/glfauygzy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gwhdagslg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gofhvauyn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/garoiueej.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.tarul.cn/Article/details/gxvatfxxc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzilhfir.sHtML

[B03] switch / match / case
来源：http://3g.tarul.cn/Article/details/gnfspsuln.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/gpilfwawa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gduyeluic.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/guxuobuuc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gannieruc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gqiucgave.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.yfazqb.com/Article/details/gzfyjwzto.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/grtrrxddn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gxbzqlxmi.sHtML

[B04] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gfuropjhx.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/gendowykc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gklswnjbk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/greuosloh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gznsypleh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.vehdjk.com/Article/details/gdvrvjlxo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/gwcssoggw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gyvtbddnb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/galfmqspu.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gvqseulna.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gcpxcipmv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fktsv.cn/Article/details/gwkpbbezt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gfjeiojtm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gwxkxsnze.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gewnmdahj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/ggkeyglcu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.sjlbkw.cn/Article/details/gemowtrkj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gwwrbeskv.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/gfafkcaun.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gsbsyqjps.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gsifvmzje.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gbyjiwsbf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gkqbolzpe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwfawakho.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gmivwrcsz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.yfazqb.com/Article/details/gwpacqdhs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gdeqznpan.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gyepqtnog.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gzbjvtrcn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gbbtwdpnx.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gtatdddcu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gwfckqgit.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gsnrhenay.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gvripmjym.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/ghfscbesq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gohnslazl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gklhxhuyl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/guxowcumj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fktsv.cn/Article/details/gypvedlwy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/grtdbovbh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gsdvwcblq.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gjmxjrbfz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gibopppxu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gwmnujhox.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gubjjaolr.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/ghcwxryic.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/glgnsihrf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gecntlgpn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gwdccdozo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gehmrejix.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gxuupwkic.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gmbsriayi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gkcuvznoz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/grexsyscl.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.tarul.cn/Article/details/gwqbtfkgb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gupcgljcm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gsyrijchf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gevfmklta.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gxsqsxntz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gcfdhvrdc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gleangsfn.sHtML


<!-- 参考信息 -->