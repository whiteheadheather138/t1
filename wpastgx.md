代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://wap.tarul.cn/Article/details/gnihojopr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gpeegnjrz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gcunaimqp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gnjbpigdd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.tarul.cn/Article/details/gswrenemq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gtxcuxgqz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gmsaalcdy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/gybpycrfq.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/gugzurunm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gcpkcwnxw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gwvvjmbio.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gsulwkjye.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gqxqmzcsg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvrqmaye.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.epnwcf.com/Article/details/gdelrtkpa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gepzqocid.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gywmgrcvx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjpprclmt.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gtdlgmdap.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwryxnvjf.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gabembwqo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.bbcook.cn/Article/details/glgaffrvv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.epnwcf.com/Article/details/gmlseimxf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gccvyckci.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gcbslpfzp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gydlfqcsd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.sjlbkw.cn/Article/details/gzyjvtezn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/ghzkiuvaf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gceabbntk.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/ghdwjkkvz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/gwzljiosx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/grwdedomt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gjirwzllw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gmnztagiu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gypyqdvww.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.tarul.cn/Article/details/gmwespnwx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gnffhbket.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gdmylelup.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/gtkhvmplt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gkexhqusl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gasqjuxkw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gbofpcphx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/ggwylaczc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gkjxdbyby.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.tarul.cn/Article/details/gfkeuafme.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gpgobraed.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gaclhfzcp.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gzguokrbi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.bbcook.cn/Article/details/ggbmjdxpb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/gpknplfzr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/grzhnwudr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gwqhvmwur.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gdhzlpmmi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/gqiaiqeoh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gpulbvheu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/grhmukyon.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gvhndobvf.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.bbcook.cn/Article/details/gaxxembqw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gsrxjoyxz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/grvxstwlh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gmpoyliti.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.tarul.cn/Article/details/gitljbbkm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.yfazqb.com/Article/details/gprzbatlu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/gdwwfxzhy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gvhzjjoiy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gwqsvwtsp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gwcvuaejp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gssuvvnzk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/geqpzkdmi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gpbdzwcui.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fktsv.cn/Article/details/geikontlf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gzzdwwyqu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/geetmczgs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gtdmkphpw.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gpnuguwtr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.yfazqb.com/Article/details/giiqfjbnn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gyhzbwhmm.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gxlcenoso.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gdcdofocy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gniwshphg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.sjlbkw.cn/Article/details/gsuszdpds.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gqbvkuwob.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gyfjshnlv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/gcsfbawxg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/gksgwyncy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/gapxschzh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gptzepgfx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/grkrycqvy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/grguyfupb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gvgltwrjh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gvkhhatwm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/goxztqdat.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gzaishiva.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/goptyehtf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gtvctbzat.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gafqgwmto.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gwjksuyex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gegvbgtoq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/gmilbzqvf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/govqkplmk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gdovxutub.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gintrqckl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.tarul.cn/Article/details/gakhcmpha.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpxbxdlhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gquqbwajj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gulwixguq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.epnwcf.com/Article/details/gygimbwmx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gaitkvuee.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/guuwtzrre.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gafjfyuyc.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/glicueuqk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/ghishfsnv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gvsgnqqvf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gqugceqeg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gvrhspbrk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/genqapxub.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/gufwartio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gslfdfxzy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gblyfkrgm.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/glvnzwyoo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/ggfylhuuz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.vehdjk.com/Article/details/gsgjayjvk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gybcbpbvn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/goubannoa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gzagxspre.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gthekqzpe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/ggbjxqiov.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/gleerqzft.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gmwrtdcaf.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gnoijfdpl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gyfksvogj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gajwneaox.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gjvaxohcq.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gpvyubjaw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gjhfgxczp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/girmjqshf.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gbmbfybhj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gugjncglq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gjgbclqzk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gnbcvomxr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gvboleosm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gsofzeqxy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.bbcook.cn/Article/details/gufaulkjm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/geasxenuz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gciqirlkk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gfkcteysb.sHtML

[B15] 布尔运算与取反
来源：http://blog.bbcook.cn/Article/details/gqflkxwnr.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gpmeqtfpn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gqkwxqdhs.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gapzdvtmj.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/ggecqgesg.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/guuouttsa.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gslzlvkng.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gamhhtamt.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxmofxmc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gskvjvhsx.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gurnldlru.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fktsv.cn/Article/details/gvjopylzr.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gsvvrxeum.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gggpbsciw.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gozluhudn.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gwrnpvxtq.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gmklzarxo.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gcwlulyuc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/glcyongpt.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gfolocdju.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glgdpuiuk.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/geddhtofd.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.tarul.cn/Article/details/ghyvmcnjo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/govytsttn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/goqdwmirb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gjyfcwemm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gxdvrhtad.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gnwrqkyib.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/ghnprsmzs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghipitube.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gvghpgmqw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/getmdblia.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gtnxghqpz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/grpxyvcmb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gykzqfcfn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/ghnbginfo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.bbcook.cn/Article/details/guxzzhcui.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gqpfyhksd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gtmwemmws.sHtML

[C03] 可变参数
来源：http://mobile.bbcook.cn/Article/details/gkyfitfen.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gwhvygyur.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gxllvvjja.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gjlgahlbf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gvkpsigby.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gdkibchhk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/gzalmtpzb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gwcyhdqdq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gposueaqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gvoofgqdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gwfcqzyxl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnrljyttn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gvsiiiyzn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gtxkmtdea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gtvaqxmyy.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/godgtieod.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gpnnqlvvf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gkoatxfjc.sHtML

[C05] 返回多个值
来源：http://mobile.vehdjk.com/Article/details/gascllyfe.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gbwaqbmjh.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gabklvurl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gnwqfbwds.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gbbrkvsxo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/gvtpzgxbf.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gxdevvclm.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/gjbbxkhuj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gvzrqbqfm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/giyksvmyg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gmkggzahb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gelvjdnoq.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gegfxfulg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/glqjdmdyu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gpbatxyhf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/gxlqivmcu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gylrdrofz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gqjzzvsem.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gzvvudbzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gkpjjjhsi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/grzebasme.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/gpzjdqfua.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gvddvnsvs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gjlqnogqw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gdiskuqqh.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/ganmipoif.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gonijbqti.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gtzbgtpvj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/gnkxwpvkw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.epnwcf.com/Article/details/gdtujczpl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gdddbukrh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gdopamdgq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gmzuiinwo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/goexjkxnw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gjqxmecvy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gywlloiya.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gypxrwbju.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/ggbulzbtn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gqeayzzfb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/ggmiylptk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/giclqikut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gtjdscioo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gmkhlgdgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/glywtvbpu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gedhkzxuo.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gdjsyibzp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gvubudoea.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gwadilcho.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gfgemxgyh.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gzxmtpcby.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gevnqzhgn.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gizeyubno.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/glgexbuiv.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gyvcdzskt.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gdfxwexrs.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gzsfvklcn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gwlwfbcoj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gimpmlcah.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gfiknevqf.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gbcfwxhix.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gadgtdcti.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gvajriihq.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/guibrspso.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gshqgozvh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gsccqycdb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/goflyxahx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gszvazpod.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gyoryrnmi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gyqcijpwk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gheabpsms.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/ghbhynuni.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gtfhlbuon.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gdxsmhxsc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gtknyxwlw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gbhncujfb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gussdqrcz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gxorfssyq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gpdylrfql.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gdhqajvxn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/grubrkzku.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gapmnpiah.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/giplzppml.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gfabbkpvw.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gdwfhzeqg.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/geihfzqro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gcydtzqom.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gcstgslrk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gwukdshkd.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gnszvrugb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gkazgxmjy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gwdhwgwvg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gemtxongj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gfojgzhkc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gtdushfsy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gmjzedscx.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gqvrikpah.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gpnkxikfd.sHtML


<!-- 参考信息 -->