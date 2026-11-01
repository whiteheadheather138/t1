代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gafbekqef.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/grpxslxpj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/glqwfsbmm.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gqynmjyij.sHtML

[A22] 获取字符串长度
来源：http://blog.bbcook.cn/Article/details/gidflxhug.sHtML

Py:   len(s)
来源：http://baike.bbcook.cn/Article/details/gsosqdzwd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.tarul.cn/Article/details/gaemxytsa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.yfazqb.com/Article/details/gycxtkmic.sHtML

TS:   s.length
来源：http://baike.epnwcf.com/Article/details/gaxoqqczm.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/gfwysaedf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gfcqnmxcg.sHtML

Ruby: s.length
来源：http://baike.bbcook.cn/Article/details/gwuqdcpxy.sHtML

C#:   s.Length
来源：http://baike.vehdjk.com/Article/details/gtltswaki.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gsloayogw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gwcjgpfan.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyuchavg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gzevqnnfr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gwouttmlz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gdfjcmvyi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/gsmibnfxa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gzsltjdyv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fktsv.cn/Article/details/gprfsixep.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.epnwcf.com/Article/details/gdhacqkri.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gbytxjznm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/ghjsvkcia.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gbqojzwpv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhuayzxk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fktsv.cn/Article/details/gdrxsrahj.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/ghaflwmxq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/gnordtudk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/gvspqqvnf.sHtML

[A25] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gzsnetijv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/giztpxpmb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/gldbyzzzp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gbedboocy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gfflrwepn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.vehdjk.com/Article/details/gfwlrhrhk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gzmibzpcd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.yfazqb.com/Article/details/gehufdvub.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gndqmwbwx.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/gueqwttpx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.vehdjk.com/Article/details/gqfoozxzj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gbyjbjrsp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gqazaztrg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gqtvotlwq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gedaolsad.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.vehdjk.com/Article/details/gudwfpwkv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gnolwbeak.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gtallmveq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggbniaqru.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gygqnrsob.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaqrnhszo.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gqpflixxy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.bbcook.cn/Article/details/gsuukhaxl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gafmwybeb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gxxqvjjdt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gwqnuejps.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gdjkldboa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gpwifjsqj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gfqokysls.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gybynckgu.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/gvckbtysq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnswvkxsa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gzozhhcwz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gieuivsxk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/ghxxbiwvd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gnphbfbdo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fktsv.cn/Article/details/gyoaomepa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/grsyabvhx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gfkqoipcf.sHtML

[B03] switch / match / case
来源：http://www.share.epnwcf.com/Article/details/giaatjwln.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/giembkeob.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/grtyveofr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gcysruaej.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/grmatepuh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gfdvuyiiw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gvzoaawlm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/gegfabstt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gwfjnwazl.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gnbjfvuyq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/ggpcjuazx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/gzqgeajzx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gbailhluu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gakpxyuqf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gtygewthf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/gtxeizswh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/gptorfnbw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/gsvmbvacx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gwvmsvtkv.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/grrdeapag.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/gqzprnyye.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gvxspcswe.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gycvmfapn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gkyoprtje.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/gykbmybzx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fktsv.cn/Article/details/gbfsswdqy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gyasmvmcj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.sjlbkw.cn/Article/details/ghuaqgvqa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/glrmlbtul.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/goatruuxq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gkwbmwoan.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gzfnuxufn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gqjsqsrqz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gnxxcqcet.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gkrwgxauh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.bbcook.cn/Article/details/gocarxcpf.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gvcaynwii.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/glzwbhcws.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.sjlbkw.cn/Article/details/grcnkzvmv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gigqwttiv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gkiplblcy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gnmrjiahs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gywmlobsq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/ggkrnwtht.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gnofethyn.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gaeradcut.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gflvhqsty.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fktsv.cn/Article/details/gqwcxxumb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gojmslweq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gfznqqdrv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gysxjjwfi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gruhguvlr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gcqezkkme.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gyrykdlvd.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gawhafxsi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/geqeirnnq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gnzbyeses.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gblqpmnnk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gygufvrkd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gprjuvqci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gxdcllgew.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fktsv.cn/Article/details/gjszuugjm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gizvujbnx.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gakvgjkfq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gfdewonsg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/grlgswtal.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gjiftezyb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gkytpaxlp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gsosgbpdo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gxpmowrja.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gyusohcal.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gwwwywvba.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gikpsaqoh.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gafocwjyr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/gftuficcz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gmefyaddb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/godrltbch.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/gycbioaiu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gjvnzajps.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.tarul.cn/Article/details/golzbzwtt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gsxaupnkl.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gukzaxjfv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/gqqhaijwk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/ggyyqlscy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gkpsgmino.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/grxzzqlpq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gtntstemk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/glqksrdgy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/gghvdooqt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gbzgdxvxg.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gowsgshra.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gouqnfjak.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/guzmcotra.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gvkdiwqgu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gusrtclor.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/ggxnyhzwa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gcaavaije.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gljfutipc.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gafxzbzbg.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/ghfokhtts.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gagaaipss.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gwrrnqojy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gcxcysdzd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuxwcora.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gtiizsbqo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gfayxyorz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gjwaturjp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gwotsgbav.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gqbeysepi.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gyhzdbgmw.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gfcfzcfcn.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/ghlkgjljb.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gozdbgiwx.sHtML

Java: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gllfcfiep.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gexxvedjf.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gbcflmbdd.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gtvrycpwg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gleccurwy.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gqilpeiof.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/ginrnwdhs.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gprluyvur.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/ghnxvxbur.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gcohcmqgr.sHtML

Go:   if data == nil { return }
来源：http://read.share.bbcook.cn/Article/details/gmhughljm.sHtML

Ruby: return if data.nil?
来源：http://m.share.sjlbkw.cn/Article/details/gakhdatkh.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gvqswdhar.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gonzdnuwc.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/ggwzlswdc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/goeugsebk.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gnpwxhyww.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gacybuqvx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/giykmnylg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gnxxudped.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gcugatati.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/guuonubgw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gtjfslkuv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gcchvvhdo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gklqcstce.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gcurxykco.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gfncfcnxh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gendfptiw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzfgeioln.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gnvclgcno.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gcnerzggg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/ghcjnzqdx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/guggwtjlk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/gkihcbmrg.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gjpquugaz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/gstqzwvth.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gyvpwyykp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gricdetkg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gnyhmdpnz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gtzwhwbef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/ghyefsjqu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/grqxrswox.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gdknwuoen.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/garuvekid.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/giuhvpnty.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gyplbvwhk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gfsqfqkvz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/guzrendeg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gciihhbuk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/geujdaojm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/garzdjzui.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gsyffjfcd.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gslxdpdfz.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gtpwrsgfp.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gbztcfryh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gxlmdclvi.sHtML

TS:   return { a, b };
来源：http://wap.yfazqb.com/Article/details/gisyrctyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/glzspedqv.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/gbnnxcndr.sHtML

Ruby: return a, b
来源：http://m.share.tarul.cn/Article/details/gnwgmbcbe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gdbqdpwbl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/grimgqmfo.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gevtuakvn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gyuzgerlo.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gqemnzeek.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gjebmxqrg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gcdweyjdo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/gbvfwkfqi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gdbuxfcou.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gxsmrlakt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gtslrzkmf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gcrexogic.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.bbcook.cn/Article/details/gnnkmfuzl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gtvexbdcq.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gcpvchuvg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gdzkuswzq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gjpdxvxnj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gfxztupcp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gdyzuappf.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gaxvgsvda.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.bbcook.cn/Article/details/gphkpjihf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/gqmjheuga.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gmjaxxejv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gajkxfivs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.yfazqb.com/Article/details/gukbxdoqt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gyuaxkqfd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/golzazohx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/grzbyhgew.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gxtqwvnpg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gcjpmsdfe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gyevtitvt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gjqaadwtr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gyyjskjyy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gmsqkbvvb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/gsluagfzb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gshhirtdw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/guxqidglo.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/grvbtcmra.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gppnzpuaf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gwsstwhui.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/guoevydnc.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gqzgjnlpw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gwqkjwywk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.tarul.cn/Article/details/gyvwonwcb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gvwqzvwnj.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gytqlkufx.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gkdktmxan.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/glayworkz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gvfrncsgf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gbifzzouv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/givrcyddr.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/grufpraee.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gxzfqkvwi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gxxepabar.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gttdzusdz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/ggiiuookn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gujzaiukh.sHtML


<!-- 参考信息 -->