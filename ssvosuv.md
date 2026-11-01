代发 wailian999

[A10] 生成随机数
来源：http://baike.sjlbkw.cn/Article/details/gczaaxlun.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.tarul.cn/Article/details/gzkgkopxk.sHtML

PHP:  random_int(1, 100);
来源：http://blog.sjlbkw.cn/Article/details/gduoxptex.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gdlklsnuu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gniwcpkkz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.tarul.cn/Article/details/gsqufkfgn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.epnwcf.com/Article/details/gtluqojwc.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gvmhvhask.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gluwqkfiz.sHtML

[A11] 条件表达式（三元）
来源：http://baike.sjlbkw.cn/Article/details/gromqdlhj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.sjlbkw.cn/Article/details/gmeydrfbi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/girbqqzdp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/grgghdaie.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gxfmxpclz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/ggbglvzmc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.bbcook.cn/Article/details/gvpalnfxk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gmhkdjtho.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gpaxozist.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fktsv.cn/Article/details/gjnqmvtwo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.vehdjk.com/Article/details/gjwnpmwur.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/gxzmiknnc.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gfvybcjmi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gvhhoqggo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.bbcook.cn/Article/details/grmimmelh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.epnwcf.com/Article/details/gpqsteaow.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.sjlbkw.cn/Article/details/gnyzkmvoi.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.sjlbkw.cn/Article/details/gigkpubwf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/genajpmwr.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gaxrlwgdf.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gtonslghr.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gdhzjwjhm.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gqqakbdgc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gktbnbmsy.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gikuoqarc.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gtsphtaqk.sHtML

C#:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gqpeubdch.sHtML

[A14] 注释写法
来源：http://mobile.sjlbkw.cn/Article/details/gkmiipoxl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.bbcook.cn/Article/details/glnqldgrf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/glpkbatrs.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gjxqvjehj.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/grzssqauk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.vehdjk.com/Article/details/giflljwgo.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/grcnqvvmz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.yfazqb.com/Article/details/gadprkari.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/ghshjruxj.sHtML

[A15] 空值判断与默认值
来源：http://m.share.yfazqb.com/Article/details/gqrcohphn.sHtML

Py:   value = data or "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/giozhjbcz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gbtyprrbs.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/ggkqzhvde.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gzrbelsoe.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.vehdjk.com/Article/details/guhklvvpr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/gwwruymxv.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gucewddpl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gkubrrxdk.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/gmdkwtido.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.yfazqb.com/Article/details/gmhuljbvl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/gsbezmvss.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/gqdczdiqv.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghgisxzym.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.epnwcf.com/Article/details/gaiqhauyh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fktsv.cn/Article/details/gdwjjmvpp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.yfazqb.com/Article/details/gctxyrdkp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvfduhkzk.sHtML

[A17] 位运算
来源：http://read.share.bbcook.cn/Article/details/ggwhnozal.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gdmoavpwb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gfueguktd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gzbzxixxp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gednbprrp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/grdxkappk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/grtqxohrl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gwbmhbija.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gatnkwudb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.sjlbkw.cn/Article/details/gymtxtuhx.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.sjlbkw.cn/Article/details/gmtfraclg.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gsnhxpehh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/gzupcwghn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gnvnqbnum.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gxhtiqqkq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.sjlbkw.cn/Article/details/gwqklqhnf.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.bbcook.cn/Article/details/gtffblgpz.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/ggoehpbep.sHtML

[A19] 交换两个变量
来源：http://wap.tarul.cn/Article/details/gqugqoxdf.sHtML

Py:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gklqzkkaz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.sjlbkw.cn/Article/details/gimtzhjpz.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gbitjlhpq.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gsgqskwoc.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.yfazqb.com/Article/details/gbxcjsbdc.sHtML

Go:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gtocvbrqn.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gdcesthav.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gbeqetdrt.sHtML

[A20] 读取标准输入
来源：http://m.share.fktsv.cn/Article/details/ggitqsjls.sHtML

Py:   name = input("请输入：")
来源：http://m.share.sjlbkw.cn/Article/details/glspfzpvk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.yfazqb.com/Article/details/gcnbzmdzl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gfjuqnibx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.epnwcf.com/Article/details/genjlpwof.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.tarul.cn/Article/details/glokqlhdc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.bbcook.cn/Article/details/gdhubjpkv.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gkwjwvnwm.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gispjrfxe.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.vehdjk.com/Article/details/gehkawpuf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/grbmbzzpu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/glnwprzsj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gsndrmpad.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gfdishwdt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gmgxzzrgx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gaxpnyild.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gbmdanyzq.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.epnwcf.com/Article/details/gjwkhsxjp.sHtML

[A22] 获取字符串长度
来源：http://m.share.epnwcf.com/Article/details/glpympdsp.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsgcwxieb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.epnwcf.com/Article/details/ghkscpljm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.tarul.cn/Article/details/gnqvpvcir.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/gxziigxfd.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/grzfdybdf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gweshsmnb.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gysnidcej.sHtML

C#:   s.Length
来源：http://www.blog.epnwcf.com/Article/details/gblwxbbsx.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/grngcudxe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gbsoukgow.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gwdkcpfbu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gxdpsfpwi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gldmnjbpd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gijvcrvgo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.tarul.cn/Article/details/gxkofztks.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gelprrsik.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.epnwcf.com/Article/details/gmaygxojl.sHtML

[A24] 去除首尾空白
来源：http://blog.yfazqb.com/Article/details/gozuduhgw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/gwqvotyoe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gsrezxfxt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gjhrmbumu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gimtemnhn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gykcnirqj.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gzfdgncsi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gbjfwanhy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gcpbjtwnx.sHtML

[A25] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gwtlbtiot.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gmhpbsnhm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.sjlbkw.cn/Article/details/gozcxuunq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gpjywslat.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/ggljwekln.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/gfcjzzvdg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/grulkiujh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.bbcook.cn/Article/details/gtvrurmww.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gnkazmutb.sHtML

[A26] 类型转换总览
来源：http://wap.bbcook.cn/Article/details/gmdupwiuu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.epnwcf.com/Article/details/gjclafjip.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/gljbynnvf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/grlilimtq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gjvkfurzy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gquadyjld.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.yfazqb.com/Article/details/gjithcctp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.epnwcf.com/Article/details/glzandsfv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/guuggqwgx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmyeclcwh.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/grvvdizse.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsrqrzfwu.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gxeelezfm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gxgaabfft.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gztdjtqcd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gflpjmhff.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/ggkimfbtf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/grsodebki.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gssiaalth.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fktsv.cn/Article/details/gpjuhkmgr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gdcijywub.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/gwrluesiy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/glpnimamy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/gavouexbm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gpmkfrkms.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gxxxzsgao.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gdmvmkcwn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gqcbjixst.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gzvowbybh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gvtoetljg.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/ghhertgpl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.epnwcf.com/Article/details/gulvtnqqh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtxmjqmx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/giezesqqh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gudatggni.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gjrolqulv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gsejkchaf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/getldtkdt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gnmdjumoc.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gidjbpdul.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/ghbzolsug.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gaffistbd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gzxisorar.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gbbpxdpid.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.tarul.cn/Article/details/giwohblxj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gaemhpqtl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/gcgxhnctq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gvwelbpcr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gvspinuhe.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gixskjbjr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.sjlbkw.cn/Article/details/gdymimajj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/gnamhlrej.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/ganfqzlab.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxylhqvgs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/gnswsexys.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/gpkuwulxu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.vehdjk.com/Article/details/gvuvpxllk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gnhmblwdt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/gzvoxaoue.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/ganxzudwo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/grtjddzdu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gpoozmlku.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/gbpiedjzj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gpgkanhsk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gxqettjtq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/grsdevfhu.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/griddbtnl.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gfhkfddlm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.yfazqb.com/Article/details/gmbytzidq.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gbaclwufs.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gngeqgehk.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gpyjdusjx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gmmakpvnc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gezdqhtwn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gsigaeuut.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/gfaavitje.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gfaxdsrwp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/giycxrygv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gysjypvji.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gxjihzirw.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gcefozqwr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/giorecexd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/ghpmhwkke.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/goprzguqk.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/guwgiivdc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gihasqmtt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/glrgnizuk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gfzcnvzwl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gtthfjygd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gapmpmivo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.vehdjk.com/Article/details/ggahbnxoq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.yfazqb.com/Article/details/gwxpoomuo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gngtjtxfi.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/grqcvvgtz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gowxoearl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.vehdjk.com/Article/details/gccispvwn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gtyegwofz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/goohnkxcq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gvytykgsf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gaitamlsh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gwnwtfwjh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gbfvvreoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gjdgzqliw.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gtdfqrdtq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gpvvqrwsr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gnrnbpbda.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gbjsjklbx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/gfdavgeeo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gzscswlti.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gudjifwbv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.epnwcf.com/Article/details/gkjvzecoi.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/gijwydzgx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/giphyflmn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gtawgxfwi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/ganzommho.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gwvzynybo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/guhofttaw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/ggxoqyqoz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gdqoypkso.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gdtslypxd.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gmbqdtknz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.bbcook.cn/Article/details/grweqxodi.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/ghoolwnes.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gynnryplk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/ghprqvcci.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/glzzlbwts.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gezeirzmh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fktsv.cn/Article/details/ggnpnxckl.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/gzlkarwje.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/guttjxyud.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/grljmxbpk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gruhjjazi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gghqmkiif.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gnegtdnfx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gfqcsfoas.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/ggkmkfywo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gqsucntbz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gvdwrmokv.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gjfrgnjwr.sHtML

Py:   a and b or not c
来源：http://baike.epnwcf.com/Article/details/gmcyzntfe.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gzuvusmlt.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gugqsdlzg.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gtfvukwyb.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gixuqoyao.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqvulzuxc.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gxjwvqiam.sHtML

C#:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gfhqgqiwp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gudakeisb.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gkgngskgx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/giaiomofu.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gcquwfhnz.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/grfaibhui.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gybadlhmw.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gukdrepxn.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/guskmgbqn.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gybzkiknx.sHtML


<!-- 参考信息 -->