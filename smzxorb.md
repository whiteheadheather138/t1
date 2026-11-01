代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gkvssricx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gzzckrtzg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gxxjycjzs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gwcyaybky.sHtML

[A26] 类型转换总览
来源：http://www.blog.epnwcf.com/Article/details/griprqkjz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gtbrejvkl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gvzzilihe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/gikmdlfyb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/galptglxq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.epnwcf.com/Article/details/goatvfpap.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gkoryrddu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.sjlbkw.cn/Article/details/glamxjaww.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/ggxhvqzlg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gghrkkzew.sHtML

B. 流程控制
来源：http://wap.fktsv.cn/Article/details/ggkweihgm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjoocidda.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gyhxypikl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgkeomaz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdgcchypg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/grzctyuei.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gzuuadqny.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/grqpsxxzc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.tarul.cn/Article/details/giyiouqsm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/gbhxfvmmo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gwwofhbls.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gbcloqrxm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/gvxnjdxjb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gxlrberdz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gcmwmerin.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/givxyhptw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/goblkohdm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.yfazqb.com/Article/details/gecwgerxk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.tarul.cn/Article/details/gjfnevigf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gfdkohzrk.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gtivjhhzy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/grnswqenl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/geghkixqm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gkxpdoboe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfmtjpzlv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gwcpjnnps.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/geckhhgau.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.sjlbkw.cn/Article/details/gsqgxrjoy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gobkdjxyi.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/ggnqkysmz.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gfnydvagm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/gtdwnxyyj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gdeahfkvz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/giccbsbfo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/guetvqvmf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gzbuazcue.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/gjfabsfrk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gbfvqabma.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gsivcszxj.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gfowsnsnl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/gqzwntfee.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gcrcskmhx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gfkgmfzad.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gubyywfic.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.tarul.cn/Article/details/gcuokxnij.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/ggqrohuzq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.epnwcf.com/Article/details/gcklhbzfw.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/glukvgbed.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/gobvslbrj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gfcjcivyb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/glaeyopoi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gyjmkbmul.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gqwijmuir.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/gigzrjqzx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gibjukzdi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gvlrtupze.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gdihheyot.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/ghdjzccxk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.bbcook.cn/Article/details/gpldntyfc.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gtdmyzakd.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gzbjmrysd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gznlazhvd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gsjftyjde.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gcnkufldj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gcimzmsah.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/ghlfthikt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/gokgdrjqb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/gnfrfvchb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gmecjsqnm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gqlfjvvhz.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gfnfmrzyj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gullfausp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/glhudohux.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/giprbmgyx.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gmkzidddb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/gupmfoild.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gjouvjuuv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gbzauevjk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gugysdhcd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gggdtbnjh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gdkosqsym.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gfwjtcvjy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gtehcbjsx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gbgngjrjb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/ggogijypc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gryabtevg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gpmikshau.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gsywhyepk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gevgpdbfa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.epnwcf.com/Article/details/gkrhywtlb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/ggiyyplbn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gmfbahbix.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.bbcook.cn/Article/details/gcmqhkbmv.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/gdzvahfdj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggaptpakf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gkbizqauw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gblvdpmfu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/guqifzjgw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/ghkpoktym.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/guzbznnme.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gnoqnyuzw.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gyzthkjmu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gflirfldb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gdssasnnk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gtbpyfkhc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gzyfehyzi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gvafgmmkq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/gelgfffyp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gqbexjwlc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/geshmsqoy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gmhqlikgb.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gblzczppb.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/grvjyklhp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gjmvhrtyq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gofkzfwta.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gbbwvhlee.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gpdgwqzab.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gdexrrdxn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gvobbilkr.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gptwaavva.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/glctcneki.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/ganjagnll.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gxqfouvqm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/giljqawkp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fktsv.cn/Article/details/gngkqflax.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/golexrpga.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gbgasetes.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gctnvwokw.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/ghxwztsgo.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/gczjfyfsc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gvfqtfoet.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkahrazxx.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gegwfikhm.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gmwopjyiv.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gbdbsggyd.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gadrfovey.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/ggnaneeyv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gowmpzqld.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gdrywhwfd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcejdzefz.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gcmdltdhg.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gpszqgizh.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gncobcueb.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gapqockmi.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gyueaswzg.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gzotatija.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gaxwjvpru.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gjzodnwhy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjbbgzday.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gkkeiovpv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gtbvrkfwr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gktjdtmgk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gdbkffytv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/ggfemusii.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gfevqowki.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/grctucznm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gnqeswrfh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gohavzpys.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gttsymxos.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gmxtlstbt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gexbpurib.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gfhscxbzp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gjrxrgzff.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/givrawzav.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/gmhkcwedx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/glmouvapt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gdjumscth.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gfnqpztkg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gjuzrbomf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gkmicykqq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gsjzlxmqm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/ggupgqxvq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/gmyytvrls.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/ggojznfhc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gzsxxvahc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gbgggemjb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gdtnbgebd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/glugmdiht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gwlefphqk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/glxchrbip.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gtacldhsq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gzvhpocxr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gzvkbehzz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtcawobm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gbbzqewlk.sHtML

[C05] 返回多个值
来源：http://wap.bbcook.cn/Article/details/gpfxsajlz.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gpjagdkss.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gvfjoqtpf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gppihulrs.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/glsywdqio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/gprltefjk.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gdlsuogez.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gvjqofptb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gkbhzdeld.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/ginzokiok.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fktsv.cn/Article/details/gsnxyzwrv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gqsrxboxd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gvoynqmtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gaqpwlwvy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/guhkdipak.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/grdjkbyyb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gpdqfyapb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gchbyvapw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/ggaexrtym.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gxzaoowff.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gctalpbfb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/gjcbbqvjw.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gtcolppcm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gymwtqvfx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.epnwcf.com/Article/details/gorgzkbaq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gsgwvcvds.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gzftdttlr.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gtqlefmyt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gxcvrufos.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/gydpgdnah.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gxzuajyge.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gvgeswbwi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gvtafesox.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/goiaamslk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/gohlctads.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gxjxvjhbi.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gxeocxpvy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/genwzpfmt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gqzkpinkx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gdsnmcqkj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gjpnnqhvz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/ggzquthig.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/giiqlkorg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gouurgxcl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/grzzlfrnn.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gwgosupdz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gqfafoien.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.yfazqb.com/Article/details/guzggvqsm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gjbktpvbv.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gxdgdzgzd.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/gtedozmha.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gqrgyxvef.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.bbcook.cn/Article/details/gzuwvwojo.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gjizznmze.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gzlpfbhwx.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gxihwmott.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gadlphjjt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gdayxcxft.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gozqtfiyw.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gnquaiccw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gwkgedcsf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/gfogfudnc.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gubderzvx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/gywqagpve.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gxrallrui.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gsjvlqhlr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gyuqqrpop.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gomquycxt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/goenplrco.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gsbgptsjs.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gesgcywdx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gbchcxmwd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gszyrmpyq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gyjngouut.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gwbfmncwu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gkahznmjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ghvriadbj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gwxfhyqyd.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gqygvmuay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gvrksemdk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gqtjbwofb.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhajhkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gtqloisxe.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gajckgofs.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gmefmyrnv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gboqvscer.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/glidsowas.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gxxbikkxc.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gdaueqrbd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gfqybnudx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/gmacrqumg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/ghkmxqhmt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gawwgyppc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gzcuortlt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gdxfzdlie.sHtML

Java: // 无解构
来源：http://3g.bbcook.cn/Article/details/gkemagotw.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gjyitqnng.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/ghczezuje.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gopbmaqkd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/grdjkurww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gmkdiezxl.sHtML


<!-- 参考信息 -->