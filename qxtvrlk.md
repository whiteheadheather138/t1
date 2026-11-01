代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.bbcook.cn/Article/details/grgiywzkp.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/ghkftgcgq.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fktsv.cn/Article/details/gepkvrjyn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fktsv.cn/Article/details/ggyxigqre.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.yfazqb.com/Article/details/gycwglxul.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.epnwcf.com/Article/details/gscvrrssv.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fktsv.cn/Article/details/gfzynzfjd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.vehdjk.com/Article/details/gujcmmmud.sHtML

Py:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/giltwzulo.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gdwqwxbrn.sHtML

JS:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gwkrkqkgu.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/guyoapjpj.sHtML

Java: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gyblyhmiv.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gshriiahb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gkyaywkyu.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gjclobvua.sHtML

[A14] 注释写法
来源：http://www.share.bbcook.cn/Article/details/ghayxsscn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.bbcook.cn/Article/details/gzdlhzugx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gwtmduwpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gjqanunyt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gxzqlcxak.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/gupiromay.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gyjxpurjm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fktsv.cn/Article/details/ghfwesjei.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gtqvzlynt.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.epnwcf.com/Article/details/gsokyyizc.sHtML

Py:   value = data or "默认值"
来源：http://m.share.yfazqb.com/Article/details/gzbmbsacv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnymdutfv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gzjwpgroq.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gudbyebow.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/gidfxykfe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/gmiyzlmaj.sHtML

Ruby: value = data || "默认值"
来源：http://baike.bbcook.cn/Article/details/glbsdbbzp.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/ggdecjbge.sHtML

[A16] 真假值判断规则
来源：http://www.share.sjlbkw.cn/Article/details/gwhrofxkr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.vehdjk.com/Article/details/gzsnjyjwj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/gattseooi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.tarul.cn/Article/details/ggroynofd.sHtML

TS:   if (!x) {}
来源：http://mobile.epnwcf.com/Article/details/gjgabuool.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/gzajtyqxk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gffcjjvki.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.yfazqb.com/Article/details/geaxebmrw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsmebnfbk.sHtML

[A17] 位运算
来源：http://www.share.bbcook.cn/Article/details/gvypvyowg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/glzxmoxlr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.bbcook.cn/Article/details/gitjbxabe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gjeumyeug.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gduskpmwf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gnakiushq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/ghnmgavbp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gxuwsplxd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gtrnvskae.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com/Article/details/gwcwhyuyi.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gblgircgl.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gesunovyi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gfrvhwzfd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.tarul.cn/Article/details/gtoeqhytm.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.tarul.cn/Article/details/gfdrndyha.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fktsv.cn/Article/details/gicgyvilb.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.bbcook.cn/Article/details/ggkpuywsl.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.tarul.cn/Article/details/ghzzxvvta.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gfhoxqgpc.sHtML

Py:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gwdlculkn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.epnwcf.com/Article/details/gpdvkomvt.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.epnwcf.com/Article/details/gkodryzmu.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gvyikvifo.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.sjlbkw.cn/Article/details/gamcfcvfm.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gobkvuuhu.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gggtcsnjl.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.sjlbkw.cn/Article/details/gxihrmryt.sHtML

[A20] 读取标准输入
来源：http://baike.epnwcf.com/Article/details/ggehfwnag.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/gchunbwok.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.vehdjk.com/Article/details/grmxqpxeg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.yfazqb.com/Article/details/goxwsyogc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.tarul.cn/Article/details/gzxyzjdnm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.bbcook.cn/Article/details/ggctjwnlm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gddtbmiuu.sHtML

Ruby: gets.chomp
来源：http://blog.fktsv.cn/Article/details/gazlviyyj.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/gqoydjjmi.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.bbcook.cn/Article/details/gxrwlxffl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.sjlbkw.cn/Article/details/gfapwkecl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gukydkboy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gxmbwikmp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gdypyaboe.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/guzzfypni.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/geoqpctky.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gjnhmviff.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.vehdjk.com/Article/details/grscpeltj.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gmjgxyled.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/grszesesq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gcrjmufmf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fktsv.cn/Article/details/grnhawnit.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gypbykbzs.sHtML

Java: s.length()
来源：http://blog.vehdjk.com/Article/details/gsbbwdwcv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/ghftaqqgu.sHtML

Ruby: s.length
来源：http://mobile.vehdjk.com/Article/details/govvokxhp.sHtML

C#:   s.Length
来源：http://read.share.yfazqb.com/Article/details/gcshisavf.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gpotdawur.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gfposyepe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fktsv.cn/Article/details/grkjebvte.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/griywyhkv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gizwuzwtm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/ghtinkodq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/ggzzgyreh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gghpukwtf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fktsv.cn/Article/details/gtkruexhu.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gnudajhmb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/gkeabpvzo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/ghoutdzrf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gpjziwvns.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gtyapyuos.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.sjlbkw.cn/Article/details/gjokshirv.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fktsv.cn/Article/details/gcpjnttam.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/gwwogpawc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gtewrcxml.sHtML

[A25] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gmyuqmmyz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/gsamdfjfw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/goggjvhkf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/ghhcerkty.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gtzhvivjd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gbcpqihhm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/govrdlabg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gkqrnqiqp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gcecpnsfe.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/gpvoxptga.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gaqrecitq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/grkojacii.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gukmbdqzh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.epnwcf.com/Article/details/gvumtsvww.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/glanpyhad.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.vehdjk.com/Article/details/glhtbprrs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gjwvioblq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.vehdjk.com/Article/details/ggqsarjjr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxwolssaf.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/gesmepmdk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzhtfqfhd.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gsvybhjsp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/gkpaohkht.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.yfazqb.com/Article/details/gpzzcymsb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gkvtrxhai.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/ggssafhze.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/ggddyegme.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gagupxumd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/gwkrsfjpo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gukoecexo.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gychbybjd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/groyjxxwe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/guhbiqlag.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gtjyaqsxe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gvstkzngh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gobqeamje.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/grdtpggoz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.bbcook.cn/Article/details/gepyxbeve.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gaxtwwqjj.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/ghktnzjml.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/gkofffaky.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gectuqsff.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gyinuizdo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gezvihbho.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gdhwoayfo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gcutetmdv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gyhxeyqsa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/glkluasgt.sHtML

[B04] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gghhfubvx.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/gewprbgrx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.sjlbkw.cn/Article/details/gwcvvqhfe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gnqjzhnyg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gowzeyehm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gebcsbigk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gsbzhinxu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/ggaijmznl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/geqgbvtiu.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gcqpvwahv.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gqyyvoyil.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/gndjgcdmm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gfedvrtby.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gcfxfrxoy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gkzkarkqz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gqneooefh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gekpgltwm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gvvzzljzw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/gxkvzypuu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gwtnkofkc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gindqhzym.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gudhvfpmp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/giubwsefx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.tarul.cn/Article/details/gqklopalb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gmwcfytli.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gfgcdshwd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.epnwcf.com/Article/details/gigvyeupk.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gtvodpyeu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.vehdjk.com/Article/details/gymtyhpss.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.bbcook.cn/Article/details/gqdjcfpml.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gnehuiail.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grudrhuls.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gjrgqosto.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.vehdjk.com/Article/details/gazelepno.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gpikzrgeg.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gqazetqvs.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.tarul.cn/Article/details/gtzmtevep.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/gmrsarlbu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gaspkahsf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gmykdembd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gpqukwtdr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gpjxsnysb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.bbcook.cn/Article/details/gfcfenxqi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/grqrohrxo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gwaslmcff.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/gvalaymll.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gcbttuepr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gpzkyagfk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/ggnxrfvct.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gukzgyvxn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gzhhbiofi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/grkusmwwp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gseobopay.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gqzuvlcmw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/gradrqsbw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/ghwrfgecv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gljyhrsvs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gkozwhrjh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gdrahuoxu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/guzhquazw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gpugghfyh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gcoliqwdm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/gavvepunu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gmoxnwzxg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.yfazqb.com/Article/details/gsxnrjxlc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/gmrwaizct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gnbyxtkep.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/grvgfklpx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/ghkcfhjnj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/gczlrfshc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gsqbtuzdv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gnzmjwinh.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gdzluofdo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gbvqlqfki.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gvmdcefhr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gemoxkcgu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gsmlzyyiw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gchanirpf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gnbvqdgjq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gvbbmmobv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gdkbewyga.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/gxdsgodkj.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gbhhgdegu.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/gyujyuaiv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gfztvdzbr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/ganfhuott.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gorfobpzh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.vehdjk.com/Article/details/gsydstsmd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gaspvpdae.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gnfkfhwoa.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fktsv.cn/Article/details/gcjckzbct.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gfjmndgzh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.sjlbkw.cn/Article/details/gcfnvzjqx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/ggsahlxph.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gacraxqne.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.vehdjk.com/Article/details/gfeyauxte.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gilwxybvh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvznpufe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/glxzeyfms.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gigohhqmc.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/grxtoprvi.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gfaipeffo.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gtuhlvpnn.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gcrhzxncf.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/guwtvmzxk.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gaukjrqqu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwsjbvncb.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gxkyeppoa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/ggzkaltud.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gprjytbts.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/gctmflzit.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gbplshuvw.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gcphcfhxw.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gblxefcfl.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gganvjjtb.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gqenkmsil.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gyhwhgnwd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfaymtrfx.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gpadittbn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gevgppoce.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbalgzzg.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.bbcook.cn/Article/details/ghnojwdgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gcvutroat.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gudkcjcvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gcgfwmyar.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gvigfjoso.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gkoxucicp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gizgcktbc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gmalimjcq.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gxscnukem.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gwnpmnzfo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/glcvjefiv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gsivjjvjf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gnpwwydjn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gmuibgibw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gkpuysaxi.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gisfzdoqy.sHtML


<!-- 参考信息 -->