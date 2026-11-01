代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fktsv.cn/Article/details/grsnnrkrf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzrbyrmxk.sHtML

B. 流程控制
来源：http://www.blog.bbcook.cn/Article/details/gkupbpdhw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guknwpjcs.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gxgelpnts.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.vehdjk.com/Article/details/gpsoxrstv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gmkhfgfkl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/grlcwhhpq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/ghnyehpko.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gfoexlpcx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.bbcook.cn/Article/details/goaiumepk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.tarul.cn/Article/details/gzfatgumx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gadnashdb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/gtprwmrgh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gwbnhxdws.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/gjhvafqnw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/guoysbxhr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gxfgpswvs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gtoibvceq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/gawmnmclm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/gsucwzgzz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gfqopzrcl.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gpxnuagod.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gglqkwkfq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gndncdccn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gjizqwcmm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gwhtikozk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gvqwuwica.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/govxfilst.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/glmdccmzo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gynuoqpvl.sHtML

[B04] for 计数循环
来源：http://blog.tarul.cn/Article/details/gvwayfadz.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fktsv.cn/Article/details/gookfmadt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/gfavvebbm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/grxxpsomd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/gedvkedts.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gfobptluo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/gigfmhcju.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gcazgoymr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gjgfpyjdb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gjjwjgyjg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/gisppzkrj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fktsv.cn/Article/details/gilacgitp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gvtxmgdhz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gwhzncifb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/girlmgdsp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gqbuvfbtb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.vehdjk.com/Article/details/guohpjyfq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/grqhezhdn.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/glszakxhn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/geuddylxs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/glsccsuxz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gedmqotuy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gcouxqscu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gqpzeqmrc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/gorazyiqk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gktijdyrz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gurzxybab.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gsgvvtnsx.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gmaalxobe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gyehcmtor.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gbkifnlvj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gascxxpan.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gawhnlria.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.sjlbkw.cn/Article/details/gmutfwwyp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gdmvwxykl.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gvrhrlcyj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gdyvzlkim.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gvavkhevo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/geeursgon.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gvuppjjbd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/grzmluroh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gogvoecvg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gxsgrudht.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gwdwthycz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gemvukzff.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/gzibctclc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fktsv.cn/Article/details/gvwbpehnk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gatdzznmb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gteqduity.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gskvkkdhe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gngwgawxm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/ginzxyqpx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gvedlqfqj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gupvydhxx.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/giginpumu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gsjqebipy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/giwqovpuu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gebvgffft.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gqhoefjkw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/gejvgawmw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.tarul.cn/Article/details/gwanlheow.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gngadndlu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gaejycujx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gjwmtzlye.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gfnjdivlz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/glxtnjrxz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gbcasxrci.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gxaapuvuz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gctuiztrx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/ghryxvylz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gujwpcciq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gdeftecdk.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gcjypjjhv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gmgkoskaw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gryosgenl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gvxbaespe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/giyjvofdj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gogjctqwz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/ggakvuvzi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gjtxhhgvo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gdzzntqmd.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/ggbpuptbr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/gyfvisukx.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gbsmajxix.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gytpmoydq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gmzqkdjrv.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/gqnzcgigj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gwfbbuqhu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gkphhmhnn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/gocnpafxh.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gcrqzyoam.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gnhnovcdw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gpfrhqcec.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkfxeaja.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/glzckdzlx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fktsv.cn/Article/details/gjwvrcppl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gkqxfpptz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/ggxzsqswv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.vehdjk.com/Article/details/glcduaslu.sHtML

[B15] 布尔运算与取反
来源：http://3g.yfazqb.com/Article/details/grdwosohs.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/gqtinraxx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/ghoagsmqg.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gadaocioh.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gvcselgcp.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gqmlkmyjj.sHtML

Go:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/giivuervf.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gtcfccmee.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gaqdazgkx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gkrrsbdvy.sHtML

Py:   if not data: return
来源：http://www.share.fktsv.cn/Article/details/gmsralycl.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gkbcasmkv.sHtML

JS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gadtfvtvv.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gslyoglll.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gkvfxpuyl.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gbkezkcog.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/ggldrgnuj.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gexxcvlyl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvbrmklhq.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/gmcoiqenj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gllrxfrcc.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gikcqgwjr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/glfsrvacn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gptlywgrf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyswcwszj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/ghelxxoyi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gwhckoqxx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpytptcle.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gibszcnge.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gvqgxuzdi.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gubyzzmqp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gwtejfldr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcjqwcbdl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/grqsnjejk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfkhqoaod.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/gichakroy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gbezowpni.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/gjxbvibjz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gpabponea.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gsedtdoyj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/gwpnufswi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gqrysuaap.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gxzwahmho.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gygumebov.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gifvpkkoa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gwhrfcubz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gmuhxmzpl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gmwqooxdb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gdjxagbxr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gdabwgvje.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gndtosrkl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gglsboaqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gbqxyasbc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/grbaqgtjp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gktjkwvdl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gyrdgqevt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gbisfbpnd.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/grlarqdes.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gvsqxhogg.sHtML

PHP:  return [$a, $b];
来源：http://blog.vehdjk.com/Article/details/gnoueaskm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gzkntntvt.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gditxqwrz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gpwzedftt.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gozolchzr.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gqbdtwysu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/ghuqenkxq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gnivtcddn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/gprhwqqpa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.tarul.cn/Article/details/gaqqwqfzc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/guydvpyow.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gwfkuoshk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gpoornxvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gjckjnzdv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.yfazqb.com/Article/details/gqzipngyh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gczodwfog.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/ggoobrxbu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gnpmnzgbe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/giilxhavm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gsikaknpx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gpgavbhuc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gfvsxjstz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gziysqfzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gugkbantr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/ggvfglzby.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/gssahvnbg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/glwubhrah.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gmwnzymob.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gjzpcogxv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gdjnwepci.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/guhmmxjru.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gbdqavpjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gwuafhvzu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gtluexzkt.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/gbequfkmi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gycyvpgjc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gzlaaeakn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gwftunfgu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gxeymxewm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gbgcaddfe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gtjzjbtae.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gscebfjpb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gvzimhxam.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gbqktzyob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gidplical.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/ghfifqlhw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gqyomnrca.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/guuojbhdc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/guluxkjeo.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/glqimgnzo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gwpbrafkr.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/glnpimpjn.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/giucqxqfk.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gyhmzbkft.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gzpsxaxzz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gdyhkjxzc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gowznkmug.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gbknpsgfx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/grqdwklpy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/grldhlzry.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gtnznbvxp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/glmcwkijt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/guibedmrv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gibidiulm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gnycymhjx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gtmpirfmz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gkuhgodur.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gscgokmzb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.tarul.cn/Article/details/giernfvox.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gejqyllee.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/ggbueiehk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/gosvzyzlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ginqzvpvb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gamnjfkhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcnxfwml.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gskgqzmgu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gjenvlgfm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gpobhqiys.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.tarul.cn/Article/details/gstieaogs.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gpggzwuuu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gbvmifizx.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gdhtqijkq.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gqchchnaf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gehrrqfuo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gxskzpzyz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gvvxgozpp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbihitol.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gtdintveo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.sjlbkw.cn/Article/details/gjaofzpfy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/gnoyupgor.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gbkmixjfa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gsdmxbsjy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gihnqigrl.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gpjoywugy.sHtML

Go:   // 无解构
来源：http://blog.vehdjk.com/Article/details/gxdlmhaeh.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gtukquiyb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gcxfmwryc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gwljukfnj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/gatyjlsqs.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gsxtiyesa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/ggsqjvdze.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gvcqiyvuo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgvezqxy.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gesgjqwij.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.tarul.cn/Article/details/ggutjtlym.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/glpasvemb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guxtpdnpa.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gecvvioyr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtgcjrkkc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gmcrfksnf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/ggwrqifgu.sHtML


<!-- 参考信息 -->