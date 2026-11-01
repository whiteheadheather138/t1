代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/gqppxephl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gcofkzmon.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gbovpndhu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gohejxodi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/glhzfcqye.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gdjuhvbrg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gubgsnkdu.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gxmywttgb.sHtML

[A22] 获取字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gkpfoynao.sHtML

Py:   len(s)
来源：http://3g.fktsv.cn/Article/details/grknwknom.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gsepsbqsx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.bbcook.cn/Article/details/gybrkqizu.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/geemoqslh.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gxdoxwgjv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gjaaawzfe.sHtML

Ruby: s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gxkmgyqpn.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/glwkviyvd.sHtML

[A23] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gztazubec.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/ggtezyetg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.vehdjk.com/Article/details/gdggbuqqe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gqbfuxols.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/guofynpbp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gjckfigbm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fktsv.cn/Article/details/gmnaagldw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gymmrwiiq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gmzchcpvw.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gwtesqnah.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fktsv.cn/Article/details/gbeuueerr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gzguvcrxn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/guqofkjwn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/godzdjtwl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/gecplzqju.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/gzshkgwbc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gzmyslqyx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fktsv.cn/Article/details/gbfadwcrj.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gobbcpyxw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gwglxsvia.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/gfoaqiddr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gzhpykcgo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhlmktro.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.yfazqb.com/Article/details/gaidcjqsq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/goskonpvh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gatvuimtc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/goozedjit.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gcwcorkgb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.epnwcf.com/Article/details/gqadrjnti.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.tarul.cn/Article/details/gfvchrsrs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gbufwdkge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.vehdjk.com/Article/details/gpnqgikxd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gvwnkxmmu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/ggvpvqdac.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/geutzeizl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.tarul.cn/Article/details/gslviwyxn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxtgzmnly.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gtjobyzcv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghimseiut.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gjxbbpgcz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gdnjsiwlt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.yfazqb.com/Article/details/glpvmueiq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gscowirgu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gufjboioz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gffcshqph.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gdecqdjnd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.sjlbkw.cn/Article/details/ggihjfszk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gkqhzocqv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gwcrcponz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gigfwwzsj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fktsv.cn/Article/details/ghpmuxoig.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gijhehkfz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gyrpernwd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/guhnitvqp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gtrdprrkg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.tarul.cn/Article/details/gnqurvrpr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gvmrphxig.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/gjbehusja.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gwhsyjyio.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gxcmgxlsj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gjdgjxwnu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gokpxcjnu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/grianrglo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gnxdfcbrm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/gbhlmpkzc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.vehdjk.com/Article/details/ghydxmoms.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/guzbdkclj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gbrobowqf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gqxbvjtou.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gooejhvgh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gotxjgawf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gnitdvdev.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/gkjwatrvl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/gvuoxramt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gpdnhmhnp.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gubrzqpzd.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/goyuwackf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gykezjylk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gcujavbpk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/grmzuggpp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gcwroceoe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.sjlbkw.cn/Article/details/gphdrhqlo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.bbcook.cn/Article/details/gkpylsmjn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.epnwcf.com/Article/details/gncgzgacz.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.bbcook.cn/Article/details/gpfpxccsi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/ggxcyboeu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gfmlyhlij.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gqksadlgh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gzvigkoki.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/grpvgijaz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gexecejeq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fktsv.cn/Article/details/ghzfknfhj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gjnbaltrz.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/gjsrvjdlz.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gnhcqscdi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gqscmcgwq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gkxdcvfem.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/glkbfledc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/grnvknkgz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gpylfvqeb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gypvkyfwt.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gmwarzlns.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/gkgnhmjff.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/gkhlpucrb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gebqfmrzh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gkzmkqvun.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gpedonqwq.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gkwfljixf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fktsv.cn/Article/details/gcqxjiddp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gikhnjkew.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gpddpznhk.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/grrmdkzyc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.epnwcf.com/Article/details/gfucuzlnx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gtkpwvrvz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gzpojiwni.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gewrkyufg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/giblzktol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gmydbonfq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.yfazqb.com/Article/details/gxmpdafvh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gqaguirvy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/gimgqmtfr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gkzftgtnv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gvipslqrd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/giblkehhe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gypctjjnm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fktsv.cn/Article/details/gkfgvijzt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gswlmqrgs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/gljyfcqap.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/grryhuykq.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gbxjzdpuk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gquavyrzw.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/gxybwtuof.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/grqjfxeek.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/godyyatzk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gcngcobwl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gmdsethwx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gjljfpfuo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gvyhwsjvk.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gckweqswh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gogrhlvbl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gbeyplnhe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gyvphwndp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/ghjgyykzn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gpsubhozv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gdsintacm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gumsbjadw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gdmxpfmdl.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gwgolifvw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gzscrgtqd.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/ggiqtrifn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gykjtqvsy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gfwuaytqm.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gayqfffkp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/gzcvncgks.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/gpkbskass.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gfibxmcso.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.vehdjk.com/Article/details/gnmdcwakc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/ghpelucby.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gzpproiyz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/geudpssog.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gqxfviywh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.yfazqb.com/Article/details/gfdmnfhoq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.yfazqb.com/Article/details/gahfbjybp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gqpsqnhgi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gsvwfeyxr.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gwalzkhfn.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/garybyhop.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gafxtrnue.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/ghrfzegxi.sHtML

TS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gdibkjddc.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gpixctuxl.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gbxrtjhlp.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/glhkttami.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gfaarlvau.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gamjvqcjv.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/ggwurtcqa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/guznjsxcc.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gzfrcfcrg.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/glyoyfzts.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gpbdeabwe.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gsmvdisyq.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/goppwdizh.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gmszwrdpy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwcmjylwm.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/glibyczpa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glsoopuqe.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gkuedhwhf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gljkpnzzd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gylgkilpi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gldesjzon.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gtfptcsad.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/guytjkqkq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/goscujiiq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.sjlbkw.cn/Article/details/geoipqiih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gjqjzyxra.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/gtaivqesz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gcfkmwfjx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gfucdafwx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gqqxzhauc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gkmczsbsg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gyyukqeea.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gdwsmjpmw.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gzntxdsao.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gatzgxugs.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gwgvladpj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/gbugggjqu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gawpibtdh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gccntythg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gxzbctpnh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gksygrviu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gpcfmgbxt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/ggvqpyhrs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gbkrgpywz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gibsilhoe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gaamcggay.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/gclrtabyr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gctnljqqj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gspzcprgd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.epnwcf.com/Article/details/gvfftbnox.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gzaiclmim.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/ghmepwont.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/ggygjtbgx.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gzwzutbaa.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gfoufmrus.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gqhycblvv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.tarul.cn/Article/details/gjcfjxzyo.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gdzodypit.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gcghprayl.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gwdkuwcuk.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gkuczrtmz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/geuyknuin.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gywpkntwf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gtsgvokwv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/gryvrwvov.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gpidersce.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gyckfjeuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/gfqokmfwi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gaofjwbff.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gwspmoruw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gxsscfnul.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gmxxpgnpo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/grhhvadav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gzwoqrfgl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gvycbrhir.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gfrxprzca.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gajgitljr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.bbcook.cn/Article/details/gnqvcxpxf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/gwzdaidhg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/grbrtnaef.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/gklhcviyl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/gxevckdxy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gpkmupwcp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/ggouoehpc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/getxykcjo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gyrljedlo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gsgnfbdge.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/gvkchgmpc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gmpkveujb.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gacmpsxkw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gssxpphyf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gdlbhvgmn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gruzbqyzo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gocntscxc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/ggkxcxkhn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/gyrcavobj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gujwhnpfu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gncojtpsa.sHtML

[C10] 变量作用域
来源：http://3g.epnwcf.com/Article/details/gtcfkjgie.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gyvosmaeg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gbxwcmghj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gdncttirf.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/ggkbqabmm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gjmintylw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gzavqrftm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gigvfoioc.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/ghphjepau.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gapdfskya.sHtML

Py:   from module import func
来源：http://www.blog.tarul.cn/Article/details/gcsncjqxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gsnzguort.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/giomfmvpd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gjxktgojf.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gjwxeblzc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gdkprxjkr.sHtML


<!-- 参考信息 -->