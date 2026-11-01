代发 wailian999

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gvcdmawdf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/ghfibweef.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gmmmhdsvm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.epnwcf.com/Article/details/gelgirdll.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/glnietdkx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gytkobyxa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gzldrwjxo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/guikwbcee.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/grrddssve.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkbzxqnjv.sHtML

B. 流程控制
来源：http://www.m.share.tarul.cn/Article/details/gwvozzkwk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gciqhpabf.sHtML

[B01] 条件判断 if / else
来源：http://m.share.sjlbkw.cn/Article/details/guzzbdxqk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.tarul.cn/Article/details/gvsyyohro.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.bbcook.cn/Article/details/ghebgzqan.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gdfvfnggn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/grndhigmf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gvhdwvryy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.yfazqb.com/Article/details/gtizhylve.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gqewypmmn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gnlmynrrn.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gcaarcbja.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/ghfqtyuvu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/grjmbykhm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gdflmqdmo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gyyasruer.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gftarvpaf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gimmgcdxm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gmgqyuzau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gahxfrkip.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gdosnyxjz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gpviaddvm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gvndthyan.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/ggsbpogne.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gcleknrwe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gyduvecsm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gjwmatzgu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gtnivoete.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gljcemsdk.sHtML

[B04] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gnncyojmc.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/glffhjxpg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gxutgxwxo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/groehoops.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gajqeqoqw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gevopimcq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.epnwcf.com/Article/details/gnnqpxcbn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/ggxsysfmd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gqqyotkbz.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gufijbywt.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gdcuusojc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gdenpbrti.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gpjrkytlh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gskbsjezu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gohzqdtys.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gkzhmnxmn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/gwsijhykp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/geqzvkyqt.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gpcdbaqkv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/grncjaohl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fktsv.cn/Article/details/gkomqzbal.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gzryryiid.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gjmebiepv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/ghzonhcic.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.tarul.cn/Article/details/gczwqcasd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gmrcpipcd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gnkwcuakl.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gcffzqosh.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fktsv.cn/Article/details/gblfsfxfs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.yfazqb.com/Article/details/gsaxgbbqh.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gzraabiti.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gkqhjmnpr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/ggljqeuwl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gdjhdoxjt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gbbbyekoi.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/ghxpiimbv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/guibluzmk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gpcxgwvsd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gevoltaxn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/googcjxcg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gyrbcuphu.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gaewyamcr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.vehdjk.com/Article/details/gjyihxkes.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/gqamubeox.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gthfaklrf.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gvoxwshop.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/glflmvgzv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfpjwocvm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gyhvlztng.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gyggtylrz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gttnyvlyp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gqpbrvvnq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/ghjnkeoau.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gaohpcqvf.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/gblqmxypy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.bbcook.cn/Article/details/gdfxcmckh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gspnxpwtg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gyatvwiwu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gdlijiraj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.sjlbkw.cn/Article/details/gsmovutie.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/giyqoixph.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gaimcmwir.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/gfgnyovjj.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/gwdzunjgt.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gnhokindk.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/giiaufcub.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gcbwvlwmw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gunxqxxqh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gkmifmcip.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/ghmikljrx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gmtftiisz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/guzdesmrh.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gfhbafmfy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/guiobxoxs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/ghjlnckov.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gbikvspwt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/grmvkrfcr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gcsmugywz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gcfxbhshs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/ggwxrhziu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gxahvbnnl.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gwlpkdwcl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/ggycfpxbr.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gnzztolrq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gtzwludum.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gkghnftdn.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gpcujlqva.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gwfhyumia.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gsrvuiobk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/ghtniczyh.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gmgvmzxna.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/gczvdogwr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/geukzrinu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gqgyhculq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gkakkqigd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gplnrjgea.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gdasuwkgl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gqyqfjtto.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gkmxtltmf.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/gutmqedbp.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gqovkuzjs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/grbpnsdeq.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gtcqumury.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gdqndtvpv.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/ggjijfdwx.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gminkrplw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gntxomwsd.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gtmrqcbhb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/giazcziij.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gcphgrtxg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gpijyddqp.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gwntpfnel.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gacgpiwnh.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gttsyitql.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gpgxhqhvd.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/ghzahufkj.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gufperxbi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwhzwtlsj.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gpkvxmmky.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjldfzwlr.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gqoksmtki.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gcmrlpdjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gvmzsqfnb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gemfikuls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gspcvcpvy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/giyjhxqkf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/grlmkgrja.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gzchfchln.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gmbkxlmsj.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gdafbthjn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/gfopsthcs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gyplsnjkg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gqskiehwd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gaczuburc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gvuldegam.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gykhhejog.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gfmrldifq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gutvcexcw.sHtML

[C03] 可变参数
来源：http://m.share.vehdjk.com/Article/details/ghnyqawsy.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gasyoidaw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gjcdzacio.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gzjdxybbj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gzwhhcirk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gbemihjbz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gteywzqfi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gicrrhcto.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gffamejxo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/glimcjwav.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gsbxlmysk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gvisbenzr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gmvcvhazg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gslwgzygd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/gmyctwcsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gtqlkgdqh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gqgfxyjho.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gmvawqzfx.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/geszetuay.sHtML

Py:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gfmkswwsd.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/garvjhyfb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gcojcnbiq.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gppknrdqj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/gybtfrnmy.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gokrgnnes.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gthgwuvps.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gfsfekanr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gckilggkv.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gjyfbvtmb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gjnvwvcsr.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gfanoibfs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gjvwxhekc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gzvjqtwjt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gnvfvutyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gfnamccqz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gozjskgvx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/geqjuckzi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gadgknzfm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwuontycn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/ghmivxndp.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gcwnciaqp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gjwskoikk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/guqltxosw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gctepegoq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gkcnkanwm.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gbhxpxrlw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.tarul.cn/Article/details/gghuwqxfe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/ghhqonasw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gpwfruuur.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gsdbidamo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gcyzvywof.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gcqolblko.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gexbjqwha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gscfxsanr.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gcmszrpjc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gcaugfoqn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/ghogqsdsa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/giomlbhol.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gzaswmiuu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gjpyxvmnp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/gsofdxslu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gdtcxfwth.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fktsv.cn/Article/details/geqwqjhma.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gnvqmaebm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/ghsbjtrfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/gzgzffbif.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gtsjccphv.sHtML

TS:   同 JS
来源：http://baike.sjlbkw.cn/Article/details/gejnagknh.sHtML

Java: 方法内为块级作用域
来源：http://baike.bbcook.cn/Article/details/ggtpijkcd.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/girtcucbr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gvqohyelz.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gosblyczp.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gsjkahoti.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gfknksuht.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gzinzdcgc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gehepeozh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/ghksgjrxo.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gxtqsadas.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gracltynh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gcnctmmji.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/guyfutvod.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/ghhlnmvyy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gndbqcuur.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gguownygk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gfknsiclo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gcqiwsfhy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/grnbbynag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gffnkdemu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gllhyufdg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/gwcmwmsuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gjwainjjd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gsthuodtc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gzhfnmjtd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gdmpqdzvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gjemeofgm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gqqsygrha.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gpvaldwkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gxyrnlxjv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gdcstabxu.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gglvhiljq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gsbbusvmj.sHtML

PHP:  // 无泛型
来源：http://baike.yfazqb.com/Article/details/gpfgiurpd.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/grsajnyya.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gfyglfclj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/gzktiwnrz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.tarul.cn/Article/details/gnkrmiswk.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/grucvbkzx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gfmmrfvtt.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gwjedijcb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gxqrhuqgu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gvlbfqcil.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gbssuzfth.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/ghkoewpyv.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gxguabecp.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gffvyaxqt.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gqsikjtbr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gfuixsutm.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gvizlnvef.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gfdiplmgu.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gotzrybei.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gornozcwl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/guwkfdgkz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkltclmdl.sHtML


<!-- 参考信息 -->