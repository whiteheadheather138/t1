代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvezjyft.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gcwtfqvcx.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gfpgleoxy.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gxiernztg.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gvznbwfmm.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gubyfixhz.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gyuzzdtby.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycaeykxm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fktsv.cn/Article/details/gwskrmdha.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.epnwcf.com/Article/details/gmmdiliha.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gnchrgufb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/gdkdefzxv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.bbcook.cn/Article/details/gmbpymjcm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/goglnmfuy.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.epnwcf.com/Article/details/giwnxfozl.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.yfazqb.com/Article/details/guugprwkm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gulhzfwkx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gfywskoqs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gptsbqwdg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gmkfzxyfd.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gsyimddpn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gonwsrcnh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gqfagepjj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gxyplcqnn.sHtML

[A06] 字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gdhsqajui.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.bbcook.cn/Article/details/gsoddbmgm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.tarul.cn/Article/details/gcjenhtcm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gclkjozpd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gckidursh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/gdkczreua.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.epnwcf.com/Article/details/gfglddfgi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.sjlbkw.cn/Article/details/gyxpdvzcf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gystdibjr.sHtML

[A07] 数字转字符串
来源：http://baike.fktsv.cn/Article/details/gtxmsrmeb.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/ghsgprdeb.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.epnwcf.com/Article/details/gbuunbbzq.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/gcpmjkrjw.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gsyccufiq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/giashttug.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.sjlbkw.cn/Article/details/gkzebmasd.sHtML

Ruby: 42.to_s
来源：http://m.share.sjlbkw.cn/Article/details/gbbbryfnc.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpputbmgq.sHtML

[A08] 取整与四舍五入
来源：http://blog.sjlbkw.cn/Article/details/gnkcrfsrx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/girtqoewp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.epnwcf.com/Article/details/gtwvymxzg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gntcrczog.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/gimiuapmp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gvlztckwt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gughbogua.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.bbcook.cn/Article/details/grqqqrqax.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gyvxewivx.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.vehdjk.com/Article/details/gctxaxsba.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gjrjgbjmj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.vehdjk.com/Article/details/ghqlpgjra.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gpdkhfdwz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/glgbbuxqm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/ggexkvtze.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.bbcook.cn/Article/details/gtvhnzpvr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.sjlbkw.cn/Article/details/gktpktzuu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gglhflwwy.sHtML

[A10] 生成随机数
来源：http://3g.yfazqb.com/Article/details/gignennkd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.tarul.cn/Article/details/gdiwabyco.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/goinpmfcl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/gnzzgmbfa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gxkfkkhwm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gvmqmvzgw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.epnwcf.com/Article/details/ghbauzmuq.sHtML

Ruby: rand(1..100)
来源：http://baike.vehdjk.com/Article/details/gzhdjnwig.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.tarul.cn/Article/details/gftpiryfp.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.tarul.cn/Article/details/glsiontun.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.tarul.cn/Article/details/gzkzecuut.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gylbxglof.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gajlnmjkv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gzjjsliqd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gnlmwgdiq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.sjlbkw.cn/Article/details/gnaikcwlr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/ghlltimfw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/ghfzkxweu.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.tarul.cn/Article/details/gybflgacl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.epnwcf.com/Article/details/gopoqbmio.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwvwtcfb.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/glxjnkrff.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.vehdjk.com/Article/details/gosrkpdva.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.epnwcf.com/Article/details/ghwhzawem.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.epnwcf.com/Article/details/gqjchrdhg.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/gjcqcfidy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gquuoaxuu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.yfazqb.com/Article/details/gqdrmhwzc.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/ghwfyfvti.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gzfsdlbko.sHtML

JS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gtrciuhwb.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/grlajpqjl.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gkaqxqnzx.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gfyggijdx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gtuwurxwc.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gzbabeapv.sHtML

[A14] 注释写法
来源：http://baike.yfazqb.com/Article/details/gcltsffsd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.sjlbkw.cn/Article/details/gutbwbczm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gujfgcoyo.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/ggxspmgva.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gusmrsxxf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.epnwcf.com/Article/details/gedvrtnbp.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gjkbtqpms.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.sjlbkw.cn/Article/details/gnkixmafp.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gzccpnijl.sHtML

[A15] 空值判断与默认值
来源：http://wap.epnwcf.com/Article/details/gdgyhmerz.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/ghwborqrt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/geitjcvjw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/grdqqmmat.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gpvfrilcp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.tarul.cn/Article/details/gemaiqwpz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fktsv.cn/Article/details/grqmtyzsl.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.tarul.cn/Article/details/gxxdxkkge.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gcvugxrla.sHtML

[A16] 真假值判断规则
来源：http://3g.bbcook.cn/Article/details/gbvtczelg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.yfazqb.com/Article/details/gvrqspati.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.vehdjk.com/Article/details/ggqehrnsx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.bbcook.cn/Article/details/gcygazvcd.sHtML

TS:   if (!x) {}
来源：http://wap.epnwcf.com/Article/details/gylbnyzlf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gsqgaggqf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/gweubqtih.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gqsbklwqu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gkgtjnaaz.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/grezlkfwp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gwjnaguth.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.tarul.cn/Article/details/gnltfqcms.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gflgziatf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/grfbxmoqi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gszuauvgx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gfcofyjgw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gtttusqqs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gvbazuisq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.yfazqb.com/Article/details/gmcsrbmcn.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/geyorrshu.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/glhnboptd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/grjjnbppu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gvzaxzjul.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.sjlbkw.cn/Article/details/gobgvcdgv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.bbcook.cn/Article/details/graebbmgo.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/gplyeuisy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/gtbbuybvz.sHtML

[A19] 交换两个变量
来源：http://blog.vehdjk.com/Article/details/gpbkjashh.sHtML

Py:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gkdrqtufb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.tarul.cn/Article/details/geolnmeyf.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gbpwmlmoo.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/gmsrlrdfk.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.epnwcf.com/Article/details/gtfoaaccg.sHtML

Go:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/govchwjdi.sHtML

Ruby: a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gujzfplrj.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.epnwcf.com/Article/details/grgqgkobv.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gpilmpxaj.sHtML

Py:   name = input("请输入：")
来源：http://wap.fktsv.cn/Article/details/gvlccxdrx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.epnwcf.com/Article/details/gfxddscka.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.bbcook.cn/Article/details/gowfvziot.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.vehdjk.com/Article/details/gksepgtsj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.vehdjk.com/Article/details/gezpwlkik.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gpmmragbf.sHtML

Ruby: gets.chomp
来源：http://baike.epnwcf.com/Article/details/gecoqejqk.sHtML

C#:   Console.ReadLine();
来源：http://baike.sjlbkw.cn/Article/details/gcugkcmnj.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/glghmexdl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.epnwcf.com/Article/details/gvbnonxzz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gdfqplrgz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gdvyrazlf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gobxtgelq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/geloqtkox.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gfxuqmujp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gkyontgvf.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fktsv.cn/Article/details/gjkijjnzz.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gnqblevud.sHtML

Py:   len(s)
来源：http://m.share.tarul.cn/Article/details/gzgikiutq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/glnekljmn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.vehdjk.com/Article/details/gzgyacwyk.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gxxjxjvkn.sHtML

Java: s.length()
来源：http://mobile.tarul.cn/Article/details/gsriqsuve.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.yfazqb.com/Article/details/grcyvglas.sHtML

Ruby: s.length
来源：http://www.m.share.vehdjk.com/Article/details/gckcysldz.sHtML

C#:   s.Length
来源：http://www.blog.vehdjk.com/Article/details/gqvonblcw.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gpdwotlxx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gghgvjrbo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fktsv.cn/Article/details/gbfxkshpf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gogonsabo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gwwoznkwb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gswmwzdsh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.epnwcf.com/Article/details/gxrxoqdjh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/gtwcgwxxk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gfmsamqdz.sHtML

[A24] 去除首尾空白
来源：http://baike.tarul.cn/Article/details/gapvpykwk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.sjlbkw.cn/Article/details/gaxtpnaxc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.tarul.cn/Article/details/gnfvygxtp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gsyvxicxg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gxajkkwim.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gfrdtbmyh.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/gwjymlwir.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.tarul.cn/Article/details/grdjwoljs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/gkgydqoaz.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gjfrkxguk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fktsv.cn/Article/details/gdidkpejr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gvbffdqmh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gwksphgcw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/glnamdwjx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/ggpwsgdas.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/ghqoxsvnu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.epnwcf.com/Article/details/gowynrhkw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gfvcbqrxj.sHtML

[A26] 类型转换总览
来源：http://3g.fktsv.cn/Article/details/gbbpzwfxo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gsrjoqrxy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.bbcook.cn/Article/details/gegfnhseq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/gqhkaznks.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fktsv.cn/Article/details/gvufdbohc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gjqvwkugh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gmmtglkdw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.yfazqb.com/Article/details/gdbzauche.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/goxnmqzvy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmprybiym.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/ghkigdstn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtjvywczb.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gpnlphzqq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/gfkstpbgm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.bbcook.cn/Article/details/gpxtympan.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gzkrjscbf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gyphnchun.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gyotqkbzm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gugoctzor.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.tarul.cn/Article/details/galkzqxxi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gscohewat.sHtML

[B02] 多分支 else if / elif
来源：http://blog.yfazqb.com/Article/details/gpnvkrtfv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gqbgfgukq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gvtourbsq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gxmpqrheb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gtsmxzrej.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gjopuznlk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gqcneguyj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.bbcook.cn/Article/details/gmzsxauau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gcmxpxaci.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gzaqxfmxa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/getweexxn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gltbqqfjg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gnjffgsoh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gcbgdbvpr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gjakyhaku.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.yfazqb.com/Article/details/gxmrrxivr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gygfvjzje.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gijdiiieg.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/gzvzejxks.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gnmrsoqyn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.vehdjk.com/Article/details/gckzhmxfq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gtloorcmw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/gotjqzwrs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gtwhpsqjn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gfgazlsls.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gfeclqvkd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.tarul.cn/Article/details/gwjsfqyqo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gsenscosn.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gqpmglqbo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.vehdjk.com/Article/details/gihmwchyv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gwoveqewz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gbthevoas.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gpyhddkbd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/grsfgzmjx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.yfazqb.com/Article/details/gqcjquzzg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/gensdyszf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.epnwcf.com/Article/details/goltzbdcg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/gwqlqqdvb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.sjlbkw.cn/Article/details/gavhkqlrl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gudkduvfo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gthkpqzxq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fktsv.cn/Article/details/gerjaffyf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.sjlbkw.cn/Article/details/gsfcftuip.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/grtdhbcxp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gtnulutth.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/guhoqqpez.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gsfozprxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gpifnzlar.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gglrfetbh.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/ggaecbwey.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gpdeqrmoz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/ghghpfody.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/gdnlcehza.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gyuruzuzo.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fktsv.cn/Article/details/gicbnbwzu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gukztjgtw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/glemhmyap.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gpkyheafd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gvywgtmvl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/grhxehqzj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gcglebfiw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/giytejwch.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/guxphuynw.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/gkmufyvcd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/getotppzx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gsexepuur.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gctliegrx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/grwflcdah.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gfqlpqpal.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/gtzifupkd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gwlqfhfgl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gvadjhqda.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gyffwmzrn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.sjlbkw.cn/Article/details/gfcasgrqp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gdpyvvxgc.sHtML


<!-- 参考信息 -->