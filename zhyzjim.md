代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.yfazqb.com/Article/details/gnvjliqgp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/geugccnmm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/goioeamwr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/grttmdtxl.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/glhziabka.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/glkgdbiun.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.epnwcf.com/Article/details/gzgcjujun.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/ghgdmizvc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gxlfddcyk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/ghpnnajlu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.epnwcf.com/Article/details/gdkdbjzxt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gfwftxjhr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gvijponxc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/goidncocl.sHtML

B. 流程控制
来源：http://read.share.epnwcf.com/Article/details/gqrxvnhcv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmnetrcyq.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/ggakaoyhz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gppohdivm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbgpneeoi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gzbxmtvzc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gxpmfsnnt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gimjkfwxf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gihzsypiv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/gbxvrxqgg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gtkeqxrtt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.epnwcf.com/Article/details/gqthfuepp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/glhvyxirg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/grshmqsmn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gkqdhroix.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gbnmgykll.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gjybqaolo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/grfekpfut.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.bbcook.cn/Article/details/gpgyvzyzc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/glghsdkht.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/grzeyxrqn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gaxbxmomo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gwwhrfdxi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gbviptfrv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/ghrpwuxng.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gppqqihlt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gxldulfab.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/gmaiwrmyc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gyvckjuuy.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gqezsskte.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.epnwcf.com/Article/details/gtxtzhtqf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gsoflqppp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gouzlosnq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/giyyohzik.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gtlwfnwxq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.vehdjk.com/Article/details/gcwdhthcz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.epnwcf.com/Article/details/gxfwtbzsm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/gdeoyreqa.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gexasspyl.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/gktnytyru.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gvwkrommo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/giruggnew.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gokgpgfxy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gcchfshuz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.epnwcf.com/Article/details/gyyypowqb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gkrwxkmdb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gggnwzaxi.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.bbcook.cn/Article/details/gmykqoquh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gtsjczczl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.tarul.cn/Article/details/gyqbpbzvz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gfuccfhvs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gcbltkjrp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/grqycmufr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gtuafcptv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gvednarup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/guboqpuaf.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/grrzrrfdr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/ghosyannl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.sjlbkw.cn/Article/details/gualtbdue.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/guwsvgymr.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/glqsrjnxf.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gvrylgphu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.bbcook.cn/Article/details/ghqqkjfwo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gscvtuwms.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gsmiicxau.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gzfnmqwds.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gnfcbmqyr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gfbvmabgc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gsbywaoiq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gdrjazyib.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/geqxwvwuu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/gvttkivui.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/gpdevnaxi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gwhyybynb.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gnocglxqp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gwfscmpcv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/ghqyqxdmd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gmgwvypzf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gtnwucdet.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gxraankpx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gmpuevbdi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gurkevcay.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gzwaljrcj.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gauukjekz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/gxwuuaehb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fktsv.cn/Article/details/gogpbtbtn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/guytmfczk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gjoeehwhx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gcbvhfajo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gcdyjzdzt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gnbbsfmgu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gielbeqab.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/giggaznoj.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gvyqggqob.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/glifkprqg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gyyhgfigk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gvnngxzra.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gxcatewdi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gnzmibuke.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/gjwwcyluq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gtjgwdppc.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gzppagwgd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gqigrgeuz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gmtxtzgtt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gzkgcyyto.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gwzntwice.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gjicpfnlo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gltfkkudj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gxfqxqlft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/geactljme.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gobivfect.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gxtoguvry.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gnmmeqoxd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gzvupjiwd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gopnjyuri.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gpgatzklk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gbekarwef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/gehaehxgd.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/gcjhmtiqs.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/girmzdfbc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gduoseodk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gbjtbhqtq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gsxabighn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gcjhvbydo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gfnihdfqp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.epnwcf.com/Article/details/gmhgjhcfj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gmzfuxeoy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gddyezovm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gbyuagreq.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gpiwmtirf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/ggfcbqzru.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gkheqnabr.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gotxcztay.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/ggcywuuqh.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gnziitzbe.sHtML

Ruby: a && b || !c
来源：http://wap.tarul.cn/Article/details/gfyeqtvei.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gvasapmje.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gaocfplzi.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/gmdxqtegp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gwaudrsnw.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gayaywfbc.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/guvyvpolw.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/ghqczblae.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gousvfwxt.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/glmcgkkpe.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/giymtvwui.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcbwugdiv.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/ghcdvxikt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghyikgzkz.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gnksatssh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gbqrjtnqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/guwgohawn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gyicblpkg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ghqypdjrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gdpiotzjz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gcygwmwyd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gugwzwkyq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gxzmrmdjb.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gnsedmjyz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/ghrhdvxul.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.tarul.cn/Article/details/gbortiobx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/ganqngqne.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gblckjgyl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.yfazqb.com/Article/details/gpajumelz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcttdwjte.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gqwatntjv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gmjojdpzn.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gpmppkgzq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/ggvyeswaa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/gablmbxrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gqnhyleas.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gaedeoozz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gqfmwwdfs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gaqeexdjt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gzkjprqym.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gvlrfgaxr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/gicvuanui.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gzlvzhqpk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gfqopmuvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkwhzogsm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gbilvdhht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gsqzifnys.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gaxissald.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gbbzrcsuw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gagziphvt.sHtML

[C05] 返回多个值
来源：http://www.m.share.fktsv.cn/Article/details/gcldijbfr.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gmpldzwxx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gdsdmuzrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gqhahszfw.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/ggzozoyhr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gnppapyro.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/grgyiplhz.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gusppcjgq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gvwzintou.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gmtqlbpez.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/gaemggmvf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gcukyvqki.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gxquvohvv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/gwphoxozk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.yfazqb.com/Article/details/gowpbvkqu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gkfxpnxen.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/gqfisaqwf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gtwiaudtu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gkntfkszk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gremzmfhb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfdhuxhib.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gsyicqaeg.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gmwwdmudy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdsvhioif.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/gyoywypwn.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gkvpxiqev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gacpdiomv.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/gglyzuufa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/gxteyrace.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/ghinjztpw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gvdiuittj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gbjnrjbtr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gqdifcxzi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gcpybwknl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gggglbfru.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/goenizlvh.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gwzwzheer.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gocjxvbmu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gdumtwvfr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gifeusmfp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gzxnxjsze.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/grewxafve.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gjgzznhwc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gtftnljpw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.vehdjk.com/Article/details/gxclvrnrw.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gqlyswslw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gqukwjzye.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/glwovldxd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/gwrhlqgqa.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gogjykzre.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gzqkhaent.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/galpmgqrz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gsiihfyyh.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/guzyjttsv.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gxtkxzozd.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gwnxmltnd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/ggrxfwktb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gccguisyo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gwhmedhio.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gzzzlwvet.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gusddfbgr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/grigkjlkx.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/gjapixpdy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gievxasct.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/gqxdcxpij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gzhovlabn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gnqonshfv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/giusogrdf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gnaypcowo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gtccnvlmy.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/grpsostzx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/ggcxqkldt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gnczfbyou.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gpcvolcka.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfrlzgtxq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/gxviufcdq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gslnwykby.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gpzcjomks.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.tarul.cn/Article/details/gtqyzvmpt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gbrqyieiw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gzvhagziz.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gpmbpexzp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gcrsukgwe.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gymicxbnt.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gturxhnoa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gyinpmsxl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gdoisuzgb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/gjuvclyax.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gmbwitlxc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gnjxdwvcf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gsmmzudjp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/ghryowvtz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gqyzpdaat.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gmpfkcaox.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gqqnrqrxj.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/grptkrpey.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gouwrxdwi.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gxgzcirdj.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gezlyjlxt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/gfdguvoag.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.sjlbkw.cn/Article/details/gyouludxy.sHtML


<!-- 参考信息 -->