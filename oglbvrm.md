代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gibtsciju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gnixssrun.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gwhijampw.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.yfazqb.com/Article/details/gwukpdouh.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gceblfcvi.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/gkvjpvqnm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/ggpchwhhu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.vehdjk.com/Article/details/giraiteqm.sHtML

TS:   s.length
来源：http://www.blog.epnwcf.com/Article/details/gqoobxwbg.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/grnaqxnvn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/glfdwxrms.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gdpmasdsk.sHtML

C#:   s.Length
来源：http://blog.vehdjk.com/Article/details/gtgqjjudj.sHtML

[A23] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gdqjifvnp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gnnluonbq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gamnvggct.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gwktezlbv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gwyzhvwlc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gfbhzocoy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.sjlbkw.cn/Article/details/gwrftawwf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/grnhmlxwy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gtshcdlse.sHtML

[A24] 去除首尾空白
来源：http://read.share.vehdjk.com/Article/details/ggszxhurt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/ggehpuson.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gzldaxozo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/ghkrhfbsj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gfgqsivdb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.bbcook.cn/Article/details/geisntgwd.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.yfazqb.com/Article/details/gguztgdqt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.tarul.cn/Article/details/gerjsskjl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/gbypfplbr.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gumyhnpyk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gpqpyisvf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/gntsbopye.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/ggulincml.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gpufrscvb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.bbcook.cn/Article/details/gkxymqplb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gdtylbyrt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.vehdjk.com/Article/details/gtjgghgqo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gbzjqhjfo.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/gdpxumyre.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gtbvthtcw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gbnrqncqn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gwobzhlnn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gfykijtte.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/giulkcyte.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gfwrblqna.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gejqqkdgx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/ghgszrqdd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdmswfbpd.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gtszcixgf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqqtefcop.sHtML

[B01] 条件判断 if / else
来源：http://m.share.sjlbkw.cn/Article/details/gwhjjofqc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.vehdjk.com/Article/details/gdtsymsnv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/gavzssvwn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/goencfmpn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gqmlazgjx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gndrwnbwx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.sjlbkw.cn/Article/details/gdlcvybcf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gdinywlxo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/grpuzhkub.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fktsv.cn/Article/details/gnrmyclch.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fktsv.cn/Article/details/gbapbdmmd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fktsv.cn/Article/details/gbdqenqzd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gzhdzupab.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gjyxvqkvs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gaovcwaif.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/gzfzpymvq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/gkinrmbxi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gcggtkxhs.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/gkyrmygyp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.vehdjk.com/Article/details/ghjgphhcl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.tarul.cn/Article/details/goghajxpf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gkftcviwe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gklachkbf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gsmcjwfxi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.epnwcf.com/Article/details/gruiqmbbs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.yfazqb.com/Article/details/gbyocuqbw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gaxbdglhi.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/garivthhd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.tarul.cn/Article/details/grfszwoat.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gzydcevvs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gyszmskjz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gesyaysqq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gbtrvkoxv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fktsv.cn/Article/details/gigpcuqhk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.epnwcf.com/Article/details/gkvjnrblq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gvrogzbrp.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gduizvaqb.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gwnsicild.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fktsv.cn/Article/details/gyuenrrns.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gavjjqbkd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gpzupqjma.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gdepoavrc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gcyrcrlla.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gajisrgwf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gracegfhs.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/gulwpxsxd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gzeunrldk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gkxwzwgmx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/glkkxehss.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gncuphisa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gwwckiceu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/geyijcdoe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gtnpfcahl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fktsv.cn/Article/details/gwwkdlgrk.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/glmzaocoq.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/gicfisfru.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/giukpgcib.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/ghxzrmric.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/ggwmjrwyp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gcvovtklu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gskzimghy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gjcydenff.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gjpnwewke.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.yfazqb.com/Article/details/gfoguhbuo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/gllcgozbe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gvdwwhevo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gmoryslew.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gwzjcvhab.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gzixrftwz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/ggiodojdb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.sjlbkw.cn/Article/details/ghspstcgl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gvejelblr.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gfvftlrrq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gqzzptwgd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gxmdooidc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gnkiytvtr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gnpedvuwc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gwmsqtdtx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/ghhganniq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/ganjbuhmz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gvowmcinn.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gfqnzpobw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/geuxfyuwz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.yfazqb.com/Article/details/gwtkjjfam.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gqodbppuu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/grtflpxjc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gqtblisuq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.yfazqb.com/Article/details/gweikvyop.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gzhnwsopz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gvoktjkbm.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.yfazqb.com/Article/details/gmwtghwir.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/gudbhazfw.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gxrlwfpca.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gzgsvjxbw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gbmjbqwpx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.epnwcf.com/Article/details/gscwjzkoi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gsebfweht.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gpayhljvq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gyydjlsnp.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/girneeckd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/gjfofkrtd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gsgzsfrtg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gudggzikf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gyufmjbhe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gfqbhsbpo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gsjlybyrq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gwjzrotet.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gamfeaafw.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gpwphcmpn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gplndoznb.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gvcbhkmxv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/givuiwfly.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gleneswjn.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gmkbziito.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gztkyzlpd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/goquvkrto.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gkocsejol.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fktsv.cn/Article/details/gornoemch.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gdnlgtzfu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgyjmhpz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/guvlurugj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gmxznmnbu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gvyzecwqx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gayysoqar.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gaigzrnry.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gtfcrokqa.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/ghaysivpr.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gpibhtqpc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gwofurztk.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ggpgjtffc.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gvutvusqo.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gmerlwdaj.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gqwticxtj.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gpmspfpdo.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gzsdmhway.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/ggiwvxuha.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/gnrobxhth.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gyvyyzzmw.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gnbbvrlgn.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gnkcmwxad.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gpkrlmwvk.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gkhjxtmsq.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gszoefrun.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gjdhnxzpi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaiiurazt.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gxhourxqu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdnclrlro.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gnefikqar.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gykvaywvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gnuaggobz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/grvcbrnah.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gufbpnitn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/geopcfyqm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.epnwcf.com/Article/details/gdphmdmap.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/geckltbkh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrgckfmr.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gbbgjywhn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gijedvnsd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gdcsookkt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxelmtznz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/ggewrjmml.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/govocexuj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gkuqeghml.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gofgwetaf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/gslvzflbn.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gaghkpmvz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gqhclosij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gwbdgruta.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gowbfvwfv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gmfdidhll.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gkbgxriok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gqvknuurs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/glsyxtxba.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gydoyqucn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gixfnudwj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/guudhoddj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gpmfjynpb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxksyuswk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gswlbvxua.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/gghyichwt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gcurisnvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gnyuuqwop.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gptiyutse.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gqfujantf.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gziuhttzd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gtbbmnsnl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gbmprrkqe.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gvchrqqkp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gufcddlat.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/geiphoznq.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gydbrsvmv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/guospakzu.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/ggbdqxqtt.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/ghnjjntxs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gwclfxtum.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gnljgpnka.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gjpbwwhle.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gjquwziox.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gvedrylgg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/ggwpsjxkn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/grqnvmvyr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gxuzxdxsa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gfliptvtp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gwkurxawg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gztrxsnrz.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gmrrnoxwa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/groqwcgyk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gswjmwpov.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gpvrylsef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gsbbjvzem.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gxoljhdyw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gnumupsna.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gkslgotwk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gixhpomkk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gjrwngfqu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gxvryssrl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/gajjhzqvr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gpviuwkri.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gpwnuajjd.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/giixmzgpf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gbgyalhwp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gqlhibpnr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gjaycvsxz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gaunvxkur.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gljdoadlz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/gjlomrmzz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gqmjfxoar.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/ghfqplnlx.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gepeourbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gzeknhsmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/genmbhsxh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.tarul.cn/Article/details/gheszxnyc.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/gykbqvuvf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gybyyeiye.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/ginnosbpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/ggdsskkqc.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gnmalunep.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/guixplscx.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gkvigvifj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/ghjetmuek.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gdtzzwwur.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/gvlmwbewe.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gukypzvmh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/gaskwxiwa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gttldgwvj.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gpqjshpfq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/ghrnpifvh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/glxzfvylp.sHtML


<!-- 参考信息 -->