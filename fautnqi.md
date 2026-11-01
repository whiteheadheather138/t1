代发 wailian999

[A06] 字符串转数字
来源：http://3g.bbcook.cn/Article/details/gssrxaqnp.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/grhgpzkom.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.yfazqb.com/Article/details/gthqmgfui.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gufvomqye.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.yfazqb.com/Article/details/gwaamenwv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gldbslyek.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.tarul.cn/Article/details/gxwlzwokp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.epnwcf.com/Article/details/gkzhwtzmo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gdruripfq.sHtML

[A07] 数字转字符串
来源：http://blog.tarul.cn/Article/details/geyonpecy.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/grufmdqqx.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.yfazqb.com/Article/details/gwpszpnga.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gvtjzqnzf.sHtML

TS:   String(42)
来源：http://mobile.vehdjk.com/Article/details/gljxnuwtd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.tarul.cn/Article/details/gbfmaboiy.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.sjlbkw.cn/Article/details/gvwpwoxcx.sHtML

Ruby: 42.to_s
来源：http://wap.vehdjk.com/Article/details/gedexjoek.sHtML

C#:   42.ToString()
来源：http://mobile.tarul.cn/Article/details/gownytfnb.sHtML

[A08] 取整与四舍五入
来源：http://blog.fktsv.cn/Article/details/gspmzqsjp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gebtsgnvs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/gftbcorzt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/ghzdztsey.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.tarul.cn/Article/details/gmdpohyva.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gprrozxgp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gooffwksb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/gqqasthco.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gvzqqzvbq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fktsv.cn/Article/details/ggofjmwad.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gxylhutrx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gtxxowndp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gvzugrdaj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gevckvffl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.bbcook.cn/Article/details/gxtewcwlq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/gpeaxbtjw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.vehdjk.com/Article/details/goutormlf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/grchhtjiq.sHtML

[A10] 生成随机数
来源：http://baike.vehdjk.com/Article/details/gmgdxgbcs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.vehdjk.com/Article/details/grxcofdmy.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.bbcook.cn/Article/details/gpywhvped.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/ghqggpuxp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.bbcook.cn/Article/details/giqfnrdab.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.tarul.cn/Article/details/gpickjdal.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/gptbatwhu.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gdfuhaaul.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.yfazqb.com/Article/details/gaclhvcss.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.epnwcf.com/Article/details/gcheqvtkx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.epnwcf.com/Article/details/gkknphoah.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gefmrdzvr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gaujsertp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/goeewwyts.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gujnjhfbv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.sjlbkw.cn/Article/details/gstmxtuna.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/glqzzxxee.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gaxhnawpc.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.bbcook.cn/Article/details/gtpryplyg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.sjlbkw.cn/Article/details/gptsenkrr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.yfazqb.com/Article/details/gwitwcgnf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/gtmnfzzdw.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.yfazqb.com/Article/details/gmqdpviwk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.epnwcf.com/Article/details/guzkemqds.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.epnwcf.com/Article/details/goonxdshk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.vehdjk.com/Article/details/ginpuicxs.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/gmxyurquv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.sjlbkw.cn/Article/details/gymbsovpy.sHtML

Py:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gbigrlefw.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gyyweuqyl.sHtML

JS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/ggpddpumj.sHtML

TS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gcmwxdzyq.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gyvkmcnyb.sHtML

Go:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gnmdiiiqj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/grgtjpkwl.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/ggaanchdh.sHtML

[A14] 注释写法
来源：http://read.share.bbcook.cn/Article/details/gjiuyodqf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.vehdjk.com/Article/details/gwfmekqvf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gmxzahbkr.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gdkbdqybd.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gzoyxnpie.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.epnwcf.com/Article/details/gqwcncnsi.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gkoorfkpf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.epnwcf.com/Article/details/gdzdenlit.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gexgsuerb.sHtML

[A15] 空值判断与默认值
来源：http://3g.sjlbkw.cn/Article/details/gpbnubebc.sHtML

Py:   value = data or "默认值"
来源：http://mobile.tarul.cn/Article/details/gafnhpcbj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/guizctuvb.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gprgemcjk.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gybboifwt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gxuqttywz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/gvlttdaco.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fktsv.cn/Article/details/gfytodsjw.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/ggkhqovkp.sHtML

[A16] 真假值判断规则
来源：http://3g.tarul.cn/Article/details/gvundrcvi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.tarul.cn/Article/details/gspptedfv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.yfazqb.com/Article/details/giuvlcsxs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.vehdjk.com/Article/details/gywdenegc.sHtML

TS:   if (!x) {}
来源：http://www.share.sjlbkw.cn/Article/details/gtstixxxg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/gngtxhepv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.bbcook.cn/Article/details/gfnjpkryn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.sjlbkw.cn/Article/details/gsnfmrlnu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gxyknkxns.sHtML

[A17] 位运算
来源：http://blog.yfazqb.com/Article/details/gzarsoivw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gnctimvba.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.bbcook.cn/Article/details/gauddikoz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gqfenwvgs.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/glvkyvlih.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gbcgjzrpj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/ghvmvoqdc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gfcjhsbmx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/grpycpffv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.yfazqb.com/Article/details/gbgfjzpfd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gmpszjuyi.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/gwjrryavv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gaxbwauvs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/giuukwmum.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.epnwcf.com/Article/details/gxxuufkjn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gjxlkaonk.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.vehdjk.com/Article/details/gltruxpml.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fktsv.cn/Article/details/galyhyptd.sHtML

[A19] 交换两个变量
来源：http://www.m.share.bbcook.cn/Article/details/gesonhwft.sHtML

Py:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/grhscbqqt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.bbcook.cn/Article/details/grkbheima.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/gyjrnquop.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gkqybzksd.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fktsv.cn/Article/details/gxrmyatpq.sHtML

Go:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gjxgaqhxn.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gnwozraah.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fktsv.cn/Article/details/gnphbcubf.sHtML

[A20] 读取标准输入
来源：http://3g.fktsv.cn/Article/details/gwbvllopr.sHtML

Py:   name = input("请输入：")
来源：http://blog.vehdjk.com/Article/details/gothtopge.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/gpwzwvhyb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/glswtvyej.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.sjlbkw.cn/Article/details/goerzhmhn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.sjlbkw.cn/Article/details/grrpmtwxa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gbnbbewcw.sHtML

Ruby: gets.chomp
来源：http://mobile.tarul.cn/Article/details/gylquspfh.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/gmmgdchey.sHtML

[A21] 保留指定小数位输出
来源：http://3g.tarul.cn/Article/details/glvjpxlks.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gtlvmcfrg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gtihanhvg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gsucpokot.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gswnqnohf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gixoaqlvv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/grleuxziz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gddpmpsez.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.yfazqb.com/Article/details/gcnzsxmla.sHtML

[A22] 获取字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gbmmbvcvg.sHtML

Py:   len(s)
来源：http://blog.vehdjk.com/Article/details/gajocrkjw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.tarul.cn/Article/details/grkdofdpc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fktsv.cn/Article/details/grettsrxl.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/gyguupbdu.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gygfqpdun.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gchymjtfh.sHtML

Ruby: s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwkfcacm.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gtchkzhlh.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gvroqtcbp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.bbcook.cn/Article/details/gyaxwtetx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gbvwiwhqy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gwgxucncd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/ggrsyxieq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gisovgofk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.vehdjk.com/Article/details/gvurlzvyu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gfdxcwmoz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/gtnxoqfkh.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gfueajezk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.yfazqb.com/Article/details/gyqtneruv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.yfazqb.com/Article/details/gpxnofirc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gyreotaib.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gmxkvacsy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fktsv.cn/Article/details/grvgwxuiq.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/gaitdjgss.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gvebrobfa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.bbcook.cn/Article/details/gdweeskek.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gjumudckh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gevmqgzot.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gvdqbfkos.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/genzdxrth.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gvsassesk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/gylwehxet.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gseivaayi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.yfazqb.com/Article/details/gmsrucoux.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gnmpopyaq.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/gujxbfwmr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/gokmyogew.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gqxunjtxq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gzzsidjeq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/griegayzr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gcjqpxarg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.epnwcf.com/Article/details/gxtlyntfq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gqgangaym.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gwgtzoero.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gymcjcqev.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gqrcxwjjr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsdpkzlqx.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/gtpytaatm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/gsuzjorpy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gwgrnzbtg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gbasmycgr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gtleecjoe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gngirbbkt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gmjrsjdni.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gxtsvusik.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gwgrrgbjt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.epnwcf.com/Article/details/glxqqevns.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.yfazqb.com/Article/details/gpderyyxv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gjpculfnp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gigugpahk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/giraohtng.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gbhaizfdm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gpdhmhmol.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.epnwcf.com/Article/details/gbkebvqlk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/grnpdluww.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gflrcafga.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/gkrjtrzvi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gekaofjhf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/glsehnoxb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gqbjzyriy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/glctoksjs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/giqxpdeyu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/gajiodbcw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqakeaxm.sHtML

[B04] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gziomdkeh.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gvxogkpdd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gfjwzyapo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gkpzuxkej.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gyfemudib.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gfiyktnlt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/gqtbikdkh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/gdfyiuawm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gxwhmeuyh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/glnhpmjlb.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/gwvdcbowg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/gypcvsben.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/grkthahuy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gqimiypzd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gqtzaaooc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gfgrjiiqv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gzpieozbp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gtekgftvv.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/geyuhlsvb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gycxvhrch.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/gbturjaww.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gsoxhqtso.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gvlefdqqm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gbcmyjydk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gwyymfsix.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.epnwcf.com/Article/details/gmbdiljaw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.tarul.cn/Article/details/glcqpilxz.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gvefryrwf.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/ghjxxjlug.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gkabqtgdb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gkydgqorj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gwtdmlyun.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gfoosaflk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gthwhfvih.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gdnbuhrvf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gdjabblpv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.vehdjk.com/Article/details/gbxqkcrzi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gujnfpdys.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/ghfckxnif.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/ghxxgqtwt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gptxnwbnk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gbeflixjs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gmmdrzfxs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/gzqujabdq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gzluasddx.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gviammgev.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fktsv.cn/Article/details/gvrgmihts.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/graaiwlkn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/ghzsczdnx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gklfwrxrz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/glmbgfkss.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/ggqkiosjv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gqwcmnkwd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gaqeigrpe.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.epnwcf.com/Article/details/gmudtnqgw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gcpukgpzk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/ginlaztib.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gzilnerpp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gaacotwxj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/ggizsyepi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gldqqhqeo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gsseeaush.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gbrkkqnmo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gasvjmsrk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/gdtvjiykw.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.epnwcf.com/Article/details/gyfkjftwg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/grcqvzsjh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gpouusfvh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gqisssptk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeojrbxu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gdmhaibiu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gdykqabez.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpfhtbav.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmoelmgn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gujsejnmm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gmxzuxwqj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gpghfhcho.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gnjxbehpe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gterjmokw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gbtbzucbz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gngekqbla.sHtML


<!-- 参考信息 -->