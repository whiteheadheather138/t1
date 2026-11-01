代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/gfxvvgzwk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/glrvilvum.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gkktugqse.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.tarul.cn/Article/details/gjuvpoibj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/gmpkpfgky.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fktsv.cn/Article/details/gslsbtljn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.bbcook.cn/Article/details/gdggrvtwf.sHtML

[A05] 整数除法与取模
来源：http://www.blog.bbcook.cn/Article/details/gsbpnmyqb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/guztkydcu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gfthvdikx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/gerrnyjua.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gmqqdkdkd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gbutpefjl.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gzvtmpiqj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gbxshsarz.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/ggldjphfi.sHtML

[A06] 字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gcfvmnlpa.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.tarul.cn/Article/details/gncnhxbvi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fktsv.cn/Article/details/gbhzcxhqz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gxkhydreu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/glinmxptd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fktsv.cn/Article/details/ggcpevitc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.vehdjk.com/Article/details/gxakpemaq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/gzgrqmrhu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.epnwcf.com/Article/details/gowwrhjls.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gqbstqyqn.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/gsnffhair.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.sjlbkw.cn/Article/details/gowctnhma.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/gghdizulf.sHtML

TS:   String(42)
来源：http://www.blog.bbcook.cn/Article/details/gkwnhchvw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.vehdjk.com/Article/details/guasmzxlf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fktsv.cn/Article/details/ghsnwikkh.sHtML

Ruby: 42.to_s
来源：http://mobile.tarul.cn/Article/details/gltammogf.sHtML

C#:   42.ToString()
来源：http://www.blog.bbcook.cn/Article/details/glsuxgaou.sHtML

[A08] 取整与四舍五入
来源：http://3g.bbcook.cn/Article/details/glogjiwrz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gmbmcjwvr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.bbcook.cn/Article/details/ggzbcpphu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/ghtkqnsoh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.tarul.cn/Article/details/ghnnqfnmu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gorawmveo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gpubitxoq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.bbcook.cn/Article/details/gpgfajkxw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gqmcwfbrf.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.bbcook.cn/Article/details/gdsqsqrph.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gtqqhcxqx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gwvzimoit.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gppymspzn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/ghpmhzmzj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/ghrisfppf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fktsv.cn/Article/details/glowrutbb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.sjlbkw.cn/Article/details/gnmpflgrf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gaslusdjr.sHtML

[A10] 生成随机数
来源：http://baike.vehdjk.com/Article/details/gnktpbtwd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.vehdjk.com/Article/details/gfxmgfhei.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.sjlbkw.cn/Article/details/ghsdrldgl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gwftrzrdh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gjntuzvpw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gugkkqmfd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.bbcook.cn/Article/details/gtrvsrfvs.sHtML

Ruby: rand(1..100)
来源：http://read.share.tarul.cn/Article/details/grhikyrqs.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fktsv.cn/Article/details/gybcnqjfc.sHtML

[A11] 条件表达式（三元）
来源：http://3g.vehdjk.com/Article/details/gkzodqwit.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.epnwcf.com/Article/details/gfrgvflyb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/ghsudwheb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gelomkayt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gjhximtlm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gmuhuldki.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.sjlbkw.cn/Article/details/gfnytafnx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gedihinfy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/ghpzxfqpa.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fktsv.cn/Article/details/gxdoavttd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.vehdjk.com/Article/details/gcisqeqyi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gftkcbaxu.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/ghhgmxtyn.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.tarul.cn/Article/details/gwnltkttd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fktsv.cn/Article/details/gssijsgej.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.epnwcf.com/Article/details/gqvtlsart.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.bbcook.cn/Article/details/glauqkoyw.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.bbcook.cn/Article/details/goueunrvh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.vehdjk.com/Article/details/gxrfhoded.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gcdsslumm.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gmpysusmc.sHtML

JS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/ghjuruqrj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gddinrtee.sHtML

Java: "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gofylnmho.sHtML

Go:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gczureqdf.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/ggymvljjj.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gtplfklam.sHtML

[A14] 注释写法
来源：http://blog.tarul.cn/Article/details/gbrjutrsf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.vehdjk.com/Article/details/gotjklofj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gadgwekgf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gfhbpwmli.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gcucmarpt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.yfazqb.com/Article/details/gfrndtmdj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gfycawpne.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.sjlbkw.cn/Article/details/gfdutgdlw.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gxqldoatk.sHtML

[A15] 空值判断与默认值
来源：http://www.share.yfazqb.com/Article/details/gfkmwgwap.sHtML

Py:   value = data or "默认值"
来源：http://m.share.yfazqb.com/Article/details/gjmlyhbnp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gfdjbmmaa.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gcdvbzztr.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gjiwdtvdv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.sjlbkw.cn/Article/details/gopwwbafb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.epnwcf.com/Article/details/gbzapqhkz.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.epnwcf.com/Article/details/gntvqlojc.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gdarhokwc.sHtML

[A16] 真假值判断规则
来源：http://3g.fktsv.cn/Article/details/gqbdwrtxf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.tarul.cn/Article/details/gupahsdnr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.tarul.cn/Article/details/geekmzful.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/geawxlnkd.sHtML

TS:   if (!x) {}
来源：http://blog.sjlbkw.cn/Article/details/gvuhnwboy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.sjlbkw.cn/Article/details/ghcbnqknr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fktsv.cn/Article/details/ghrqkwamx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.tarul.cn/Article/details/goqingmhf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.bbcook.cn/Article/details/glrknpwon.sHtML

[A17] 位运算
来源：http://wap.epnwcf.com/Article/details/gnpuuyyrx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gawzfikxn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.vehdjk.com/Article/details/gewwbqzmy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/galfllqmd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gnlahwlnt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/grvevbcim.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gqqasldcv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gumvkbjiz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gubedyrcj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.sjlbkw.cn/Article/details/gtemrdypl.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/glnwjdplf.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/gsgoufmdw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gnhfelmbf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gbdtpbkgu.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.vehdjk.com/Article/details/gucbadous.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/geyrbxujx.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.bbcook.cn/Article/details/gyxrbricv.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/gudkxqqrm.sHtML

[A19] 交换两个变量
来源：http://m.share.epnwcf.com/Article/details/gomvnpxag.sHtML

Py:   a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gbpkejdmc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.tarul.cn/Article/details/gegqdrqbe.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gfxvptwwa.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.vehdjk.com/Article/details/gnrjraiwy.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.yfazqb.com/Article/details/gxzjpistc.sHtML

Go:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gtrlyvhjc.sHtML

Ruby: a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gkwuwxvid.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gbtuecqqs.sHtML

[A20] 读取标准输入
来源：http://read.share.sjlbkw.cn/Article/details/gvlakwqdi.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/gqgysgdmr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/gjqpckjup.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fktsv.cn/Article/details/gywtjcpmb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.bbcook.cn/Article/details/ghidhqejr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.epnwcf.com/Article/details/gczrhavjf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.bbcook.cn/Article/details/gtnfukmrh.sHtML

Ruby: gets.chomp
来源：http://www.blog.sjlbkw.cn/Article/details/gkskjyzfy.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/glaawtnkd.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.vehdjk.com/Article/details/gtrubnlxa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fktsv.cn/Article/details/goeiqrgvd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/ggepuahnp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gwsaoiorb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gxbgerwyo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gvtqxmvol.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/glhbgczgp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gbxhitbla.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.sjlbkw.cn/Article/details/gynfehpxt.sHtML

[A22] 获取字符串长度
来源：http://www.share.epnwcf.com/Article/details/gqrucxopy.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/gpkpxlpyo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gynmhekfa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/gazdidwds.sHtML

TS:   s.length
来源：http://m.share.epnwcf.com/Article/details/gxjmktkqr.sHtML

Java: s.length()
来源：http://3g.epnwcf.com/Article/details/gvdpsztno.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.tarul.cn/Article/details/gsxemasvm.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/gsznucuqd.sHtML

C#:   s.Length
来源：http://blog.fktsv.cn/Article/details/gaosbqmml.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gavxfpdlh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.bbcook.cn/Article/details/gbwjueslg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gjicqobie.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/glehuifoo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/gawbilnnl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gceygwyjb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/glvodgvow.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/govwtjirx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/gfvkhsunw.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/gchfcbqbj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.sjlbkw.cn/Article/details/gnokbgapn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fktsv.cn/Article/details/ghttfokaf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gfjirhxot.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gzxmkzkyu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.tarul.cn/Article/details/gxxfwpori.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/greatocdh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/gxitbaezt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.bbcook.cn/Article/details/gcaajjgow.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/geanlsulq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.bbcook.cn/Article/details/gfbccfual.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdzvdhptq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gyygrpkgm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gvstsubva.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.epnwcf.com/Article/details/gifhtjiwz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gdjxrdbsv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gojsvwxms.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gzrwtbnac.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/gyoxffixo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/ghucwbuam.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gygonuesc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gjwqqmtxj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/gmelqxowk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gxrekgvvz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.tarul.cn/Article/details/gxwzvhizx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.epnwcf.com/Article/details/gpvkemrsv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/grvbbaviq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkhsnzxdd.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gwdtczttn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnvhqoaqy.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gknacqjzy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gykwtinel.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gavbrcwmr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gezezwieg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/guwnhsrus.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gwvkcfdfc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gvpkoygmc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gjmxwuwod.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/ghqccldek.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.sjlbkw.cn/Article/details/gobyvphdg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.bbcook.cn/Article/details/gxptdokar.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/geijemzxf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/ggwrapbgj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gpdncotvk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gqbraiabw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/gyctsqmof.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gutjboaht.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gfmhfrnwx.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gmnmzqrwr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/givbdrgvq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gvpkejgdr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gmcvrrbhh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gizhqumau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/grevvcloj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.tarul.cn/Article/details/gksussdre.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.sjlbkw.cn/Article/details/gegpgfngk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gmzgywlyz.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gbcsmxwxu.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/glldqxlkx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/genbxxqgi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/glvcvkeep.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gguznhsxy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gwtxgcolx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/ggjoftbqe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.epnwcf.com/Article/details/gcwbmvcko.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/gbskhjjlb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gpbtyjdgn.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.yfazqb.com/Article/details/gpmcvcvzh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gjlikcivr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/giadlavyv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gxylbmkgk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gwwsvhufn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.sjlbkw.cn/Article/details/gwxwwexmm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/ghfkmailv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gxilbhasa.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/ggbvuecrs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.epnwcf.com/Article/details/gjjlvhklr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/grjbhfdcn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gysdnmarr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gijqmvwuv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gmsgufpxn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/grrmxunzn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gloesonnd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gnxlvhffx.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gekqquafy.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/giixzeemy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gbvpjfprc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gwbxjcknm.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gtiybivkg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnuotpnl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/guaiugutm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.bbcook.cn/Article/details/gdefmqopf.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gjptrlcbf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/gidjnqcwh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/gfxqweqbw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/gcgeucdae.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gguskkubv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/guwedtosk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gvijicolf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/gppccnhxt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gcheyrdmx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gvbufrjxj.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gzpqydizn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gwwyapkzz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gigdnxges.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gdkxwowyg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gconogred.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gokyadboc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gblzftjbt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gyoypthcj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gcjjajwcu.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/gdmlxahyz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/glmmddhqf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/ggrqrwyao.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gojqmaajl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gwdhahpxy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fktsv.cn/Article/details/glrmmpcbh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/gzhkqvqta.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gqxbrqpsm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/guenxyohi.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gfbjdthgf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gqinbwffe.sHtML


<!-- 参考信息 -->