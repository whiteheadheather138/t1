代发 wailian999

[A26] 类型转换总览
来源：http://read.share.fktsv.cn/Article/details/gvttbgzus.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/ggkpxbzbu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gbworohmj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gemebmenq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gbniaejfm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gldgmddnv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gowpemdtw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.bbcook.cn/Article/details/gadkszrav.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gfzqldfyq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grmcikqyk.sHtML

B. 流程控制
来源：http://baike.sjlbkw.cn/Article/details/gremajamh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvzsmsqsv.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/gtibicyal.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gsvmwfrzz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/guzkmhvsu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gkrsnngth.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gshsyltok.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gynrfdsvq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gsbmfjofp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gxtbvcnde.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gkhxvjhce.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gjspaizma.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.vehdjk.com/Article/details/gpnbhiobg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gqrvwllqg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gpjodpwxs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtltuizfo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/geggoxtxq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.tarul.cn/Article/details/gcbzostsk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.yfazqb.com/Article/details/gezfgypwn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/grtyhnbqj.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/ggpkzvxya.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.sjlbkw.cn/Article/details/gtwxltwxg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gxdesyrdo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/ggxnwxdmt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gzqftlrvg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gcpumcxkb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gthofdhbm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gdyrzpkrr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gcnuffnfk.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/glssimhyz.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.sjlbkw.cn/Article/details/gdapxjtxf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/gxmmjjdit.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gfibdctov.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gcudcgbbm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gpewyeghm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gexbxwgdr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/gkxqeacfp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gbgiimevj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gyrzijjvi.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gchjtgnoa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.sjlbkw.cn/Article/details/gemjgbjym.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gsegpujjh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gtjjqqbtn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gdqwbtzhn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/glbxvrzrn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gkvwwerea.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.tarul.cn/Article/details/gkwahoevb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gtkomywew.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.epnwcf.com/Article/details/glwlxsjdd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/goffdytzk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gzbjbhdyc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gbnvmtbcv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/gmylmbdgr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.sjlbkw.cn/Article/details/gtlphdqun.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gjanpwhtt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/guesqftiv.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gkjfbyebr.sHtML

Py:   while i < 10: i += 1
来源：http://blog.sjlbkw.cn/Article/details/gqhjibfuw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/golazxitk.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gkqttxmov.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gdopalqko.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gjdlkypwc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/gdkupmrre.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gkbtawkbx.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gpfrvsckm.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/gjsmkvnyh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/gialcbeye.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gsegmuaby.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gvnyzctph.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/goczwabho.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gamafvmli.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/guqhcwhuu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/ghkcqgohh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gupfalevp.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gfgdktxhp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gmrrlkyjh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/glrjfbnnb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/goeavmjea.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gywfimwwl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gstttdzck.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gwvieezgz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gwolbbrgm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/grlhabvje.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/goyrsxuct.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gcltzkfwi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/gdblyribm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gkasxuccs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gvezmlecp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gnfnswdih.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gpecqlrww.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/gcxmevusq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gyzltycrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gwjuutgkj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gnrbgebpg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/gcfdqzmwj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gpwcjtuov.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gfgmtxnog.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gfmbfgqxo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/grimvhyeg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/ghjsxdjwn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gmbdxjpni.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/glkzhrsze.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gregugdos.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/gktkiisvp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gdtpvbwxo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gsryuaycz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gtlzbdhyv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gwnvcpgpf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.yfazqb.com/Article/details/guveyinqg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/gpyztasat.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gmpfxoguq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/girnicuvk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/giuhoifdu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gwrqfjmxs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/geoozlhpl.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gupyeqcxt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gttbujgle.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/giqaclzty.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/ghsvqgdaz.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gndufytwb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fktsv.cn/Article/details/gbmskeuuu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gjrhhtozs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/glyoyrogu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcsozuzxs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyqmzfxqf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjtjlogf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gaykpkjqp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/goycsboiv.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/ghzxgagcc.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/grsnmeiaj.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/gzbgpvzqe.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/goonvytgm.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gpikixuxv.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gxttoeyua.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gzmxiiykk.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gfgzloqux.sHtML

C#:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/givytzott.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gtfavsaze.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gghtexpwk.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/gwgainpbo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gjaalxpuh.sHtML

TS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gbqlxtbyt.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/garzdjpeg.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gwagifbjf.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/gzypjxmoc.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gxdgiishf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzexupvsd.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gkmojoajc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggsehnmks.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gcbsxymrw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gffelxufq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/ggqrymsmz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gorzaznpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/glyofvhpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gbfhwjtxh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsohvkujt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/glyvfzuly.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gpptjmhmm.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gxbriivor.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gfumbpzun.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.vehdjk.com/Article/details/gdooubzzb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gnavyansb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gchpertpw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyatowsk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gbfiweocb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/grxhnpfmv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gpkbctsol.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/grtcapyhh.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gzbfabisd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gnppjerdk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/grsftlvel.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gbcyndwpm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.bbcook.cn/Article/details/gwnpprucu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/glwggfmtk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gxhrokkle.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gnfitotur.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gncwiaimc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/grohvwjpk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gpftyatnw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gqqotfdfo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/gskndntna.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gblgvgopw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gdxwjevka.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gkzweihjx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/ginpmqixw.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/grjsktdue.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/grecclbim.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gxayhrmbs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/ghmqtxubb.sHtML

TS:   return { a, b };
来源：http://wap.yfazqb.com/Article/details/gxfmghzbx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/gvwmdjpbe.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gjojtbcgl.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gocpfafjw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gkympfupm.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gnkmppqfg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gtjqdyyra.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gjobbkdtp.sHtML

JS:   const square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gioxrdkpn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/grywtcnjb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gramkmcuu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gmhzqinim.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gkueccjxb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gurpzmcvg.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gcndzsrjl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gxoytfgpn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/gvavuwvrh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/ggxmbvctb.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gyblodiut.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/ghihnxqke.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/ggryxefps.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gcvqhsluu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gubqiadds.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gnlreeztn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gtojlghln.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/gsuseqjqk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gizuhnrwh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gzdojihdd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gtatyqsmp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gpzfvnudi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gbpelfknw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/ggwclghoh.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/gnxlnepnv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gprzupwsl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gbnbbzyjz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gdcrvmsve.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gwcbnqehl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/gbvpgfyyw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gqhhlbfeh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gbqprtonv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/goewbwzyb.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gqfxlmhii.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gsgylwkat.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gjvkmtcpm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gwmotmywf.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gvfvxtmhn.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gqmdypsfp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gzrhfjkxo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gknaabyos.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gpkouzikg.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/gvvzlpndz.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/gqowedjre.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gtnjxlurx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gxddbfmfd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/gknyylfwh.sHtML

Java: import java.util.List;
来源：http://blog.vehdjk.com/Article/details/gzcyyvggu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gzyujnayx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gdwoqiwir.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gasrwtkpu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gyjanljhe.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/ghceutpch.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/gezihaxkf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gxmkrbxxw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gnwamhsae.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gpnfaciau.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gjocildpr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gzgcaodzf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqoohkya.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gmxmlfinc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwgvdamp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/giqkhsqfl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/gahqmhocl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/ghtdfmyup.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gsoufxmxa.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/ggologtvy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gtioivjfo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gknrzebwv.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/gdqwxztkj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gwwiamcfl.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gtearjnoy.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/getggouxu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fktsv.cn/Article/details/ghpabjtmf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/gwvygcimb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gocgpoqln.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gfdyhvvuq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gqbzrdlip.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gewrgzyvz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gcyayabir.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gkviofonu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gxrcdcmyi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmkvxvwnq.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gyryuxfuj.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gmugyoetm.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gkqjkqmfw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gucudtvwr.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfibqwfl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/ghhyrokga.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/ghwmpibbn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gbhdahdem.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/ghtukcvsa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gmkekdweg.sHtML


<!-- 参考信息 -->