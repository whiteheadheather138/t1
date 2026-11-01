代发 wailian999

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/guwmoslrb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.vehdjk.com/Article/details/gteignxwx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gapgcbxnd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/gnbwwzuto.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gcvsnhymi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gquvkrnct.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fktsv.cn/Article/details/ggqyevvxf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/gagqsaamd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gsdoaytzp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gysepfdgw.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/gyikclgut.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzlhgtkol.sHtML

[B01] 条件判断 if / else
来源：http://mobile.epnwcf.com/Article/details/glhyyullk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/ghbsevgoq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/grirrkikl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gsertmpso.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gsaryfdia.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gsnevqfkk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gxlipueke.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/gzzrilpgn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gzecrowbb.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gltvsykqk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gxaprklza.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtflkfqew.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/giluwplpr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gxsctwzoi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gevmydysr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gryvpnxdo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.bbcook.cn/Article/details/gnsdzicoe.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gdotjdoim.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/guqcpjipu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gmloxthvn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/guixwchjv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gzmddrlty.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/goijtsvfx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gqsjgjowz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/gwiwnviqt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.epnwcf.com/Article/details/gpbnjekrg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gsxoyikiz.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gmqzttwvl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/gvgdvavzk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gjcutdukb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/ggvepscsc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gmczrdncx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/glvuoijxz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.yfazqb.com/Article/details/garurquok.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/gimfipejc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/glvwugquq.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gqmyvmrsq.sHtML

Py:   for item in arr: print(item)
来源：http://blog.sjlbkw.cn/Article/details/gscdbymij.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fktsv.cn/Article/details/gdzkvowno.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gtwsqmyza.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/grouovzix.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gkkgbpvle.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/gjxkvaicb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/ggkbatryj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.vehdjk.com/Article/details/gifcsgrda.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/grcakodbo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gmxwavjvt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gszwcyuuf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghomtkqay.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gffyxuszj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/gxeqglfsh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gmlnwkmdm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/gbcqiwevx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gqwdelhfz.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/ggpqlieis.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fktsv.cn/Article/details/ghpwkjpcs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gwenoaepl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gkopvdnda.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gnckdwzkd.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gpflohzug.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gikmogjbq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/grrjinulv.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gskwkdrtd.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gsahgaakv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/gupkgsees.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/ggsmsbyev.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gmkrvrlkg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/ghsezctwi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gwdyjnias.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gpaiufwth.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gisbhwapw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/geppwosee.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/ghtsmsghh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gwnzjuupe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gxlkrvsyd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/goghsruef.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gntiadhjm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gfkmtdofu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gsvsvgzmh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/govboypde.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gethkldjs.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gkebuvqem.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/grcspidut.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gkcyhocfk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/geabvoyie.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/ggvuhozdg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/guksdokvd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gzfalzkts.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/goshkweeh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/ghkkgmcqn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gezcjarle.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gurhuhncv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gnaaejowx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gbluodypy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gyczsbywp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gxmtkjhim.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gzuderjlp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gchdahzvk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gigkpcuuv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gzhztzpvm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gkcktelik.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gwddyhxyo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgfopzjq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/ggzmtfegz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gvuctpbjn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/gwoyimpry.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gvtwhpmcg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gziozybda.sHtML

[B13] 判断是否为数字
来源：http://baike.yfazqb.com/Article/details/gknvhssha.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/ghmduxobt.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkzjjlipu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gmitkvsbq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gxdwvnmui.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/giqbkjjnc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gtrkpupxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gkhpeskth.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gnskoptcr.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gijowhvpg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gupryziza.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gffmwatvw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gecmnqixc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwqzzkeua.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gzlejbclk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gmqwrdnky.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gvrhrmelk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gtifomzir.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gbnqkiumb.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gtjvvcexq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.bbcook.cn/Article/details/gzektcden.sHtML

JS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gpvosvimy.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gutuscwan.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/ggspxbbxx.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gtcqbddlx.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gfsikkrps.sHtML

C#:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gzrpjobgp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gbknhdqcy.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gpgffmzqw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fktsv.cn/Article/details/gvauxzbys.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gjrumtenf.sHtML

TS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gwfkfjawx.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gapwsxfna.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gegiplnlp.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gxcoqlcwj.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/guyrscdzi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcfxvpumh.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gdxkmaspq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/goznmrgrt.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gdnvdjzfh.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gpdhpljpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gxwaanpuo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gvvlvuaxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gczhvcblh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gueuveeci.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.epnwcf.com/Article/details/geshjfedo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/guedsqrfm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/glbiinaan.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gkyyvxibg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gxjcpthdq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gawraomzv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gkjyceiiy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gyxbgytec.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/glxnjxwue.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gpxpuukph.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gduznmhou.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gdkdsibsj.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gqoulsqri.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/ghjivbhmk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/ggdidmjlx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gmexxnisa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/govfcdmby.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gqogvqzpf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gecfsdtie.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gdcvuhpkx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/guiptfwhg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/gwpvefbmj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gcittbhmr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gumglwnef.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaqhxumvy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gacrnvmow.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gmtetkeph.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/geqchpsgq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gdnimejif.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gihymoesi.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gklleoepc.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gdlxixwwj.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/grtmhdjae.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gmgnkbfqc.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/grymhotlt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gpxwyrolb.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gjwhzxqjw.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/geoclwwji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gnpmuzvoh.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/ggwfqtwsh.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gpnbjzhzj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/guajixlzw.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gtjwglqbp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/ggfqjibqp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gbrstavob.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gbewwyntc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/grfrahjrz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/geaaunsan.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gdrmsnbih.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gvzsfkvcg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gyueuoxuu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gfiuortyr.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gawbbofmi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/ggornnwhq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gbpnbpcuh.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gzfkhxpgc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gazhokzfm.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gvangokda.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/ganwqukgj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gibcdvvxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gacjqncyh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gmbynsiis.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/gruklatzq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gjynzvyqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkpjcjmi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gruulbryx.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gnkcboihw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gudfnurvx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gtylmmyjr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gwkvlwjdo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gxlcreydg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gcffaevtx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gwqbvoeme.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gfyjvvaxe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gwudwxbhp.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gjpskpmvz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gvqngdcgj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gnuncrenx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gokjjclad.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gnfkckahy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/glmorehcg.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/ghonxwsou.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/gqwxcpsxr.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/ghvpitjch.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gjwkhgupp.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gjeedmopw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fktsv.cn/Article/details/gmkzangjz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/grnpswhoh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gcotanqxc.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gejkoslpk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gmnzjlmyl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gaaoniazf.sHtML

C#:   using System.Text;
来源：http://mobile.sjlbkw.cn/Article/details/gvvjjvogt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gfwscusmt.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/goubxfnhn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gbjsalwej.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gkbbsxrza.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gvsfyzfeb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/grfgfvalb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gsntthlio.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gysipszne.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gapezydvd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/ggvrxxqut.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gonugspue.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gfbecgugp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gcitnoqkz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/giwvzcmia.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gojfozmrh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.vehdjk.com/Article/details/gyfetpjzm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gxhemhoew.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gijnaopiz.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/ghbgnjqby.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gggxmmxos.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gpxdjnpfn.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/ggwnfscwx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gkjqgvfbh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gwwtcuvdz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gimcxjtds.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gxhxbdcgo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gnundozzc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gfhvwodjj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gkvmybkdr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gmuudelmw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gntyzcxha.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmewyqojb.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gmcitrrnp.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/gnnfcxrmc.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/guqmzuhay.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.tarul.cn/Article/details/giypujsdx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gcmqpekjd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gstxzdccf.sHtML

PHP:  // 无重载
来源：http://read.share.vehdjk.com/Article/details/ghwmofrbh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/grrjhwvcy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fktsv.cn/Article/details/ghqjrxvjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gswpyqkcy.sHtML


<!-- 参考信息 -->