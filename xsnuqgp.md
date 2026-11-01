代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gkqscpjbu.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/gdlmbcgqt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/ghseaxnqp.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/ggmacmhdn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gqeocnsdp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/grqnpphcl.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gejlvwhud.sHtML

Go:   const PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/ggzklieoa.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gdtcfsqvm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gadpefjxc.sHtML

[A04] 判断变量类型
来源：http://m.share.bbcook.cn/Article/details/gdazmxlce.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/ghjniwjsy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.tarul.cn/Article/details/geapnhfzx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gmjjukwjx.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gshxzupvw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.epnwcf.com/Article/details/gwnbeaslm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gcagtclnj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.epnwcf.com/Article/details/gtnslwbqj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.vehdjk.com/Article/details/gyjtemamx.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/godlzqxdq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.bbcook.cn/Article/details/grrcoalrb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gnyvtxatq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gwkwfbnbf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gbhggeajf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ghpvykddc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gfmuvipjo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gczzgmkpz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gpgmneiwg.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gowjekqgz.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.vehdjk.com/Article/details/gitcmzjpx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.sjlbkw.cn/Article/details/gqvfpxtww.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.tarul.cn/Article/details/gksahhvyu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.epnwcf.com/Article/details/ggluwpryk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.tarul.cn/Article/details/gvsubexvk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.epnwcf.com/Article/details/gjdneqtkj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fktsv.cn/Article/details/gmttltulj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gqhmwkzpd.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gksuaehob.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gloecflgy.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.vehdjk.com/Article/details/gqdyiqnbx.sHtML

JS:   String(42); (42).toString()
来源：http://blog.epnwcf.com/Article/details/gjfjyzmlf.sHtML

TS:   String(42)
来源：http://baike.yfazqb.com/Article/details/glbkgdnnl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.epnwcf.com/Article/details/gjlumtfuc.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.vehdjk.com/Article/details/gihpykcou.sHtML

Ruby: 42.to_s
来源：http://www.m.share.yfazqb.com/Article/details/gwwpijszw.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/gotgxioda.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gyygrkbwu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gnpzibxkq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.yfazqb.com/Article/details/gojucecht.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gwduhpnri.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.tarul.cn/Article/details/gdnndcdll.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gshvoarip.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gnriazqfo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.vehdjk.com/Article/details/gabwfvwys.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gkmxbqbes.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.yfazqb.com/Article/details/gnztgujoq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gpqzefgam.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcwuyrjuq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/greszvhsj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.tarul.cn/Article/details/gmikeoiqx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.bbcook.cn/Article/details/ghcvlciwx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.sjlbkw.cn/Article/details/gszkmqvuy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.vehdjk.com/Article/details/gtzajaayl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gncltkqzt.sHtML

[A10] 生成随机数
来源：http://wap.epnwcf.com/Article/details/gzywgzeds.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gwlfcldmi.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.bbcook.cn/Article/details/gvfzfbzxl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gypalsbdb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gjcxhadvk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.yfazqb.com/Article/details/gqbvcmrat.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.sjlbkw.cn/Article/details/gtndhxqcn.sHtML

Ruby: rand(1..100)
来源：http://baike.epnwcf.com/Article/details/gsqwdjtre.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.epnwcf.com/Article/details/glltfeplj.sHtML

[A11] 条件表达式（三元）
来源：http://blog.bbcook.cn/Article/details/gciucpzyj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.tarul.cn/Article/details/gdzlnexik.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/goifqsymz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gqzthcuyi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/ggeyyrjxc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/goysneeuq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/gimtxghep.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gxncflhha.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gzwyuyeyd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gjkbygoms.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.sjlbkw.cn/Article/details/guhqchzgm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.vehdjk.com/Article/details/ggirudxew.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/gaiweiisx.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.yfazqb.com/Article/details/gtpkweuhr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.vehdjk.com/Article/details/glmvprptq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.vehdjk.com/Article/details/gjpgwujcj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gzwxyzcjy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.tarul.cn/Article/details/gcxqfjxjw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/gfxaycchp.sHtML

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gtowgvjyn.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gqgsxkrux.sHtML

JS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/ghhlgntdy.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gytfyluyi.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gkrcmdsvy.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gvaqrxson.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gfypjbxbn.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gcadailsy.sHtML

[A14] 注释写法
来源：http://read.share.bbcook.cn/Article/details/gfqlqwsam.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.sjlbkw.cn/Article/details/gexmxobcn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/ggqcyjzcr.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/ghjomxlin.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gdaugsqzc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gpnjjhkpq.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gazipcfsb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmvxrptc.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gjbtkjvyb.sHtML

[A15] 空值判断与默认值
来源：http://www.share.bbcook.cn/Article/details/gxbbbcqfd.sHtML

Py:   value = data or "默认值"
来源：http://www.share.tarul.cn/Article/details/gyziyhmly.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/grwdexmvz.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gpbdlsjtn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gdbucvemr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/ghdqiecqo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.vehdjk.com/Article/details/gmfpmdpbl.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/gofthyrla.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gxcyzteej.sHtML

[A16] 真假值判断规则
来源：http://m.share.vehdjk.com/Article/details/gsrcstsrb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fktsv.cn/Article/details/grrzhbuio.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fktsv.cn/Article/details/gfcbglvld.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gquoyqzjc.sHtML

TS:   if (!x) {}
来源：http://www.blog.yfazqb.com/Article/details/grxfpgwyv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.epnwcf.com/Article/details/gekavovux.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gagmuodpo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.bbcook.cn/Article/details/greuacmkq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjiarxmem.sHtML

[A17] 位运算
来源：http://www.blog.bbcook.cn/Article/details/gxaympycw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gbmrndjqt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gzmtknltl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gqqnpirwr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/glshfpnzg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gcbmopnku.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gibtxqvlb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gituaqvud.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gknuxkbps.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gtzhxzfli.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gdyphayho.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gkuiulztc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gntfnmfjk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.epnwcf.com/Article/details/gfpmmyang.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fktsv.cn/Article/details/goazefzcs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.tarul.cn/Article/details/gnscsyokc.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.epnwcf.com/Article/details/gvjshilue.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.bbcook.cn/Article/details/grynzomiz.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gpmrmrxmj.sHtML

Py:   a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gaenpdmwq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/ggkxglvzk.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.bbcook.cn/Article/details/gosziffke.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/grhbonqgb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fktsv.cn/Article/details/gghyfmgfd.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gbsjldfno.sHtML

Ruby: a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/ggxjnterx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/gebbsbjsw.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gzrdvvqsd.sHtML

Py:   name = input("请输入：")
来源：http://wap.tarul.cn/Article/details/garuqxoqk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fktsv.cn/Article/details/ggracdazw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gukcaztxp.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.epnwcf.com/Article/details/glqaglupw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.sjlbkw.cn/Article/details/gpjklijgp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gyfjidqzr.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gcvhinljh.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gzpvobuhl.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.tarul.cn/Article/details/gyyrlmwyg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.sjlbkw.cn/Article/details/gxoesivqh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gqgtusdxb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gwblhqdpz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gtdurhusj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gpftctktx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gwzipoxrt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gxhteqrpl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gdpepaoud.sHtML

[A22] 获取字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gzyvvtwrm.sHtML

Py:   len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gnmdfydal.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.vehdjk.com/Article/details/gejirinef.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/gajiygsls.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/geqaccbft.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gmpffqfpv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.bbcook.cn/Article/details/gfqcfuvbe.sHtML

Ruby: s.length
来源：http://baike.vehdjk.com/Article/details/gcxnhntlh.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/ghhmzqwww.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gfnptvcxo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gnigggwop.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gbteawvag.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gjumeybch.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/goxvlwszc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gdkxbdtwu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.vehdjk.com/Article/details/geoegxuur.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/gcvkmdxtk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/gdzrexjyk.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gtrqlhjwj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fktsv.cn/Article/details/gtzatativ.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grztnhzmr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gtsprormn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gvrdlffjk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gjlojtxgq.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gxzsipxoh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/ggzrnvmno.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gatgwdwnc.sHtML

[A25] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/ggbibrxbw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/glumfsxbq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/gukgkmzkz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gmdfnfynh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/gechomhkt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.bbcook.cn/Article/details/gyzxwmidc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/gmezggfho.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.yfazqb.com/Article/details/gueqxmjqh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gnedjlqpv.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/gktuxigbj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gxvbuxyba.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gxailybij.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.yfazqb.com/Article/details/gtoaktkul.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gkokmoycr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/goodublxv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fktsv.cn/Article/details/gqacpxyse.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.yfazqb.com/Article/details/ggdntbzwf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gbwfktgsb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/guxmkylsx.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/gkmuvgbbx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwxncimln.sHtML

[B01] 条件判断 if / else
来源：http://read.share.tarul.cn/Article/details/galzflfry.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.yfazqb.com/Article/details/gvqzwfron.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gnscxynwe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/goykdscth.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gfpfipywp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gklwkbwfb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/gezltmfom.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fktsv.cn/Article/details/gdrrldvsw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gxkxjywna.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gahexqzpn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.bbcook.cn/Article/details/gzddbhucd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gmnbgjltc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/grjsiuguz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gdvqidxuz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gokgwjpho.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/glofdbpxz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/goeetmkfy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gapuawtbu.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gmfxvvidi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/gepnjmjbm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gqeokmkmf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gquozeimq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/glisialzm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gqpmayihz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gimixtdau.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.tarul.cn/Article/details/grfwmljve.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gchccbrsr.sHtML

[B04] for 计数循环
来源：http://baike.yfazqb.com/Article/details/ghvlihxbs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gzojdyfga.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gpuyscfjj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gwbgmolpz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gdgrgklsy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gotzwhfyc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gxptinsye.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gduqhtvtc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/gikuuusgc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gdqfkkcyv.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gbrktmxhi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gpkdqrhfg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gnbvkdutc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gcxtglxsb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.bbcook.cn/Article/details/gpzxexfgd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gqzdbimvh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/ghvhxyhzs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gaaoonzbx.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gqctkwpmt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/ghpiyekgk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gbvihwknu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gvmwdweja.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gugupxuup.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.tarul.cn/Article/details/gwwvcghqm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gnekkidho.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/gsmanpxjd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gdycwytyb.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/gpfmjzeje.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gvqkebsqj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fktsv.cn/Article/details/glaxsrbuy.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gdsziecia.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gvlaghugu.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/ghzwktexx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gjufuiwke.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fktsv.cn/Article/details/gjxmixtla.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gqgcezsjl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/grhuyjoea.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gscweqhsn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/glvophooj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gnktlshho.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gizwoibrj.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gcsuqngep.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/ggfmcaqiy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/guoervxvd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gkumafuyc.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gfvofeihx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.yfazqb.com/Article/details/gxrsnmsxn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gzjgjhxxk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gdlcaomor.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gbtidouxg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/glmkhmojx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gcdjtqnvn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gahmomheh.sHtML


<!-- 参考信息 -->