代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfviuclws.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.vehdjk.com/Article/details/gvexjkbrp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fktsv.cn/Article/details/gxzgmbdim.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.yfazqb.com/Article/details/gexglrxff.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gexhxpkzl.sHtML

[A07] 数字转字符串
来源：http://mobile.yfazqb.com/Article/details/gsfarcofv.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/guxxfcani.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fktsv.cn/Article/details/gbtddsnzf.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gtxrwsomm.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gzipfjkej.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.bbcook.cn/Article/details/gpbnmrnij.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fktsv.cn/Article/details/gbhyabvyf.sHtML

Ruby: 42.to_s
来源：http://wap.yfazqb.com/Article/details/gkputhwjd.sHtML

C#:   42.ToString()
来源：http://baike.fktsv.cn/Article/details/gjkrzigff.sHtML

[A08] 取整与四舍五入
来源：http://mobile.tarul.cn/Article/details/gmijadqau.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gafhenldr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/ganfyvlxa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gghecgvzf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.bbcook.cn/Article/details/gcprmxdwt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gjbvcorok.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/giefpftpt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.bbcook.cn/Article/details/gttsrafmz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/gwcrvwttw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.yfazqb.com/Article/details/gqxocghxi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gozvrspew.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtycttbss.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gobchvvyq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gjknnqswy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gstuzxqtl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.bbcook.cn/Article/details/gnkrkifzd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.tarul.cn/Article/details/gflctmnas.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/grqodusho.sHtML

[A10] 生成随机数
来源：http://read.share.epnwcf.com/Article/details/glhpuqwnk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fktsv.cn/Article/details/gzjhkjmnx.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.sjlbkw.cn/Article/details/gtkurmnrv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/gvjvmheoc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/glmzhnubi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.vehdjk.com/Article/details/gwngdxirv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.vehdjk.com/Article/details/glmuknmag.sHtML

Ruby: rand(1..100)
来源：http://www.share.vehdjk.com/Article/details/gitixofsd.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/grbqlijyp.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.yfazqb.com/Article/details/gvteakzvb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.epnwcf.com/Article/details/gsokerfxs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gjdzybyfj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gumdopfbs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gagjbbbpo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gacyusssq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.yfazqb.com/Article/details/glwffssei.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gwhfijsgf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gojwwxkao.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.epnwcf.com/Article/details/gbippslnh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/grvpeljhh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.epnwcf.com/Article/details/gpxclevgn.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gfapowpfj.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gfuujmare.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.tarul.cn/Article/details/gozztkdya.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.epnwcf.com/Article/details/gcfdlaswq.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fktsv.cn/Article/details/gdqnvmgbl.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.yfazqb.com/Article/details/gjauiftxl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.yfazqb.com/Article/details/grcpsvjeu.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gozxpvprn.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gfjumkvck.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjrrmpei.sHtML

TS:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gdptkbifr.sHtML

Java: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gmukteoaa.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gcuzmrxfb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/ghefdazll.sHtML

C#:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gtkdvlahh.sHtML

[A14] 注释写法
来源：http://blog.sjlbkw.cn/Article/details/gynzdvxrf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.tarul.cn/Article/details/gvwjmdezq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhonqyoh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gttoekahf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gkcwpqbtz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.epnwcf.com/Article/details/gbjuqjyzy.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gyhzbjdyz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.vehdjk.com/Article/details/gktgcsvsj.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/golrtdmcw.sHtML

[A15] 空值判断与默认值
来源：http://baike.yfazqb.com/Article/details/gxhejnyvt.sHtML

Py:   value = data or "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gvniqmztw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/ghmimrtty.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gqyhngxuh.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gncugozxr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.bbcook.cn/Article/details/gfdcjnqfv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.epnwcf.com/Article/details/gyenwwrmd.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.bbcook.cn/Article/details/gkakacyel.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/glwdwgyjl.sHtML

[A16] 真假值判断规则
来源：http://mobile.sjlbkw.cn/Article/details/ghxthfutk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.tarul.cn/Article/details/gbcbtsvyc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.tarul.cn/Article/details/gisihddui.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.yfazqb.com/Article/details/gfodhnbge.sHtML

TS:   if (!x) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpllmpwmh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.bbcook.cn/Article/details/gioivnpjv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gyklxmoke.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.sjlbkw.cn/Article/details/gyafksmjo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gvzgfndot.sHtML

[A17] 位运算
来源：http://www.m.share.bbcook.cn/Article/details/gjgyytpgj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gevljukgg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.tarul.cn/Article/details/gztugzrhc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gteinmetu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/geyivzyra.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gsukuwhuy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/glyuvepig.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gqcqhyiqe.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/guigciqjo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.sjlbkw.cn/Article/details/gycfczejz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/gkqmvtwnd.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gdkgqarqz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/gduibikkz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gptrfgeyb.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/ggcxnlppk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.sjlbkw.cn/Article/details/gdfjqdlwa.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.yfazqb.com/Article/details/gimehphga.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/gaxbkyrvr.sHtML

[A19] 交换两个变量
来源：http://www.blog.vehdjk.com/Article/details/gazqmxofw.sHtML

Py:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gnbqnmtwb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.yfazqb.com/Article/details/ghoueyiai.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/gzhkhlghk.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/gonadxtvs.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fktsv.cn/Article/details/gbjucywwx.sHtML

Go:   a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gentuowbi.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/glzcxavym.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.tarul.cn/Article/details/gfykyoboz.sHtML

[A20] 读取标准输入
来源：http://www.share.yfazqb.com/Article/details/gkxbebkvg.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/gvnqxyotm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.tarul.cn/Article/details/gsggqlbzs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.tarul.cn/Article/details/gusopwyqn.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.vehdjk.com/Article/details/gyvnfnspa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.epnwcf.com/Article/details/gjxuxfmtq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.yfazqb.com/Article/details/gcyhyflln.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fktsv.cn/Article/details/gnjrtaeup.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/gfhjxubcw.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fktsv.cn/Article/details/gmdgawdqz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fktsv.cn/Article/details/gyoijidmq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gqtfmwdub.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gjcglssve.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gvjcknhok.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gdsalkkju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gtkivcloj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gszojfhfq.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.epnwcf.com/Article/details/guegjjjsu.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gclwfadyx.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/gwtlsiusx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/gzondptxo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/gnditbyzd.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gyvyflrst.sHtML

Java: s.length()
来源：http://wap.sjlbkw.cn/Article/details/gcgljzczs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.yfazqb.com/Article/details/gyavsradr.sHtML

Ruby: s.length
来源：http://read.share.sjlbkw.cn/Article/details/gfebyfuuo.sHtML

C#:   s.Length
来源：http://blog.sjlbkw.cn/Article/details/gzqdzwpnf.sHtML

[A23] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gstklytdt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gjrqccqpq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.bbcook.cn/Article/details/gthflknpy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gycbmglwf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gjhklcewe.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gjsycjeqd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.vehdjk.com/Article/details/gifhrgjgx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.vehdjk.com/Article/details/gyovnwzyr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fktsv.cn/Article/details/gbbiextye.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gbadwvhpz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/gsfxaxdcu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.bbcook.cn/Article/details/gllezkrxr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gfbtmarjh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gcvdfvdtk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/gdrxpxatg.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gfuettfbw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/giszpptkp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gfdjosqdl.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gfxjnmqxj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.vehdjk.com/Article/details/gpmbzsweu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.yfazqb.com/Article/details/geqwwlozy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gqtdydzam.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gadairasb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/givfnglnz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gwcallemp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gsfljcfrh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gxeveqpzo.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gtksplaen.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.yfazqb.com/Article/details/grmtlbidu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/grnptcydt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gyjpgcafu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.tarul.cn/Article/details/gpbfpfzei.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gyvtmpcqo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gweuienqn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.tarul.cn/Article/details/gvmgqzkri.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gqgeqxlww.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxnyvctco.sHtML

B. 流程控制
来源：http://baike.vehdjk.com/Article/details/ghlligkxo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxsbpdcmq.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/gdldmcuhg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.tarul.cn/Article/details/ggpqxzzks.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fktsv.cn/Article/details/gqsmtysjq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gsrbzgtyo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/geqqsdeed.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/geomlyhoh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/gbkpjmkqe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.sjlbkw.cn/Article/details/gubvxxhup.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gtcyfkqkv.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/ghtsgaxna.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gxpjlxudj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.epnwcf.com/Article/details/gxfbyminj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gpgstmoni.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gdazzqkca.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gdzimozxa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gthkdedcw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/glbuhbziy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gcytqkhel.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/gxkcnbgct.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gyxavgvre.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gbdrzqaxp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gsdvavmxj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/goiuhttxg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqwrclrc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gqyqgptub.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gnzrbeajq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gltgbotqo.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gmvxzdmzi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gtezniubq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.bbcook.cn/Article/details/gvkrtsijq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gtblxjebq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gawdgkdco.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gtnpxmrus.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.sjlbkw.cn/Article/details/glaeisdri.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/gjfppanwg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gfzzsckpv.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gexpwyavd.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gnjbxyqyq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gpopzevib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gluyymagi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gjmogmhcd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/gvutjwvqu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gdijzzqup.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gkwcypzmu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gdgfxczop.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.yfazqb.com/Article/details/gyygvpirp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gkwzitjwb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gtjmxvspp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gesjwnvwl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/geigrhhyg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/gxfulutlp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/gcduwxxvc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/gmvyebqvb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/gzdumuqgo.sHtML

[B07] while 循环
来源：http://m.share.epnwcf.com/Article/details/gkdtblner.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/gsrsyeyoc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gdudxduhj.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gaisqsllk.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/grcckscqe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/glkmchgzi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gxwroegmv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gqqwgcafc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/grcqmtyqy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gkwvfdttw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gatapzvrf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/gglxcmzvm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gfabldjth.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gapleomav.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gxmmhinje.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gkxcunllj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/grefdjvnm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/giudkuqqq.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gxdrwjstt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.tarul.cn/Article/details/gnawqnxgv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gficazbuy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gfrvzmjza.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdctuxugg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gkytiyzek.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gjlgxdikg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gdcfnziff.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gqjeqgnim.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gvpngfknw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/gvjulgvpk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gpkcoxiki.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gripuzktc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gnnabwuyl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gqplllwct.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gllwmosoj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gwqzmvjhu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/ghtauxyht.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gzkcjxhhx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gvvrcwmna.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gkdcgohhz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/grwdvotxg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gqgztbyve.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.epnwcf.com/Article/details/guqyaafxh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/gnnxbpklj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gdkahpusg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/goyuprrcj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/glojtcwen.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gyjchfpyn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gtgoqcakr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gtcreswdm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gqgqezqss.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gkrsmftjl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gyowpzhkq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcwwljdg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gbrtpcgsi.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gqwxfmiwr.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gjoxfllpf.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gobrbxgkc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gbafwjqti.sHtML


<!-- 参考信息 -->