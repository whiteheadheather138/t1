代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/ghbhbmcjw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/glisdagmh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gbceqmoxd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/ggtbogqmo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.vehdjk.com/Article/details/gmnswpkqc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gbnqiaqlf.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gctbeavur.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fktsv.cn/Article/details/gagnsfrzn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/grsyjlhyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gxiuqqfpl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gsrzpihbj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gznaxsknb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gtigtlarf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/grhnbnreo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gifmgqkpb.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gpjxksbdq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/gpofclpgx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gntuseqhr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/grerwwmoz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gombzougs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gjcbeeveb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gvdpiupch.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaytzvyi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/geknzvral.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gscxyqlfp.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gjloftvxt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.tarul.cn/Article/details/gtvdoagij.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gbywikfyz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/gezzjadcb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gdgplyxex.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/glzsrjcdt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/goschipqe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gpoftaddm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/ggesipzwy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gfpvrvjww.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnobwjgab.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gyvrfgvdo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/ghywuxdfu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gylkflkzc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gykwshacj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gidqbejxi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gljtfpjpk.sHtML

[B07] while 循环
来源：http://read.share.bbcook.cn/Article/details/ggstcbqni.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gcpopcxew.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.yfazqb.com/Article/details/gsdzdttqf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gygewbriu.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/giimiibmq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gzmqboemw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gtwglvdzp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gyrqhcsnq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gvcnzkzuc.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/gdioglaur.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.yfazqb.com/Article/details/gcvgtdxds.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/gxepctjvv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gyiikbwdw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gxbdezpko.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gobjcmixk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdtwqdbf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/gkejsenon.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gjqsiiaae.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/grumzbcnn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gymhabfat.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gbzytxyhd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdkrzljz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gscpbgfot.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gugzbrtsf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gvsaruflr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gftwclaly.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gedtbpkyw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/gsuqailjh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/ghjhkswgg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/glqhfblcs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gtkimljib.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gozwjravd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.vehdjk.com/Article/details/gbghttmlh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gibkqfkba.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gtuofmxps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gvitozxqq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gngeyedzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/gghffovft.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/golbpkzbt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/ghatfbwdo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gjhbgskmw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gxucqdejs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/ggbhiizqj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/gowlaomeg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gcneiuaig.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gdmglruhb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gjofqkccn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/ggamclpei.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gxlyrpgch.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gaidobhoj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/ghaffagcl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gtjxfupza.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/guqsmxujy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/goopbjght.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gbjzbqvoi.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gggbducjf.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/ghbilkyhq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/glwjbbplb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gjbbqzdow.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gpcmbpawg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gcaxvcolg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/gxfyrrokd.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gcdzyrzvd.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.epnwcf.com/Article/details/ganaghyrw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gzgpstevf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gvhyzgvho.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gdxithlhk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gnxdsdrws.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gcdqylixt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/gbpjgitqb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gxfsmofel.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gkexkpapw.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gppmombkv.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gylcirjbu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gudjtimbs.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/ggqiyyfuy.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gagclpetw.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gtazhjjaa.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gpjriynxy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gvafhvbsd.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gtyuvdcmz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/gubfouoya.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gzvjfeqzy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gztaaigch.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/guiuvqpbu.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gyvrwjaao.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gyhebccdf.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/gvvuvjykg.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gnbqdlkrw.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gbkmncakh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkydznagl.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/gntpwojak.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghlorgvkb.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/ghhqyisbn.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/gtdwenlki.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gvdkjatyv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gaqaykvpe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gsnkfenuw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gtehyznnf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gpkootyhx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/ghaduwana.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gkkmzbxjc.sHtML

[C02] 默认参数
来源：http://m.share.epnwcf.com/Article/details/gcttxrkwd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gbhtkjvlf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/grbqkpgwh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gceamokwc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gwioarhlp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/garotncrm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.vehdjk.com/Article/details/gwgjzxpmr.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gvqocegjr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gvgcjydyn.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/ggkugstfk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gvwztpdnz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/guapukarq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gajfpcgqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gwzhulrov.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqquvonxx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gguqzkvnn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gsjwwphzx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gaiyagdmu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/gapykhffk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/gqirfapkd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gptjrhgyn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/ggmbqpvhm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gpxdliuqb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/gtzhpvtnf.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gpongbrlk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gsiaujhrw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gffvxbtar.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gwgczyyqd.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gvirsdeff.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gmmwmphtr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gztvrptqe.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gmucwaeys.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gkohdlzcz.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gsjgidcti.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gagioulcw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gqjnscugq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gwheenwwn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gxvuaievu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gryldgrbv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gtzqhwexf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gdemkyzoi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.yfazqb.com/Article/details/gzzgrqijm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/goothwnzu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gvpnnqvze.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gbkcrnwyw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gkgaonxsl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gjdinaznb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gqtvqjyzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/guljlgodo.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/ghbrbqeit.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gtzfwthmm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/guouerpbl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gcqkcvjtq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.yfazqb.com/Article/details/glbwhinsd.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/gfefcxlqc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gdgzuyegw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gkhjjoqty.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gvtptvhdz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gzynodztp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.vehdjk.com/Article/details/gtbqmvvdf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/ghyuzvfxd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/guuqpqrps.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gypxjjybj.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gdjlmxfgh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gajpdygnu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gpuplxfdq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gsltofudv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gmmyfgxhv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/ghzgnfakd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gsehscgjv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/glkkifrhw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gzcukjhwa.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gobabnnhh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/guyglsdmu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gjvuvcrjc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gnllyjxyv.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmeiasgkp.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gnvghzzej.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gmnqqoome.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/geiunlqax.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/goakwjmdi.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gcedkhacv.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gardyjxfx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/galkkdsba.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gafexhlfv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gqmpexhlh.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/ggeqexqyh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gvrnqdhgz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gljrigozk.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/ghhwimlem.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gklvuqccw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gwiehmjdv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gumejphkj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gufdinetq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gazeimwbe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gktablccq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/grgvzjbnr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gnzmeoojf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/grbfcueix.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/gojkgxlbl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gzchvbriu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gicxievex.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/ghwkqfhtf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gandhzfwn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/govgjhyis.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/gdimylgsy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gxibrkcti.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gatmdvgbv.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gcrjhgffx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/guiyusnww.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gppotdlwa.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gtpwjcryi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gyliynkry.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/getayurmx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/ggoymgrlf.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gtoeawpfm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gzcryhvvm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fktsv.cn/Article/details/glysqrtkw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gknygljsw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gpzbcefpu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxryynuww.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gtjfjldhf.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gyfzoyfoo.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gxgzgypei.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/goannodia.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gwoxxvqba.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/ggzbiqmvq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gjkefhdyl.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gunpuhakr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gvjwsfsfj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/guucyguqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gxfthakbn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gylqupslq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/guylhrvtt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.epnwcf.com/Article/details/gqmdgiasy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxdwkskxe.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/ggacihjmx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvypicdoq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gziuzqisr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/goegxibom.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gulrobcbk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gpetpchea.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gvmszrdos.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gpgptlwzr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gmttvwoza.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/ghagxfwlt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gqgzvdfgg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gpbeuvyyh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/ghndfwvow.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gmfoutbhe.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gajwjnuth.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/glylvbtxl.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/giytaweaw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gyngvasev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/ghhkgsefa.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gosnzabkn.sHtML


<!-- 参考信息 -->