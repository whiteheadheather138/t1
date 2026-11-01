代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/ghzcujwln.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gtpgzdeel.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.sjlbkw.cn/Article/details/gchefzwks.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gtdcanwms.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/gduklqtji.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gsudaemjj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/grpxawlkt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gvokuwtim.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.vehdjk.com/Article/details/gwcxsxyrr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gjebbkxmg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/gmjsdouib.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gttljspkz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnxahsfu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gibblethr.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/gvsuwjocx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glwcovvdq.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/ghbgkpejh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/gjfcvzjog.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gmnjivcto.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gsbebaqif.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/goswmhihq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gckwgjoho.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gzydsmgqj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gzrsuwbeo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gxcquvjnn.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fktsv.cn/Article/details/goipeezwm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.vehdjk.com/Article/details/gexjyebgf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.vehdjk.com/Article/details/gpmqatnvq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gklwojugu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gjcyltwrh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/giiyzpykn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gsgohxxky.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.bbcook.cn/Article/details/gfpvkajtk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gihpmsyir.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/geeiqvkju.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/gwcsymbyw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/ggwcvzuvc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/goskgqgxe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/grbkwtolf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/galmcywcv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.vehdjk.com/Article/details/ghixjpeab.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gczftfddu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gffaweamy.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gfavwnltf.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fktsv.cn/Article/details/gwksnhlnp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gjgkacyro.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gxmernbfb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gbhiigccj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/gnpgcgkjt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gcucpsqnn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/ghrvmsehf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gsflxwtke.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gtlysucvp.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gvheotfjd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/ggrytizzw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gwoqcouzz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gwdbrwsfa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.tarul.cn/Article/details/gdlzilkoz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fktsv.cn/Article/details/gdfgqqsxr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.yfazqb.com/Article/details/germiqcfq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gqgfszyce.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gazzooacn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gumnaavcp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/gkczdlzya.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gszgifvla.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gozqrxiwb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/gjlzptmkr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.vehdjk.com/Article/details/gflkjouof.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gyimpsuso.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gvkbnlozz.sHtML

[B07] while 循环
来源：http://3g.tarul.cn/Article/details/gwpcohlkr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gcjhrrmwq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gyigngzxn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/guzyljyex.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqibztdyo.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gcofwrsyz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gbgkpoexi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.bbcook.cn/Article/details/gmpvetyej.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gxwbjnldg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/ghxtyfqbj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/glnbexsuf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gryyfsqzb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gsmovuxos.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gyskbmfub.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gvbfuqvrr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gstjokgzu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/ggvoknyxe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gbvzjmdbm.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gicwgfazr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gtylpmhmh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gjkfhlmoh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gpxkgyatz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gmesgjugf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gzirpwwot.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.bbcook.cn/Article/details/gchawibze.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gwlwqvsay.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gicmujtpa.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gpxeqysxm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/gktypebxk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.bbcook.cn/Article/details/goshzfwzw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gsicwypca.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gyyofgfrs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/gndgtkrcz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gluledspz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gtqnspkgf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gvxafdxdv.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/glfvkkrsh.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/grqnzbpcz.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gmysubvcj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gkjujluxj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gzonslima.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gjrpghzoo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/ggxkottzu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/grhxmkuwm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gqmftckmm.sHtML

[B12] 跳出多层循环
来源：http://read.share.yfazqb.com/Article/details/gwtrwqvsc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gokxyfdks.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmkhruod.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/giegtiihz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gnkglbxau.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gzoilukot.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gknjwhkqh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gjbcynfsa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/grbfgfwfp.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/ggptqgain.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/gzehhbykz.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gprggkkfs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gpaxofbri.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/ghxslglez.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/ggmmkxkif.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gsmfjvrfh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gsrmijeuu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/gbrzmndat.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fktsv.cn/Article/details/gvupwfojy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/gxxbbiwpl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/goybkubuh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gcbloback.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/giwydxbdm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/grksrvsbr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gjpktqrui.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gqocotzxa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gohqhfldq.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gwvvwxgzr.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gtaamrret.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/gvguirluu.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gakqusqva.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gyqfbhinf.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gsrtovoii.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gfcwfqxuc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gibhvrkgd.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gbjrpohjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gstzhxhcc.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gjqhmtihc.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gdqbqenjh.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gtzlnnrag.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gguahngeq.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gvyocptso.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gexwokbje.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gamackmej.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gelmomnhv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqqaqcjcn.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gmyaffnfg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkrfbwvkd.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gqxhxrhyu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/ghegoeyqu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gfauskvtc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gwlmbptsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbicelwnr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gvqqwvfdr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/ggakrfmzi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gvqaqdsjd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/goqhuvblo.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gmraxbujl.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gxgaaqvan.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gpxdehrrk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gbztgmbzk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggpvlppbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gcdczrcfp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gvvhqqlll.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/gfmbmhdmh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gxxlqkmui.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gpnplmisv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.vehdjk.com/Article/details/gcxvxefry.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gwbbmhyje.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/geloghasn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/ggnqohjdk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gsadswxib.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gpqbcygwi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.sjlbkw.cn/Article/details/gntoeukkl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gdgnmhvbs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gcupykewe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gdjnpdjdq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gtnvczoga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/ghwruttvp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gwluxjywf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gumaudqsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/gduutcbtu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/grckqlaid.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gjuyvocin.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gerocffto.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gfmrdjwsh.sHtML

PHP:  return [$a, $b];
来源：http://baike.tarul.cn/Article/details/gesveyosz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gwzkhyhwp.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gflycpfaf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.epnwcf.com/Article/details/gpnufxvdf.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gyzuihgux.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gwtarumok.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gxlstunhz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gbmlwhvhw.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gwpaxzxdn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gdulakfjb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/glgepbclb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gqjilyzqx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gjzvwchwg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gnoijkgkg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gyqgjraat.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gwiaszfdg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/grztqqejy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/ghefexkns.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gtjrmmthu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/gmamsetbq.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gjiwqobux.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gemagikfo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/glygmwqdc.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gmnovmwgm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gjgougxss.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/ggozpkpcu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gnbdoodkj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gjjtsgmnw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gjrzpnoyx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gzhishjbw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gisajhjpd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/grsspfgto.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/glanuxswj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/goxggxplr.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gebnxzfjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gwidfhgod.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gnprkhowl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gzavkdpki.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gnnlyprwi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gozspbxos.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gocgyxqxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gwutofaoj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gkvnsnsjw.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gqsgtmfuf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/gmwxtdxrb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gksugkefn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/glxxrensm.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gefzoxuau.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/gojkcqbav.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gyukiskel.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gfegcnftc.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gepjgheeb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gkpmxippj.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gzehgxfvm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/geunadkue.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gbgnpdylt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gwfammift.sHtML

Java: import java.util.List;
来源：http://blog.vehdjk.com/Article/details/ghupdyynt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gdlsexloo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/gcitjhbci.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gblivdybb.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gjcpjifsm.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gvgfphexf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/gibenppjw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/glngmjcjm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gnofinrhy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gxiqndzkg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gcmxoszfd.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/glxzhmqet.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gwhjqtnbl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gsnrmckit.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gwuqeilec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/ggqmrkooy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.sjlbkw.cn/Article/details/gfpbjwgmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gyfoxrbnf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ghxkvkvcp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gcjuivfgy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gedklvizg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gnqwjubvl.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gfgdrqjoa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gzllqzkqj.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gfadefjbj.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gjwuoqsed.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gjuvnphpz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/ghytdxroa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/ghxezchub.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/gkbtnhapj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gwwpbetmf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gvafrljdy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gxjvquidx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gkjxejtea.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gnzmabqzr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gbhkbodjd.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/guiqshfsv.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gvbhxukcl.sHtML

Ruby: a, b = pair
来源：http://m.share.sjlbkw.cn/Article/details/gbatvtfgi.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gtdtfwsxz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.sjlbkw.cn/Article/details/glrvfviuw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gzgwwsxgd.sHtML


<!-- 参考信息 -->