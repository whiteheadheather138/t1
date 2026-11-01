代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://m.share.fktsv.cn/Article/details/gbntdevyv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gzkdtrxem.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/grzwlkihn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/gjefursja.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/gokfgusno.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gpxvputkd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/grlifqmxn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gpvbzfhzw.sHtML

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/gphzqjmrc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gwxeclwfc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/goxraosix.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.bbcook.cn/Article/details/gizjqnffw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/gjzxokmxa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gjstcwppj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.epnwcf.com/Article/details/gefntfttp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/gcvqrwgbh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gmqixpfpy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvbqxfttl.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gbflwcjwg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtrwackze.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gcfcwkecq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.epnwcf.com/Article/details/geowfewgh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fktsv.cn/Article/details/ghimakbok.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gkutvfygp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gnvyslxjp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gfngzzxek.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/gefkssdzd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/gvogsaqgt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gptxrtggl.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/gxtbhzqxo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/goathmnjb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjwemrkxc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gowbdfjrr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gjyuumume.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqkgwyui.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/gwkcirebd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/ghhvvjget.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gvkvrsqig.sHtML

[B03] switch / match / case
来源：http://blog.sjlbkw.cn/Article/details/gnbyqqhvj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/gqhgjbkqg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/ggxjcqrpf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gxjwyleou.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gyeuwpyvi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gdrhnqtbw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/grhumybcm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.tarul.cn/Article/details/gcmyizqdf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gmfzattmm.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/grylfasmt.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/glwnnqqmb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gefwpqwru.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gfqcoapud.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gnxzwnbkj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gildqstld.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gqbobuity.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/gruizukfm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/gndfopven.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gojyovdyp.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/grllpxkyn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.bbcook.cn/Article/details/ghimkphsx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gxvdzgfwz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gslwngvtb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gaesieyco.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/gsbnpcqeg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gagrtsmpo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fktsv.cn/Article/details/guejoqgfo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fktsv.cn/Article/details/gjjaebvdy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gojtqkurr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.epnwcf.com/Article/details/gcbzzlnsb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gvwymochd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gbvmilvqj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gkjnhxqmw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gqywxazop.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.yfazqb.com/Article/details/gmhtbxued.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gdvvlzijp.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gazppmkbx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gijjnsqoh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gdmqtglxz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gikrtqxgg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/goioxzxyq.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gsnvhspnr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gvobdwkse.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/glkkizrgv.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gwctvlqem.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/glfexsdui.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/ghkbmdnco.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gxrkwsqva.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gsswznknj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gjfhmupdk.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gesmwyvge.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.bbcook.cn/Article/details/ggssbtgqc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gbwwaxhpi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/ghbqsjxjv.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gbdlgeagk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gpzntyofd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/ggrmcginb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gamnwehfo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gqfidhxnn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gsdhydxnl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gkymkddiy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.epnwcf.com/Article/details/gwyrqfclv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gicdiaeux.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gdpmxnnkc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/gliuriugu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gpeypnbwy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/ghhhtydjv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/ggbzyopaa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gvvxftslf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhnuqdch.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gdicakkei.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gsojekthk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/gulhxdyoq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gmubgulwe.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gkzvylkjz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gwcfbcjjb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gamujrzja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gnvwtewly.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gchyujbuq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gdwnkeukv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gejzpikpy.sHtML

[B12] 跳出多层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gzzkppoue.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/gjjzzhmpr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/ggawvjyvr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gfrbaqyea.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/glzplubxw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gvarszirx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gvmrcrdie.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.vehdjk.com/Article/details/gzgaacruh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.bbcook.cn/Article/details/gmpncajih.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/gnmrsqgao.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gwvanjjkn.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gkvicmrqf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/ghktrqmxg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gdithtluf.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gllbnmtnm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gndnivtxv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gncamoddj.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/graftzxcq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gwrvjtscg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/ghflqzley.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/grmufifbg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gxcmmdluc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/grxfbheek.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/ggtwdivyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/givjupqjw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gvjblcsgh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gqrjmgnns.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gjkcevtpk.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gutiekvza.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/ghlwghzwi.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gpvnfrnru.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gynrhnxko.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/grdjzftyo.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gcqebttwi.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gmhnyrmsw.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkejksvyr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/garqibrnb.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gzcoadliz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gvgdcjple.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gcofecbkx.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqleexoo.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gpwscofhy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/ganxfkeuw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/giqgdckzo.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gaitzbrrg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzqnqwzul.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gzkeqedmj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpwpwhkuc.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gizyjhljh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/glclcirzs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gtasmyixf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gnmuzqgxe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gcwvvcltl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gfhbyfxli.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/grjcxubws.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gwjtwjlrv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gjllmmyow.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gqnbbczlf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gyofjbqnd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gkipkgcvg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gaflitufp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/glrbspwbs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gmhgzulhs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gdrnbnder.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gdjttursm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gsksjfsxi.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gytyzerzf.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gzbvauiyw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gnoluxndy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gxnejbzpe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/glcnzufac.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gkbyurgxh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gvsjfzbek.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gonzhhtkr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gzivreqbr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/ggmedeycq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/gjajblqwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gbdembmah.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqeakphhb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/ghwoqfhzm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gwdkssdsf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/giyiywsbd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/glffpurcf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gdoaveync.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/ggycddgpb.sHtML

Py:   return a, b
来源：http://3g.fktsv.cn/Article/details/gfvzhenji.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gofzwjjtj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/gqunzjtvu.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/glzgspgsk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/grnksxmif.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gapvxqygf.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gadftfxon.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gwglfzmiu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/grxjcfidd.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gmftozmyz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gfjtotrnc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gnrphfcob.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gnmibnacr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/geyzjufwo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gbptlhbhz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/grfvaggcw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/ggpbqhjbu.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gxufbozrr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.vehdjk.com/Article/details/gguslfppv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/grzaaszlk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.epnwcf.com/Article/details/gvqebijuo.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/giokwmxdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gyrzqpyfs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gcfhldjsw.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/gquckluvu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gtyaqjhaw.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gpfaaqjmf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/gbgmhvsxl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gquhftzly.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmlbpwskh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/ghkpbmhga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/ghkaineec.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/ghzmqpalx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gmijnbekj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gdcyplsjv.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmlvebfy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/glhsxdomn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gganadxtr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gyrwbqvcd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gfwktxlew.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gneveqxfc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gmbzomimy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gpnsougwy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/ghdfdpili.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/ghtoktstg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gvottlauy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gfflgbhpz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/ghpjvqhql.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/gqrbvpexj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gdbkqgivs.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gsbbhsqjc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/graihvjft.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gcqmajchn.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gqgprqsyf.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gdnpyfqpo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/grzawunuy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gnsbzspgv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/gfpxddvqz.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gkznrukbl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gfcdxdujb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gcaxjkqkj.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/guwoojhak.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.bbcook.cn/Article/details/gpgubcmot.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.bbcook.cn/Article/details/gpxeoiall.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.bbcook.cn/Article/details/gbbxucmsj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/giuermlxo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gygpfjyoc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gexlyjaxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gassvqpam.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gfgkvtewv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/ghnudqcma.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gttobrefs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gwhbshrml.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gfudclpph.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.bbcook.cn/Article/details/gzzhxodyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gosgjtprw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gzdorgvui.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gfxxdldzl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gegcbczwv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gowzsobvi.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gqrvqnbev.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gifsbndww.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gcbljjvip.sHtML

JS:   // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gwemybtwh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gjnxjjpam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/gnpgxcuxk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/giplqtsty.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gmiymtzvb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gbkmlfxpe.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gdtnxlgml.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gpwbazlkp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/guozxddee.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gbrftthta.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.yfazqb.com/Article/details/gvoyaxjfe.sHtML

Java: // 无解构
来源：http://3g.bbcook.cn/Article/details/gdigdmdcf.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gmofrclpm.sHtML


<!-- 参考信息 -->