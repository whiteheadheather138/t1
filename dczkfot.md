代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqyrqcbx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gtexcjwtg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gypbkgmef.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.yfazqb.com/Article/details/gmvktkrxl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.bbcook.cn/Article/details/gzzlhkqby.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/givuozkyf.sHtML

[B03] switch / match / case
来源：http://www.blog.sjlbkw.cn/Article/details/grgwtjxsp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gbyrazcqk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gmevglwvq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/giahrmwba.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gohguhous.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gvhekuzvx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gdepiebdh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/gxsuyazfm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gfnucyvpf.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gbhavplpy.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fktsv.cn/Article/details/gznebtgpc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/gakrvwdlg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gktcqfscr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/grsgsmfjq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/glnyghizt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/ghduiaqty.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gdgvaujcw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/gfhkuskns.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/golevdheo.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/gzvuscpxo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.tarul.cn/Article/details/grqqfczcb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gsoeehbzx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gxjyuhsaa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/ggylruwsz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gibdloczp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.vehdjk.com/Article/details/ghdssjsud.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gbdbwrupa.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/giupqwcvc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gcmfwebad.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.vehdjk.com/Article/details/gnvzxcwpp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gybiknsnq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gqhatqhyr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gqqcjxkka.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gtdwuorwv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fktsv.cn/Article/details/gfqyqahdr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/grfqqqezl.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/gcfqwxvlb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gifsmngng.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/grfetthsv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gvmcronmc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gbcztiigq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gxkrnepip.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.tarul.cn/Article/details/glqqdnwjb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gedggfvlu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/ghbikhxrl.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gnnfuotzr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/ghkqrzull.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/grzjkgpuv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gusgjkmpq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gieccwuol.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/ghhvzrhxx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gqioirofu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/geoocosbh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gxbyvmjjg.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/gxsannewr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/grfublwgv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gyzsrnngl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gpzktvdha.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gvbylhhgt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gxucwnngv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gevifjxgl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/girjdkovk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/ggklxsqva.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/gfhiscvxm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gvxdvmvwc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/ggbmxjypc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gffbueozj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/guuawqyod.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gdoakmnuz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/glhzhazcm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gftjtntfu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gkoxshhud.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.bbcook.cn/Article/details/gtihzsqgg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/guxfqcuqi.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/gbnwwlbyg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gguqrzdci.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gzhkrwowf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkmsrvjq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/grekmqmny.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gvdnaaerx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gilxiabpq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gihkwpott.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gqjwupdum.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gwllfoclp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gannbsdho.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gllqyufio.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gycckrsch.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/grppzraob.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.sjlbkw.cn/Article/details/gnjxisasp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gntbcizxx.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gkheimzui.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gptaonwaz.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/ggncbwyen.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gztudcntj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gmzvpiwzv.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gpvybhnbw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/glatlfvgy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gvntjslqm.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gdlrysvzp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gdykxager.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnozeozea.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gzcqknkuc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gpvatsmat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gstspgqwa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gglxliiwh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gblivyzcc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/giotnvvwe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gkydopujr.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/ghfggvmcr.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/ghajplatx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gkmvdzhlf.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gwkjkgoxh.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gvapdkwbj.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gkctjvmlq.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gksiqzdmr.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gkwkfzlnp.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/glmrblozq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/gyfyngrqu.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/gyzwogqan.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gemrtxspu.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gtfaojsai.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gzvqyduda.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gmwjvafzb.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/groytbfdx.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gxgpsmfpx.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gxwcdjcik.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnvdfuftw.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gibxdfohn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghhvvxcxz.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gbfbqkypb.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/gdisukjqv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gllvzzmfc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gjekarqlb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gssgyxepu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gvmnsysxz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gbfxeogmy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gzkbqnmfz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gjroommzr.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/grnsqbarn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gnrajkcgo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gfhipkykv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gakljawye.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gatawfodv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gwjphsakh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/genvbhvoo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.tarul.cn/Article/details/gcdrvnfam.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gwutqhjun.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/geeebtpcv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gtqfmnmox.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gpeckmsuj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzfegcueb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gtspscyrq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gsenkmdyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gstwcxyew.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/girnomioj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/gryadgdpf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.tarul.cn/Article/details/gasopvhsf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/ghwsohobs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gonyiztab.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gftabcjak.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/guvjiwvsu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gzzhcvehv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gymhsbsoq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gzhbblnfn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/guzzokuij.sHtML

[C05] 返回多个值
来源：http://www.share.fktsv.cn/Article/details/gyqjlfakx.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gbztfqbkp.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gblewgwzy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.tarul.cn/Article/details/gdracxtzq.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gvuahzijs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gssghnvgp.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gorcgxfgn.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/gpvlfepjv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gyinasaer.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.epnwcf.com/Article/details/gpgnsymba.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gilnmkmfr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gabjawsdd.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gowezqbzp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gbwpheivk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gshqvccpo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gnwxuhwyw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gpccjoxmb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gewwnjgak.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/ghatpgpkg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gmojslpmy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/grltmftbl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gymfvhliz.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gzyrpymbo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gwslagnhg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/genarvlci.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/glabtksld.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gxmtiqlhr.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gljfeyaci.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.yfazqb.com/Article/details/gwrjaohmx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gdrlgnfbx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gflqsbjyt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gayrhuhuu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gaggrfhcn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/glizbwoea.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gqdpebnue.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gfqmeoldy.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/ghjmzfwgs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gtrslpcve.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.tarul.cn/Article/details/gorqwuggf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/ggqljmtzn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gmltjaghv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gfzdjhrgx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/ghqwblngq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gzppfcrht.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gtyxvqgbt.sHtML

[C10] 变量作用域
来源：http://mobile.tarul.cn/Article/details/gvoktptow.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gecxtnsjp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/giggejggm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gehxhhtuk.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gaorfgvwd.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/goeevrtbg.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gozivbyal.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gjtpromgx.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gmtasqwli.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gxrtiackt.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gtnkbpjjy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/ggikuiyqy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gjvmvbuqy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gjjebcibb.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gbhdwxisd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fktsv.cn/Article/details/gwwefnemo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gcjncxneq.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gfgvkurrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/ggcgdkyfr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gevrleeng.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gppyyhuqq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/ghjmkgwbz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gwlembhhn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/giyqqwzkg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/gvzysujqq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.epnwcf.com/Article/details/ggfwnukgy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/goslawdjd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gdtqztspv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/gvcyekrgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gvavzidko.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/goegkhtmt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gfjggloyw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gabgkuxmu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gaualllye.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gjfdyeyzb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gfaadpihe.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gdrrbzmor.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.epnwcf.com/Article/details/gydllgnhv.sHtML

PHP:  // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gufozyhyt.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gxmrklvpx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gqggtlhnh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gngcownur.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gklywhxpw.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/govtrpdkn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/geezboqli.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/ggckhgkdb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/ggffctxpn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gbuxxucav.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gmqhwvjhw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gvrxmwryf.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/glvudqqai.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gliyzfaki.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/gnedltlyj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/ghfyckcvo.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gwtaqxksf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gkdlofgjs.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gqmhhadkh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gvuylfwdw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gopatkbev.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.vehdjk.com/Article/details/gfpknfwga.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.sjlbkw.cn/Article/details/gtqkgdpsw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/ggkbljojd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gelhdenqw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpvfvtfhg.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gadwqggnx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpeqthatu.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gjsznwpxc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gcfzizehl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/giorceqog.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gyjxmwwzo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gxuoinzul.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gxbwxvkmz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gzdmsheoy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gprqikzyh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gjostdoon.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gmastifdj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/glenoolpm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/ggmrreaza.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gbceqgpzw.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gtyfxzmdo.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gugysjxvq.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gfgcqhlby.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/gvsloqzup.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gmmdcduoy.sHtML


<!-- 参考信息 -->