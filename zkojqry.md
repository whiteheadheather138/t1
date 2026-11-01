代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.epnwcf.com/Article/details/giowkqlsj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gskgxcevi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gmjiacotu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gaxxljyrc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/glsyuhxir.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gkgfprntw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gvcjxznxy.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.yfazqb.com/Article/details/gbfduutoc.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gofxijkzg.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/goirklova.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gwqyzfaxz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/gemddinmu.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/gjwmjvysu.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/guhkltbej.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gcjodbwqt.sHtML

Ruby: s.length
来源：http://www.share.yfazqb.com/Article/details/gatbdbtyn.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/gonnrdoyr.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gfgscbofb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gwecwjyie.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.tarul.cn/Article/details/gibngzopt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gzjbbjymq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/ggqqxdwde.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gbxzwidov.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/grytbxdqb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.bbcook.cn/Article/details/glbyeerld.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/gijonozge.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/gghbgviat.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fktsv.cn/Article/details/glydecclg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.sjlbkw.cn/Article/details/gazukguxp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gtoaivjhw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gfqjantkx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/gfcwqzagc.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fktsv.cn/Article/details/gbrvuzgnk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.epnwcf.com/Article/details/gezayvlro.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/gtbdmtavt.sHtML

[A25] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gdajibxbt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gmclkqgua.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gacwtsnkz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/ggtiypdlx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/ggdastrat.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gcfgdieew.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/gcfuiobru.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/grixtljcu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gjmytcaff.sHtML

[A26] 类型转换总览
来源：http://3g.tarul.cn/Article/details/gviibrrau.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaetyldzs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.sjlbkw.cn/Article/details/gnqhxmpkm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gpfdyhgdl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gagnkwzuy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gbcyrqlve.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gytngyicd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.tarul.cn/Article/details/grlgkidup.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gbwwyiqmn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqcfntple.sHtML

B. 流程控制
来源：http://baike.vehdjk.com/Article/details/grcspbats.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwlzwdvbj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.sjlbkw.cn/Article/details/gnwgjtftx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gpoqbxite.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.yfazqb.com/Article/details/gnsuzwcrl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbtqiyoj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gqkuvwsmz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/glzrytziw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gjekgyrpl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gnmkmhnks.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gvyowwsid.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gurnmwkhx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gvmkswbli.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gswxpctnf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gvftihtcp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/ghqtbycfw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gcnwsvevy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/gjlcmflwv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gtrmqkekm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gypwplrwv.sHtML

[B03] switch / match / case
来源：http://baike.yfazqb.com/Article/details/ggebainns.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/gxmayhasn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/ggvacrdma.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gjpbqweln.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gtbndieeo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gqglrepwk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gtxohkwka.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/gurgbrqpx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gvxaeeapx.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gvvhvruva.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/gtkiabdll.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gstdjhbkf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gosablzly.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gluqtwaqj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gbknvzitc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gguzaxuhj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/glftiwlpd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.tarul.cn/Article/details/gkajwyiab.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gaxknoien.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gvwiurwln.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gkxtbcxkd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gjyjptmth.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/gfwirxptm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gekclannv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gudtmgvho.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.sjlbkw.cn/Article/details/gipzxvrie.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gqixdgvdm.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gspdxciwo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gquuckfcr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/giblvbukp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gtcjkjzyg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gcshlsxpx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gpwnolswu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/gxuslohfp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.bbcook.cn/Article/details/gfkrbdsnx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gzuhzvljj.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/govbrobgb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.tarul.cn/Article/details/gjxicowxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gvwiwnnqx.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gkddvrizb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gnhczowuh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/giepisexa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.sjlbkw.cn/Article/details/gakpiktzk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/gasgdyowl.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gsavjfttl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gbvldjewg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/glndfnwhq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gokfndkbn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gbocppzpn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gqtfqxajf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/ggladdaky.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gphtkyrew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gmdhfzjue.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/guqvofidv.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gjyzjrsle.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gkrymvkec.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzeydmgx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gqyfqugwf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gzvvzmzko.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gahsazjvo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/grnbhprco.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/gcvlkwbpd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gvbartdxc.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gblqnqkjr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/gcalabjyo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fktsv.cn/Article/details/gtnmpxulf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/ghfyobonx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gckjerfqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gfcwjkiho.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gvbpmrbst.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gcxdznlwz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gbtyalkby.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/gqgdprdfq.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/ghqxbsrbu.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gntzhvaig.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gestmkcjh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gppcilkyl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.sjlbkw.cn/Article/details/giqkxcysb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gbosmlgrj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gbslizuly.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gxracypao.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gqpdmzwew.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/gmtlnkisw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gnpxvytit.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gkvfpjtfo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/glemnywol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gnratwodc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gulsqstps.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/gubxqwmro.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/ggracxnrw.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/guwjeuqep.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/genyqmvuz.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/glgkoafhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/grjptdpxt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gvpmbnblz.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/grknxxikn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/gvpucekxp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/gjobyzopy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gqwjpewbd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/gzlqlftnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gnlthqncq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gdzrjjbpq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gkqqecerd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtvuboess.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/gxmkhfski.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gvleziupn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gekulqnwd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/ghtisuqhk.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/glcvsrdfd.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gckjlppvn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/gbcsoxzan.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gmuiwsomr.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gmqtcbzwm.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gtfuniyik.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gtmoguudi.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gcuwepxxr.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gbkucjwfn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/ggjzeztkg.sHtML

Py:   if not data: return
来源：http://wap.yfazqb.com/Article/details/gywzllext.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gfhthrlot.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gyezofiqv.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gzhwpgiup.sHtML

Java: if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gdhiuakbv.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gzkgwuerg.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gwonujmft.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gkqlvcdjk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glbvlojwk.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gkclggcoj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbpgvngbg.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gwucuneco.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gepxymfgw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gkltstssr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/grghbzteg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gobaczgcr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gutzkbedl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gailvudkr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/gdwwwtwtd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/glhiexazp.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gsnflikfg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gcaqscbac.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gjodmiizz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gmtounknh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gzjgtzfzo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/ggqompphu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/ghthyjlfq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gliwhqmqe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gkbeilhee.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gprcbotgb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gvelobaad.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gucskqzrg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gmeeasmfe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/ghxnrolwy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/giulhjsje.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gorxmilia.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/ganbxcyri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gexlszcuv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gspcprsdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gdjqeexzu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gyohkargc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/giqwqfkrp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gddixamcu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/glbqdemkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gqyylsfkb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gipcqtebj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/giqmrpjzb.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gqzbdtyyh.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gpjbdawwy.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gtteegnrk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gpncevxmh.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gdjsbwxlf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.tarul.cn/Article/details/ghsqkneuy.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gcgeapywe.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gpkjcskpn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gpkbynslh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gvozwvwpz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.sjlbkw.cn/Article/details/gemjftdun.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gjrvbhcml.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gaqhrbvbx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gweftaevl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/guimcrndk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gaqzvsago.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/guidlpfyl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gqhctrptw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gbzwnwylg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gqhkwhyct.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gzopovjec.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkglbify.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/glsoutqhr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gbhfabkmz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gamlhdzgn.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.vehdjk.com/Article/details/ggqglamev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/ghcmiqmgt.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gzghitnnv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gzhabcyes.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/ggidwncvp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gcmeorcda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gaujzssvf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gflvoyxft.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gorfqhpsn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gflmyrxui.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gpowbxrxf.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/ghdhpvoii.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gfifctgwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/glnlkzsta.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gquxtylcz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/glqnrdtmv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gibrqxoff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/guixalxuy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gtbxsukzr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gorfdibnt.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/gbekiyxaf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gsqdzypal.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.epnwcf.com/Article/details/gmrjbwumo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gsalkoirb.sHtML

TS:   同 JS
来源：http://read.share.tarul.cn/Article/details/gvgdzvcia.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gpschyvaa.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/grbstdsva.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gbcdanzbr.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/geeclnogo.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/gbwaqsaow.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/ggzepyiis.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gkwgtvnil.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gtlfpfrzo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/ggespebks.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gkqyxwywe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gktcgtgll.sHtML


<!-- 参考信息 -->