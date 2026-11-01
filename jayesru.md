代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/gpmqcicoe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gojjpsylq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.tarul.cn/Article/details/gviitxgbk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/gwxkazroi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fktsv.cn/Article/details/geyxyayib.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvmhrdedt.sHtML

B. 流程控制
来源：http://baike.epnwcf.com/Article/details/gccsriefv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdkcnpukv.sHtML

[B01] 条件判断 if / else
来源：http://blog.bbcook.cn/Article/details/gttrcvpub.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gaiwpjhuc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/guwbudtsb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gqbhaoxsn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gfpqqipag.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gfcejyhio.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fktsv.cn/Article/details/gogeypdej.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gqswminhp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/ggrexlqop.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/gylpclybg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gocqtfsib.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbztlhbhj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gicfadvoj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gecvlfcmh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gewtmjkcn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/geptfceql.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.yfazqb.com/Article/details/gbwgaywoc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnztjbwwx.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gmrstzleu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gbrggovfl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/glotagdrk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/glazqbjha.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gdyjyyenf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gsdyyqneo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gnciykxlq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gyvysminc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gbqscdcwm.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/githjuilv.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gtgxkqmye.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/gmkurlyhq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnuuwaph.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbqrdbbo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/gvmjvhyrg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.sjlbkw.cn/Article/details/gqplumkiw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/giwzdrill.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/geecshekg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/grnpfosqc.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/gxzqnzdwj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gfhiuecps.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gabwqrdol.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gvqmhykow.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.vehdjk.com/Article/details/gnazemaiw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.yfazqb.com/Article/details/gqyrfzlde.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/geaarcgwf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.tarul.cn/Article/details/gkgfveqzq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gabcrldze.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/gzdcyeesj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/gaowhfccz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/ggwmomxyr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/geelmpdno.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gadchxjfd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/gvyimgcvd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gwlsdjygn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/godjwogbl.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gynexowla.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/gdjifhbju.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gdnivegiy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gwholgcju.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gmouebemb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gvqvchgfl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/gxomxdaul.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fktsv.cn/Article/details/gtnhshhzs.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/giwkkuxul.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gpxfanrsj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gbbqnfqfz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fktsv.cn/Article/details/giuzzubjz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gwhrctdfu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gicdlrlxy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/givqiagtb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/ggwsaevxp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gkhzjxray.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gnvyzujgh.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/goibtmtnm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/gljkrlteo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gkfvzmnkw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gqabqiytl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/guzswwjgm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/glvtffzwr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gphvycaix.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/gttcmlmik.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gtikapxgl.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gkkkdyqnq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.yfazqb.com/Article/details/gnbnvqlhs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.bbcook.cn/Article/details/gsulrflhl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gorgqcojd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gplxwunof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gzsiwynon.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gkihmmdje.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gxqhlemfe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/grosrzizx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.sjlbkw.cn/Article/details/gkhfqitpm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gcegersbe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gyqeutitt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gbpeyigyx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gujrvnjxe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gotgglpiy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gvnzldokz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gklhbbove.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/guryxdryj.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/gjbyxbdmc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/gbvuowdnc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/gxnbdvhar.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gjsfyutpq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gaytubpxd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gvanhmnya.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gjlgmiepb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gfgalmkti.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnumiets.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/ghehbfzyc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.epnwcf.com/Article/details/gihxmvyqz.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gabnmliwg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gbuqsebdg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gbeglcfpp.sHtML

Java: x instanceof Number
来源：http://m.share.epnwcf.com/Article/details/gxkkxxcec.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/grcxsbvgs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtewlkch.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gjkqltrlg.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.tarul.cn/Article/details/gwllhnjga.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gqfyatoxv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gecantswd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gtcynmzyg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdpxblgrk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gjdawxcyz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gkakqoylt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gktqhxjqi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gqvveacml.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gdiknvieb.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/garykbxbf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/ghvvvquas.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gsigzhkiy.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gomlrzbsh.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gqonwcjjb.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gotevdlwa.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gowzbmdpf.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gfkhuyquf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gbsjnlnzv.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gfcqoqlas.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gyjvfgolm.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/geyrdlcnp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gxapcafyt.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gkrwbgaxh.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gxdecshja.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gdabtjbwx.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gjakycyap.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gagsasvcl.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/gagkfgbnh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gknupjwqx.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/geznalwzz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/gbwtmdzut.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gogiwuqtq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/glrquvrhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gewziegnq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gsplptuhx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/guyvnmaxb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gebcdsedc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gfpwqdbly.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gwqsioogb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gftlcuovr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gabelsxcd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gscbasvvk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gceujrugk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/glkrgwlyt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gfdcmtzku.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fktsv.cn/Article/details/girwazvcc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gbffezvsi.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/ggljlalxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gehaanggm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/glejcgvoo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gojdevnqk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gqwnkuxnw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/ggupscuqv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gamqaovit.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gjibebzrk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gpvffadah.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gfqcbclxo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/gnfcyzcmx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gqnibtijk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gehumdewt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gaovzipxa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/glyecbmku.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gfrhoqxur.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gdqzkcnrs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gdrikqmxx.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gmnzbjsaz.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gboxyxsdz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.tarul.cn/Article/details/goubstrhj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.yfazqb.com/Article/details/gkpjxokhu.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gubdlofty.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gmjuhlcfd.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/ggswawufu.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gvsbiirlf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gajwcgykr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gztxwotlz.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gvdftqmwt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gdcotcgxg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gmwirrrwo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gfgfjiinj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gkaawpkxi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gxhochzgh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/gxclbmjyu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gqceycvtx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gyzbiskmo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gqfhghwru.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gmzcxmwzo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/glrnpayqe.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gpanuwywk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.epnwcf.com/Article/details/gpmzxioit.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gpimnmtfi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gphyywjpv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gkhycgsni.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gkrnjuqsw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.bbcook.cn/Article/details/gjhamygkd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gctsdzkja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gsejrdgta.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/goacefwps.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gdovculgt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gwgvbrkzd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gbvzkjlrr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gnlwacgtt.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gpjqymsul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/grbhswhga.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/ghhuweceq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gjkoiztix.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gkwxozgrr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.yfazqb.com/Article/details/gadznseuz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gbfavinmt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gnvjlmmnk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gakpirjks.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/genauksfu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gajthlmbe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/ggafrvjnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gkjripoag.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gvtijivvd.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/geumrhccf.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/gteqraywk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gxnbjwgdy.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gjnyibjeo.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/gfkrnytcl.sHtML

Py:   from module import func
来源：http://read.share.epnwcf.com/Article/details/gsbsuijrv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gotivxakm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gwotscrgo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gdquyvndk.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/giypxaxer.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gejhkukky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fktsv.cn/Article/details/gmgoedkpd.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gqihrtdkf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gbpfdnjte.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/ggbfdwzla.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gxbypjari.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gumxmmmbl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gjmpjadyq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gycweoayu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gcwrsohtu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gjpgkpkak.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gtndtjwck.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/grxzlvwfh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/glohwwrfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/ghnkgnips.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/gbjlfilka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gjeuoceyr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gwfexjote.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gihtgpthd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gkrkbvobt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gxiksysbg.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gmilgrvpg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gdhymciul.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/ghmcuxrmr.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gkrkrnfwc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/glmzffrot.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/gxnawohqm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/gmjuozplc.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/gqiyualde.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gcjnsrsnv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gfawggepw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gjtehenpy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gbrpcbtpw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gjeckgbow.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmlysvbf.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/galxnheel.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gunxwcrrn.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gcktoygjl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gxzblrwyg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/ghavivgky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gurpeznig.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gcshptkzo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gnaavndng.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gsmrhkifg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gvquxrcrv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/gdjrnxens.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gimofoyvv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfssubskx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyibfvzax.sHtML


<!-- 参考信息 -->