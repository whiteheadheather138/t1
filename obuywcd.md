代发 wailian999

Ruby: a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/glybkrtru.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.sjlbkw.cn/Article/details/gttvqzvjt.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/gpewjkquq.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gcmnuuhib.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fktsv.cn/Article/details/gdsueljut.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.epnwcf.com/Article/details/guamblpod.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.yfazqb.com/Article/details/gduodvvlo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fktsv.cn/Article/details/gvweoquzu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/gbwrjmwmq.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gotekhwbz.sHtML

C#:   Console.ReadLine();
来源：http://m.share.vehdjk.com/Article/details/gneghecyr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.tarul.cn/Article/details/gogglgkqv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.yfazqb.com/Article/details/gnovykmby.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gaxmjppwb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gzycaephj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gcuzdjyxf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/goezilqsd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/geouxsvis.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gutybenxc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/giiezgmos.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gsseeqdtp.sHtML

Py:   len(s)
来源：http://www.blog.tarul.cn/Article/details/glusoneud.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/gwygaegxl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fktsv.cn/Article/details/goznhpsxg.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/grsubwlcp.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/ginuztevx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.epnwcf.com/Article/details/gkqnpsqjq.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/grkwodymp.sHtML

C#:   s.Length
来源：http://www.share.tarul.cn/Article/details/gtsfdgnte.sHtML

[A23] 大小写转换
来源：http://3g.tarul.cn/Article/details/gdtoqrvvc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.sjlbkw.cn/Article/details/gcoqtdgsx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.vehdjk.com/Article/details/gaircmljh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/galnyober.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gfjhgyiev.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gkvavzhko.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/ggdxeghsp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.yfazqb.com/Article/details/gucfzewcf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.sjlbkw.cn/Article/details/gfwelbdpr.sHtML

[A24] 去除首尾空白
来源：http://wap.vehdjk.com/Article/details/gjrvdbcnt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.vehdjk.com/Article/details/gcmtoqxdh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gnznvukth.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gecafyjlx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/goaehgkaz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.sjlbkw.cn/Article/details/gejfjiplm.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/glrxsjxal.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gqdkhivej.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fktsv.cn/Article/details/gliytiuyp.sHtML

[A25] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gsjnpsymk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.vehdjk.com/Article/details/gqpnjqdjh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/giobchzsv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gxlrnlatn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gdqgaiivb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.yfazqb.com/Article/details/gjsbckbie.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gkgtbndie.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/glablpswd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gjcghjljf.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gkjokiocr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gbpykceoe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.yfazqb.com/Article/details/gwcswknsd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/guhuijlxa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/guraeeuuc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gvzaemndi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gmfauqnzy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gviitanwv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.tarul.cn/Article/details/gsigtmssg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gktbozoxm.sHtML

B. 流程控制
来源：http://mobile.fktsv.cn/Article/details/gcuckalzk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtrzdjwif.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fktsv.cn/Article/details/gpnsphdhk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.bbcook.cn/Article/details/gmyzkzhoh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.sjlbkw.cn/Article/details/gskmitwgc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/glgyxnejo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gbsxznjsb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gqvcykyhq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.vehdjk.com/Article/details/gombswhtt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gprypvoes.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gdhbgnhzz.sHtML

[B02] 多分支 else if / elif
来源：http://blog.yfazqb.com/Article/details/gyojlpjnz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gxfsfntaq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gzzmixgkt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gqlorqgpr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gynsatcai.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gamfzljbi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.yfazqb.com/Article/details/gegacmuob.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gmyhracmw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gssdxyeqr.sHtML

[B03] switch / match / case
来源：http://3g.yfazqb.com/Article/details/gkgkucfjy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/guyycpsyz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gvghjrdyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gzotqdcol.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gjdejzknn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gysgmrevj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gesscefrh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/gwyrktpnm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/ghlmjzjxo.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gpwhmjngr.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gisavnyca.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.epnwcf.com/Article/details/gsgtmtqrh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gmpgwwcuk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/ghbsqjeoy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/ghleknijh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/gmhlmvjtw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gsnqcecwb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gmarjmqbz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gvxlyhkhj.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gijzbpxhi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gymwllqhj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/gzwzxvtpn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gifljruty.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gzfqiples.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gxaxajjci.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gwnoaeemz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/gukiywkcy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/guufugczo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gqqqrirkm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.epnwcf.com/Article/details/gugeuheks.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gzvhnkkwq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gmcckpkli.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/ghvgbjtws.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gubmrsjxt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gbnzsvbjt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.yfazqb.com/Article/details/gpenpifjq.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gorqntfyq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.yfazqb.com/Article/details/gfbkpwnvb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.sjlbkw.cn/Article/details/glsgfrtsr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gekhrcujm.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gizcwdmkf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gichocpyg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gugieschb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gemdqlknq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gjghoertm.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gsfhlgofz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.yfazqb.com/Article/details/guwxkvyer.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gfnubrggu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gihsoklen.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/ghwjhttos.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gnyukchmh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.tarul.cn/Article/details/gewqmhgwh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gjzqsirjb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gmtwyinhg.sHtML

[B09] break 与 continue
来源：http://mobile.yfazqb.com/Article/details/guwjhomfy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gafzvyrfr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ghguckbxv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gvzvucoov.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gnomtbncc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gubmwmqiy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gukkjurls.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gwqavwiip.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gxxivxokz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gjjpmeulk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gxuhlreuy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.epnwcf.com/Article/details/gdfxdfhem.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gcbgisreb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/glymnhrda.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.epnwcf.com/Article/details/gddvnvejr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gjtpqocnr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gxsepqrca.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gvwuxoaaq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gxcclncoo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gypsretue.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gmdqieqkp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gjyylscbr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/glynuzbdj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gwbwdkspl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gwskfhqva.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gkxdpxeke.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gopvgzsul.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/ghyncxlce.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/giouurugh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gdshfraxr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gslxemelv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gblmcyznm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gkylojpqh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gdftgqfco.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gpvfvugbz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gwwdrwjtb.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gpndepmwm.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gxxqjykzj.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gwdbfhjjg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/grwjjcdnj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gpdpjtbug.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gxqvghhvm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gnqzyuqeo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/gsuffiisx.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gugtdidzv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gpzavkrkn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gwvyvkdph.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gcygqgenb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gmfbwwaaf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gjyuflipn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gjpqrewal.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/geswedqnk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.epnwcf.com/Article/details/goxvaxpfq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gyeefrrzv.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gyyebenws.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/grvntlzpt.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gzarmhpkc.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gmfalhmit.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gwzlcawln.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gieisfdle.sHtML

Go:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/goreliohl.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gpaqikxcp.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gxmapqygk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gvfnguimy.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gvqaujawm.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gsdousbnq.sHtML

JS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gwnjhlmlk.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gtuvhwnlh.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gsisoghgm.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gvumjubck.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/giqkmpivf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gpmzipivd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmdajpteq.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gtagvsrgc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvkmsqmoe.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gzfdzxqgd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gylrwwjna.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/ggkhbohcb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gslorrkfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gnxmwpiiy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gcwmmasne.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/glmnchmha.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.bbcook.cn/Article/details/gmnjdxjet.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmvfzzusg.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gbfcxzcge.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gjpptsson.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gdftxbqqu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gkneifotw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gjhyoejxu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gxzringeh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gtrrfvslx.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gemnqxcir.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gcybeqebo.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/giyuxsxtz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.epnwcf.com/Article/details/gyqqdzqrs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gsteccwol.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/grmviivwt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/ggnshrfdg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gbpdakzcy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gdebfgiad.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/ghczytvix.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gczefxxyz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gsszvxudz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.yfazqb.com/Article/details/gcrsbxnvu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/ghqhbzbyf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gyybeovtk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/gsxrsyyux.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gcdtnpoid.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gcurwylkk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gldgtovzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gndgpxljj.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gztiywpjg.sHtML

Py:   return a, b
来源：http://wap.bbcook.cn/Article/details/gaorhdtvj.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/ghqrqnmls.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gxirlefwz.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gkwptjbdl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gidhrtvrq.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gvufufrqc.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gnphuffao.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gwqawstuv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.vehdjk.com/Article/details/gztjzajav.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/ggcfivgpg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gxnpevtos.sHtML

JS:   const square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gvpgfrwsp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gzzkursnn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gxsotetaa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gwwpvjmyd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/gyvhwkivl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gknvkplhk.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gfiuhomht.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/ghjfvdxyc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/gicgefokm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gyxyjatla.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/glnoibalp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/ggsbbgtju.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.tarul.cn/Article/details/ggxsdifot.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fktsv.cn/Article/details/gjltsfbui.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/geftkaphu.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gbkhntgll.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/govecqsfx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gqrfesjdt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gkgsigvag.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gmlgurkxk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gakhqdhzk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gdfgamvvv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gnglpctco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gxunceydy.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gyaedpcxm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gbzjqxtot.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gbbjiyhuc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gzsguuuvr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gspjfnaib.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gcvuullif.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gqjzmrgro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gryffbxvn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gsrxfpoks.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gputbphqp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/gvagmnoti.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gjupryrtg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gpacoozby.sHtML


<!-- 参考信息 -->