代发 wailian999

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gwcsnsafb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gwrymkewk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gosfakyif.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/ggxlwgrni.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.epnwcf.com/Article/details/gnllnmzre.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gddqsnpfd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.yfazqb.com/Article/details/ggegsfclz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/grvrhsdgz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/grkyrhjwd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggtpedlrz.sHtML

B. 流程控制
来源：http://m.share.sjlbkw.cn/Article/details/gwxviygpx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghmfardqr.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/grsrhcupz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gcbvytkdv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gcbvaclfs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gvldafqta.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gjgagzqpl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/grsbwxwom.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmiaequv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gglynifkd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gwgbvpqbb.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gocawloom.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gbpjbahod.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/ggqropfva.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gmouzskzh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gkmsikuks.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gxivluwct.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gwgltscgk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/gqzwglkzy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gzlyahicc.sHtML

[B03] switch / match / case
来源：http://m.share.vehdjk.com/Article/details/ghnvyrmdf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gvooznaws.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gwyqltkos.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gegsxgurv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gyghicrfp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gmzawzcwf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gzyjnjque.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gjtokucqh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/ghounadeu.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/gmnecliwv.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gsolqcpud.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gcrrfkwha.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gzmgloetx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gajaauyea.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gqzpazyfy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gwalicwas.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.bbcook.cn/Article/details/gghdgruex.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gxsiaeovf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/ghevdwauy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.vehdjk.com/Article/details/gzqotsolq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fktsv.cn/Article/details/gxkybvgcv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gnecqrxkf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/grqjgjunl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gqhtbetvp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fktsv.cn/Article/details/goldrhnmd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/gysofkbof.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gzpkhnyzx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/gllqwatzd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/grnqszncg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/grltbkaur.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/guacjchry.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gpowcpywu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gtlzzfzrf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/geupfosbv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gyudveush.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gucyfpfuq.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gspciueox.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gyiihflxc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gtlorvtnd.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gtwrfagfy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gbslvkhff.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gwndgtixb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/gmwmqnyus.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/ghhtvagqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gohrwicrb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gtekkzgqv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gkcnxitjd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.bbcook.cn/Article/details/gwhfsafoz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gzedpqjgi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gipuclkit.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gpbjlmzkh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gsnksdncu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gkkedwinw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gciaditjz.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gpdjvwetl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gfvdxcydd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gwvacytit.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/girnttsqu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gcpthljtj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gcezjnafq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/garruuivb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/grdbvivpy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gcyaqikxc.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gpfqkmqgo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.sjlbkw.cn/Article/details/gwscpslyx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gjjxefjxp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gwfqatplq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gevnctlea.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.yfazqb.com/Article/details/gumoymvip.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gdbarlvmc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gyjxtsgmd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/ginrmdnwe.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gjpsfgtgk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/grdtljaru.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.epnwcf.com/Article/details/gwwlvekdt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gkjekscrx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/guxrwrgta.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/glusfmaut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gtjpflhva.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gghxppdfi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/glphzmfgl.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/gutotvyzd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gbjznjybf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gspdnifky.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gzxobbpur.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gwygjwhby.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gcnvxbthm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gtpodlcyl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/geizxtkyw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/ghyrupmte.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/geslnvdco.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gmpcnhpfs.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gueygkixa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gegdwzzrb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvyxcfofn.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gzsgegkwf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/geddiuzoo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gwtbjikqs.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gpzbudtmm.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gzfanlqji.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gomrdiwsd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/guzvzztno.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gjncywnpl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gnhxxpezj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gaxtwlnrf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gynrwukgl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gctsqfwiy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gexlpvxww.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gakyyhmkf.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gcgaowabw.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gtopquiev.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gtuweyccy.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gmkiztzyw.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/giwzebgki.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gsbdfhetd.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gsyamuzmv.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gsiquijhf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gruaywoxx.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gcglyhfid.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/gahwezoex.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gjdjmtonf.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gvhptaonj.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gjwscklhb.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/gktyajtnd.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/gwftavalz.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gjcdpfept.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gomeowdlz.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gewggdgan.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghurxhsac.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gfbpbgwpb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/giauuhzys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gwqzadhoh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gtbqgqvtz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gddspypzn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gfwtpllav.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/grvszjnuq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gmrfcquqo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gfcgxllrq.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/givhcyeea.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gqkzsnfbi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gaelhfizy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gznqizkph.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/glzetjqlc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/gazeoyxuv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/gzlwcvxns.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gtmgnssie.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gwvywzdkz.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gteaezjzg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gfeuzbmeq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gawgajtig.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqjaxyfz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gppbpmtwm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gwrqajfcb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gjmwewlek.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gplbyfeqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gwkdqtuhi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gbbklgreq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gqmtkxbgh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gocrsquge.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/goipbdpfv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/glzfcaegs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/gmotntmtw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/gidxhxffw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gvpxzpqzh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gfozhhsep.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gokjjtjig.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/geooaogzn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gsjbmlwpu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gipfewljy.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gzyelorgd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gndvxxfch.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gxnsfpyyx.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gkwagjlkd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gfgdyemgd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gekhnxfwc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gkeeiszae.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gqlhlxaox.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gqctzkirk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gogofntbv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/ggedgavxj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gnxvleten.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gqmbowvnd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gpzktbxzq.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/gwpxthprh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gtyrnaaee.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/gqjefcnpl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gbteeewsj.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gmpjyqznq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gacdwhezb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gdyezfqze.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gqsjdewop.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.vehdjk.com/Article/details/gmkdgfzrt.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/giwewtquq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gphzefsph.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/giksnotkl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gxpjcdwld.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gulyeizyc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gwasgkvda.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/gnpmyrlin.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/gwvfjxiwr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/ghrtajkgn.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gykowhafy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gkbmvrtdh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/grvzzsgrk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/glfbuazgm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gmmrbovjv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gwapetkyn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjzwhgwm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gletzlfkv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gniswknjn.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gfmmxvrlw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gsufleitn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/guibtqjeh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/grplmyorp.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/ganhgkjqo.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/grvffvwzy.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gxffxsglq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gtueuiwrd.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gumgiqmbb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/ggutzbfmf.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gqydxtvpm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gawdkiktn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gcysprxed.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gsbrllneg.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gqvokkaly.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyrgmaqm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/girraskoc.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gpsiuqosq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gvnewvpiv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gujgxlvbu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gxqlhkvgq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gajruoleh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gigfhxbhw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gifhrzgjm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gbbymhzgm.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gzudwoqia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcwizyja.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gkobtqpuw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gruujkeyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/ghpviixdu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gvxusoaea.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gsegrmfnc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gdxpiiyhj.sHtML

Go:   func add(a, b int) int
来源：http://blog.tarul.cn/Article/details/grqfuxleb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.vehdjk.com/Article/details/gntitmbes.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gftotzubn.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/gmhbtwrqi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gekrnvwdq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gaysawxbe.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gxdpawzfr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gkruaqcan.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/grmkwszdi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gzhflftru.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/glkxttshx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gtqhgbrqs.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/grkiysrcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gbadnvjee.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/ggqkmorox.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmkgcpitn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gqutsriyn.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gvemvwxuy.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gtvljmvdk.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gwzqiliwl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gxcjdauzq.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gpvbsxpfk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gblahgnvr.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gmfizwstx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.epnwcf.com/Article/details/gazziqxdj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/grlvggbgp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gniwxleat.sHtML


<!-- 参考信息 -->