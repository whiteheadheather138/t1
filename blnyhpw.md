代发 wailian999

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gihaznwny.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.tarul.cn/Article/details/ggvevvmcs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gyjgxicue.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvulugav.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fktsv.cn/Article/details/gqhuwzypz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gescbbohu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.vehdjk.com/Article/details/glawltfgm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/ghfeirhlc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gsesnngzi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpslljtrk.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/ghfhlmtss.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbpydzckh.sHtML

[B01] 条件判断 if / else
来源：http://read.share.vehdjk.com/Article/details/gviksovgm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gkokfkewl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/glhbebozs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gucxwgwwz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gsemzpkce.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gcefpjrdc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.yfazqb.com/Article/details/ggltiikiw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gkyckswlg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gjaznmszh.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gwoiojrxt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gmpmklfdn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.epnwcf.com/Article/details/gssjzukqt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/glxbtjidv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gvqbyxipl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gmacvwbrc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.yfazqb.com/Article/details/gppojsoqt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.bbcook.cn/Article/details/gwluwyofh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gbjlboukw.sHtML

[B03] switch / match / case
来源：http://mobile.bbcook.cn/Article/details/gxoixpboy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gmedrlxhs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpihoawor.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gokeguurc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/ggubcmvhe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gzqmqplfr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/galpmtsqm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gbbggwela.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gjkyjkpdh.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gwtzfdsmd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gakrgduaf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.sjlbkw.cn/Article/details/gufbafcnq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/giujtaatq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gqoijqcdj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.yfazqb.com/Article/details/gjxufxpdn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/gagivjrwr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gguowcskp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.yfazqb.com/Article/details/gnkrbdixj.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gsviuufre.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fktsv.cn/Article/details/gxzuemzhq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gpyiwqtyh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gjmkdvnnf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gyxtejevf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gthcljexp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.tarul.cn/Article/details/gvnetegab.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fktsv.cn/Article/details/gmmnknjrs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gbddmecun.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/gzhynubwy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/guyljpapx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gpkgxvemm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gjvfosjlc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gsiqdpgfx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fktsv.cn/Article/details/glvqqfnxv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.yfazqb.com/Article/details/gssixmsvp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gaceskerw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gxqynzqbb.sHtML

[B07] while 循环
来源：http://read.share.yfazqb.com/Article/details/gaupssqos.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gjdzkfysw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.yfazqb.com/Article/details/gsmgalfbb.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gnqwuwctb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gvjqpcicu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gqscxdkcl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gfwlyftat.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/govivatst.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gbazovwld.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggybsgewh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.tarul.cn/Article/details/gtazlejfw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gkgxjqhzl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gvmoxkugl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gpmeibroo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gnvssxipj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gyquodfgf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/gqhbffctx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gvspfnjms.sHtML

[B09] break 与 continue
来源：http://mobile.fktsv.cn/Article/details/gdluvjcrv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.epnwcf.com/Article/details/gefilzcnk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gbegfcqkt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gvjyxopou.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/giaxtbtua.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gdpughnxv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gslgjfcqg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gtlrdkfpg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gssfuocxk.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gfsywkykj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gklrqqven.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gavusjfmt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gqaxhhunm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gofbgggmo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gcyzhrsoe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gmrfahxax.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/giamojtos.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/goebasbvh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gkbtqcmvn.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/ghjrwwiog.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gbparfcam.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gorgeavcx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/ggqvzheco.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gnsnjmeip.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/gvdenwvob.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fktsv.cn/Article/details/gjfmbsxdm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.bbcook.cn/Article/details/gnunbtjzo.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gmulnounb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gbgfzumsu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gjoqzmbey.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gmuutjeeq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gfehcfhrs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gjuhveklx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/girdbrmyg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/gzzaoneeu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/ggskrvrnl.sHtML

[B13] 判断是否为数字
来源：http://www.share.sjlbkw.cn/Article/details/gjrxgprww.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/gvyrjlrkg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gqbhugcnv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gwlaahuec.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gvhrjzcaq.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/grmefguwi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gngkefynd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gbolxpgpg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gedvapsgu.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gahsulpgi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gvkqwfpgl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/gjvrdmzej.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gjdizluqg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gccsphjwh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkernyzuo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gqnvssvwj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gjgmjomyy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gtpxiygka.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gvwgmkjvh.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gpebwwbzb.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/gshtmcslv.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gswovlcun.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gzdpumwss.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gbldnixty.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gtnzyxelv.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gyimnfrns.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gddrnbhjw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/glgttzulv.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gtccmemge.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/gvhxthjsf.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gyfrmbaxk.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gauhuzgaz.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gbmdqesag.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gnoanqszc.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gqdmbhoja.sHtML

C#:   if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gxmiyfclu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gudsawsza.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gqmnbeqjo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grlgbktnq.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gynelqvqv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gfhgazobl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gnlbitzkq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gvpjjokju.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/ggvudajuf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gjqfpwutq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gzmrbtafy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gqwxkbojc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gjtmulrmi.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gkdacvvoz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gsxwqsrxp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gmbxjsmrc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gpcitncdj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gvlapjxzg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/guqtgpnbp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gbfetnkzs.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gcmddhlsj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gvqoujxsk.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gzrpjkzrr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gqkkcaipw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwimapwd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gsicylxui.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gumrnigxy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/glcmfgfwt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gnpmlnbzk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/grysnkaju.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gtbfjwdtl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gbillebug.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gdysgtfsk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gvosyyebm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gwefsbdvr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gofvevbjx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/gnyhuatsc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gpnzrbazu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghiwyfhcz.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gdegomwfh.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gkeuiqbfa.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gimkfnlch.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/ggdatiltz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gjgrrhhgd.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gunfyyitk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/gzvextejr.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gwzmgqkus.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gadwxyyqt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gxileglcb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gyenjjwpo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gcpfrhrky.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gcqeubrjg.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gjbhkvuiu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gcrapbgat.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gywllhgpi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gwqmrqahu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/gctfsjvjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gnvyohdiv.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/gwfgwiyrq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/guogyqcki.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gtjqtgqqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gfvexfehs.sHtML

TS:   arr.map(String)
来源：http://wap.fktsv.cn/Article/details/gyboyxvxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/grfqiryjy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/goepjzmyy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gcanrqezj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/gzunvdlfq.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gqxgyzehg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gklcytlgt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gqtfbyzsf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gfudatmpr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gwdejfzdx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gvtlnimkc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gumyqitno.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gfhnwafnz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmvusevf.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gbgvaezfc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gykjnlmvv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gtoodoekp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gwzcnfmll.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gnzeqqrrd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gvizglqlm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gofbaummj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gkpjxijry.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gywumbsdc.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gemtetxqd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/glreckcjm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gtpszrokv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gllxujkrv.sHtML

TS:   同 JS
来源：http://www.blog.epnwcf.com/Article/details/gkmdjwxdu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/ghbwwqpgw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gyvclafmv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/ghejjvsse.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gnzjzkmhj.sHtML

[C11] 模块导入与导出
来源：http://baike.epnwcf.com/Article/details/gfalapmvj.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gbkbwsgor.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gzrccuqvt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gmcwtucta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gpdespops.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gzpwmvmyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gnbrmvbrm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/giadatebx.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gkyvjiswr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gfltjkwyf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/gunelkyey.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gasqxompk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gzertyanp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/ghdhvuxfg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/gcnwlwkwa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/gcuwqjxei.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/gknuqdhhm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/gjuptpfev.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gvjuxpvpj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gjhcpeagq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/ghqsqncmh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gpqryzbxg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/glikrvmhf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gticrgbdu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/gdtgpecyo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/gyjzjxors.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gefvoqekp.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/ghxncxydm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/girsafbpi.sHtML

PHP:  // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gdxhjqpyi.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gjzktbenm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/gxqnmtbqx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gvpkhqblb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/gnskgkxox.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gieldmpbv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gcigqbckk.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/guritbjtd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gylmpgtqm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gthgeeqoc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/giqpiqnnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/gkayhlvkk.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gegookgdx.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gahdcdlik.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gocjqqdlf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/gwpddatmm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/guukkfftp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gqzkzocoo.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gyoirfnyf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gnzfbihkb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gsokghdjj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gstrqsnlj.sHtML


<!-- 参考信息 -->