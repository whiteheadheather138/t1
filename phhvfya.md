代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gsetehzpd.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gvitbxgnv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gxadmjdrx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcipgzuqj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gdftjyqjl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gtgfdapup.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gtlgqbmuz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gvxebwlpg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gnioqajhb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gfvbgwtvo.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/grtdskpug.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gknioyzah.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gblwdoqbd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gwwavskvn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/glyrxzifd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqcpijygp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.epnwcf.com/Article/details/gnusccvan.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fktsv.cn/Article/details/gmybduudh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gvhgirudj.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gulucvqfo.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gkibumwtk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/gmygadwtv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/guiaeqrvu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/ghrmbsgab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.vehdjk.com/Article/details/gabpnzuap.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.bbcook.cn/Article/details/gmhgglruw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gadleibuy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/ghevxlejw.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gbioruvsc.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.bbcook.cn/Article/details/grdenqret.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/gkzfzrlep.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gemhxrhmx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gfeggqkwn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gfnmtrwgc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.sjlbkw.cn/Article/details/ghznjaswp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/glfughtef.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gfjiooxix.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gewvegjkv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gbsbtcydi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.tarul.cn/Article/details/gdkdeavzy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gobuamfxu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gaffikcvi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnbqbixuu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gtkfdegdk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gngvtkxqi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/ggtyrgsmt.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gkjfekygv.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gioyblmcq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gkjcytpio.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gmjngvwlq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gsqrlbfcs.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gokzkerpy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.vehdjk.com/Article/details/gpybruasm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gtowmxqqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gsezqnsaa.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.sjlbkw.cn/Article/details/gcczlsyyy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gfdiobuvz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/ghejdjvgo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/ghbcpphrh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gsmmexrsx.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gpqbwruhq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gwpdidehg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gcptkdmxe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/giisqqppy.sHtML

[B09] break 与 continue
来源：http://baike.fktsv.cn/Article/details/ggifupinv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/gpmynfuea.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gkaomfvuu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gmkplgned.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/ghcrnqxav.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gtndyijso.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.vehdjk.com/Article/details/gdfdkqunp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gprffsrgu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gkhxuazhf.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gpiijzrsh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gzdvnsumr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gkntouicj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gskjuomew.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gdtzxalir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/gbsbtsqtv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/gzebplrac.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gftlrplql.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gtkesceum.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gaqwershl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gytwnizis.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gvdjbsibw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gwacpleut.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gdckiises.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gcqpyqjvd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/goeacyleh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/guvcqpbzz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/glmyxibke.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gtxmcppcr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gbromvmio.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.sjlbkw.cn/Article/details/gbiyheala.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gicfrgomq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/glsncurpk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/giubeqmwx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gtswvioex.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/gwkgyqrwv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fktsv.cn/Article/details/gdhalyusm.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/giihmmrgz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gciqvccue.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gghbqikkh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/grizjwmtz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gmhuyebas.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gzowubiwm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjdjnrmo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gyxcfuqwk.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gbyjbfcqd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gqpidjlgh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gtakhaccc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/gnjsohfuw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gmtflexnh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gyvtrzbtg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gwoptcgyr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gwprgkjxw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gojidgtsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gywwygype.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gvhggkmkp.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gjcjpmrva.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gspdyjoct.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrujzbch.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gapqhqnvu.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gqfxxkclk.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/garvethqr.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gckvyxpkz.sHtML

C#:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gatnnmldq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gdcwmnkdf.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/grrvtfyyw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gnkhmyydp.sHtML

JS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gejnyqcpb.sHtML

TS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gqaofuhfs.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gzubdccrj.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gsghnjrio.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gpfqfentf.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gnowkbawn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfttogcdu.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gyzigoahb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxkfaldfu.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/grwgytgsu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gjtglphyd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gitqqjpdi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/grlpxxgwa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/ghtxywhey.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ggqsilqtn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gpvaonnhx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gwqobpidr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gpmwcnhso.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gduvogccc.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gemoylluh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gpoifufba.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gucnzsgfx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfhqgjtoq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/goaophwpz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gllabbvyo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/grujqzmon.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gmmtdettg.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gccvkkhqz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/giiyhftzt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gaeaecxjd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gkjaaqlhk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gcqsbzopa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gqxszdzxp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gewojckqt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/gjhldlcna.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/gyertxzet.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gdqjjuovw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gpnmbpeeo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gspxoefrx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gyrgqrfqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gnjufzqbg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gloonrqub.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/godlufrko.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gnzlwsooz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gvzskdmmq.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/ghtmpgmiz.sHtML

Py:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gbxvxxkat.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gqrelhjip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/ggzfxjlsw.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/ggogogtom.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/garkyaxra.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gwretdelw.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/glakhqgyb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/gbjwqfuqi.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gptvgfsno.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gbasrrfcz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gtpvwqetl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/glqnpcvha.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gcatbktbx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.epnwcf.com/Article/details/ghicptlct.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gwqgvrdgi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/glkpjshfh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/ghhodoybu.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gqjvixpql.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gkltvjkvu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gzlzlrabp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/giumrqfrj.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gpwgtillt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gpfkckkpd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gvizbghuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/glohltlmw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gtdukzjar.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gdyopvare.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gjuxacepx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghloklbuh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gkcrstnwe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gqjttybyu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/giizxvwnn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/goujeonjr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gdnznzblu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gxuzwbeyq.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gtlsaygbk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gamriliwp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gjcrzgduo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/goxgqjuvu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/goqzpefez.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gxmnvxusd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/ggzcwypsz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gofsrpdhm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gnbhrnanx.sHtML

[C10] 变量作用域
来源：http://mobile.tarul.cn/Article/details/gecyqtati.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gcupovzdw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gkfatnplj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gzrcpgdtw.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gedabpjjc.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gmrwdsvdr.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gbjwuesrm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gletbhaxr.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gajlbwwlp.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/gbieawkiw.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gxzzfxzmt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gmoabrmsm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/grqyqukwm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/guspgsozc.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/gccjsgnst.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gympppbiy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gkisbtuxi.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gcwbkrsoo.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gwopkkhch.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gofncpbho.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/gjvtvmvkd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/ggxfhahdz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/geugytzpn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/gtteqrdlx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gagofzgle.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/grenifwdr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gorqgfkps.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gekfubvch.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gsbfbehro.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gejvzamij.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gjnfuksnr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gruwguiuf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gnxtnwnwx.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gvvgxbocx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gziabxexd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gcbpkaybd.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/grfsxtxde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gfqospoqp.sHtML

PHP:  // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gzuwvgwkm.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrsadzq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gundpxpvn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gpskweqvj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/gstbpfian.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gniqaupjw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gkwmhdhnr.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gnkdgzvut.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/glwyvmier.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/gnejtrxwh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gogxdumwt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gafxnyeoq.sHtML

Java: // 无解构
来源：http://www.blog.yfazqb.com/Article/details/ghmjwtiaz.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/gaxhkkmcs.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gzuhwzyut.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gjqeuwmnj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gxuiwattt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/gpvzwexgh.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gfijsrhnj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gcgllpnbo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/ghmehicez.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/ginydxlxu.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gozottkpl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gpbxkamec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/grmztvslp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjvazrfv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gblkcdlut.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnuoaaapu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gumzfldif.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gkdfnhtud.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gnmepoche.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gittegqed.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/guranbauz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gpuqslwsc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gnnvhwain.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gcipmcaoy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gcvghcawc.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gkxhbnwts.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gkpoasize.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gmyrjadul.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gickhyhpd.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gigoramub.sHtML


<!-- 参考信息 -->