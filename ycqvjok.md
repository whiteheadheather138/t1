代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/glsrtspcr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gbxubmbob.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gmusxcwhe.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/grtrrqkyb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/gxxfhdiys.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gixerbqpb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/gjyhzolca.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gzzujbfuh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gzrwnmjyc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.yfazqb.com/Article/details/gmbxnwmsw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.bbcook.cn/Article/details/gzmcrznap.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.tarul.cn/Article/details/gygezmdze.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.tarul.cn/Article/details/gucfqmeyv.sHtML

[A19] 交换两个变量
来源：http://www.share.fktsv.cn/Article/details/ghquifyfh.sHtML

Py:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gtkvarszh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.vehdjk.com/Article/details/gzjqrjxve.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gavrifyqj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpfbpqaj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.yfazqb.com/Article/details/getvsiyih.sHtML

Go:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/goavswbwe.sHtML

Ruby: a, b = b, a
来源：http://wap.yfazqb.com/Article/details/ghnhcomix.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gkieffpcu.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gvknutijg.sHtML

Py:   name = input("请输入：")
来源：http://blog.bbcook.cn/Article/details/gnylqhebi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.epnwcf.com/Article/details/gfogwhxly.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.tarul.cn/Article/details/gwtunsqfx.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.tarul.cn/Article/details/gpoesvldx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fktsv.cn/Article/details/gjocytvnu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.tarul.cn/Article/details/gdghrwane.sHtML

Ruby: gets.chomp
来源：http://mobile.fktsv.cn/Article/details/gbkbbmknz.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/grcxgxdrf.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/glonphmct.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.yfazqb.com/Article/details/gbrdbaxjt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gqukmmfsa.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/ggzixkrgi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gsossdlyk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gjpqxqudj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gcyoawbzf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gfzczupsx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/gxhoqyumb.sHtML

[A22] 获取字符串长度
来源：http://www.share.fktsv.cn/Article/details/gswrpfpyq.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcvqudnhl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.sjlbkw.cn/Article/details/gprmeiiud.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.sjlbkw.cn/Article/details/gtmestrlj.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gbzgrrecf.sHtML

Java: s.length()
来源：http://baike.tarul.cn/Article/details/gybrxbztu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.epnwcf.com/Article/details/gnzgeyppo.sHtML

Ruby: s.length
来源：http://mobile.tarul.cn/Article/details/gcncvrkya.sHtML

C#:   s.Length
来源：http://wap.epnwcf.com/Article/details/gajcsinmf.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gbuflduoe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gndnqkqms.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gzkfkvcdr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gyilecaqu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gksgnjvul.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gnpxcunsg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.epnwcf.com/Article/details/gvybplxkc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/glkgxrwop.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.yfazqb.com/Article/details/gylntqjag.sHtML

[A24] 去除首尾空白
来源：http://3g.fktsv.cn/Article/details/gyspuwqjw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/gmiphfgox.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.epnwcf.com/Article/details/gqoppqcth.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gzaaiuizq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gntkxlasj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fktsv.cn/Article/details/gwtmvvpxl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/gupetoaal.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/garhxmcma.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.bbcook.cn/Article/details/gknecxhbo.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/goixtattx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gluwbzhmm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/gqxawncwm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gfvhbicma.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gskcgvayn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/gyrfjflsv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gwfnrqyte.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gqwwqntch.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gfigwnidq.sHtML

[A26] 类型转换总览
来源：http://mobile.fktsv.cn/Article/details/grovxcmoh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.tarul.cn/Article/details/gpgapkiuc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gtnhbxsnt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gwkkoyhis.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gulzhrxuw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gxdblhuec.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.vehdjk.com/Article/details/gxasgvgqu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.bbcook.cn/Article/details/grliyjmfb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gylahlezt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwqcixsft.sHtML

B. 流程控制
来源：http://www.m.share.yfazqb.com/Article/details/gbaqdgmph.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvwzfnozo.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gieprakdy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fktsv.cn/Article/details/ggnxwgrfc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gfydgukaf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gfwdzvfvw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gfqwvblpy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gqrrrduhv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.sjlbkw.cn/Article/details/gaowllvpr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gmlqvizxs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gtrtsabbm.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/goyslikfx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gkozzabvr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmdynaxqc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gmdyqiddq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gkmnktcpm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/goaecixdv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/gjgeaolvu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fktsv.cn/Article/details/gwbpzsaeb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gygzyewxg.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gztkcchzt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.sjlbkw.cn/Article/details/gxivdxmon.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gyjxjqkjt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gdxyubbik.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gnilfeggi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gcpewionx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gbdqgrwbn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/gbwrdgpwg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/ggasmgjnl.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gortpayau.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.epnwcf.com/Article/details/gpgxudmml.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gtbgyzdmw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gaqocdols.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gftebpuow.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/ggcdpfhnv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.yfazqb.com/Article/details/glglrytmd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.vehdjk.com/Article/details/guxdfqqbz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gezlsnusi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gtusegyzt.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/gstdkebqc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gjhkbkepo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gqgjunyag.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gnlpiorda.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gtfqxptqs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/ghqyibtbv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gmbjvoisv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gfsdrgzbc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/gippoqutc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gumxzprly.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gnrcbqzsy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/ggsaofypo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gbeinfxan.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gqpqdcerf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gpqtwnadp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gxolwhsmp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/gegvlbomf.sHtML

[B07] while 循环
来源：http://baike.epnwcf.com/Article/details/gxvisecon.sHtML

Py:   while i < 10: i += 1
来源：http://wap.vehdjk.com/Article/details/gidvfoapu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gvadjvyfd.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gmbzypzlc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gmgqbdptv.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gwafumdzo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/gukwayhct.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gddeeuxgt.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/ghrwvytrf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/gjwzejwwf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/galilftmq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fktsv.cn/Article/details/gzopnjito.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gjcsgrnqp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/geqwovmnc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gixadlswd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gcqwcrkyc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gvtbeuwkk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gsizjdhgi.sHtML

[B09] break 与 continue
来源：http://3g.tarul.cn/Article/details/gedwpulvx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.bbcook.cn/Article/details/gytrabkqh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/ggoutoyty.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gwhwpffzt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gpyjjvmps.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gxizjtexw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gkzgxtqfa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/glwdztxzr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gokbfghrr.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/gcpbzkwni.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gjqmeqsmu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gzfozxorl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gjargolli.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gfhtbysvh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gjojhukux.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/ginsxuwgj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/gitnlopzq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gorxwbhnl.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/gnvvnnoym.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gibwaqwtp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gjvvltutj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gvkshcsfi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gqwxyawmg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.tarul.cn/Article/details/gzovnuvdq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.yfazqb.com/Article/details/gmmmgnxdt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gohnchcwp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gqcxsnihi.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/gaakxgjcb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gnalvicay.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/gwhaeensz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gznrlxsws.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gbagvlomj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/ghrnqiadr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gmharsfiy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.tarul.cn/Article/details/glfphscop.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gviofzrhz.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gwzmypmpu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gtslpdojd.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gwczsubob.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gjplgzjcu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/grxwawodm.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gsrgguxzj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.yfazqb.com/Article/details/gpcnifghs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gfqnfnfls.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gulrevutv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gctssjabz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gfniehkpf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gmlthofot.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbhidmsld.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqavdafiz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkuqlmjjg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gragohsgj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gaknypgrr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gsxwvddiv.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/gigzomzan.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gxhhcdclh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/guhaieafy.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gycgiubmx.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gurrlckef.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gwxvjcdta.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/glmfxzmpm.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gxgdztomc.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gokekwnrt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/geybhgfxq.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/glyyccgjv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gfaajzpvy.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gynidhpdw.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gcoskeemq.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gxcroifor.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gqfqniodf.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gkgmjuygj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gvifgeaqv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdncfolqw.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gnbshaotw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghefcpnlu.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/geiznfhqh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gwkekgfah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gyjwjdakz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gddxoweqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gidgmjiwz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gihlvmhlo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gqtpcxlfz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/ggebvvyjk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gcbnovdgu.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gtuwizejm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gaoewyjce.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/gbsvggiah.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gstaknwbt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gcrcwtjtq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gduvcamli.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/gkirvpwpv.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gjwslokaj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gfjojfktn.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gwoiurfnz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gnfssiykr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gjdbxwkti.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gtdkceksw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gewynbhrf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gmbcrhbkt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/ghzldrdtb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/ghrjvpznn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.epnwcf.com/Article/details/gljxvruou.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gjvrqzbhu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/ghxvormtj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/gavzqzwnh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gutdwumsk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/glgfipjjj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gpkyuuatc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/ggntaenjb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/guutgufai.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/glddptund.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/ghwdtooeq.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gdodledxs.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gcaexyshe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gphgxpkuv.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gaaiwrufu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gvvomslxl.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/grxnflrkp.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gjtszcafk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gqknjmcnl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gqcxyewsm.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gyjulvhvo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gvkmdvxwk.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gsodywnek.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/ggiiznfnb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gqqocftgg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/ghpzlhdzv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/gdgkdzfls.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gsoeclmvb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/gmdmrcicy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gmtpayzpo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/gzkecfojk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gagfrpvph.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gzitmihvk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gtmavttrr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.tarul.cn/Article/details/gwhnfammi.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/gatjerbpd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gfedtegsk.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/ghcqxiwcq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/gcforujvv.sHtML


<!-- 参考信息 -->