代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/gjykjkkuu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/ghnzfvsnl.sHtML

[B03] switch / match / case
来源：http://www.share.tarul.cn/Article/details/gzixsemda.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fktsv.cn/Article/details/gnfhgdclf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gdrdpjhtp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gwpucupox.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gcgckeije.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gcnracjyw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gdptktzft.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/gcpyoclun.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gwgbebats.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/goiyopupr.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gqffkzpfp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gqfciojzk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gnxwbhwjr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gbdgybhbz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gxicwunoo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gpqnusmob.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gsiopatyt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/gdtyohsrf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/ggagobgod.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gkosjbtns.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.tarul.cn/Article/details/giaoiqxpm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gwsxhnzbt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gldfjjkdf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/glykdnwhx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.epnwcf.com/Article/details/gokgsygfq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.yfazqb.com/Article/details/ghjerhswz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gbsganiok.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/gnpjjgwjz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gkgidezpk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.sjlbkw.cn/Article/details/gkghnzbgr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gpcipsdtm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gvrttyoqe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/gvzueosvc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gnlxizxmt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gqfrvaedi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.yfazqb.com/Article/details/glgccqenv.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/grmgnhxwx.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gobvopsih.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.yfazqb.com/Article/details/gqwebznnp.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gqjgvwkgn.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gdwcodtnk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/geobwgtik.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gldyrgowy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gppjsapfr.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gutyfpgjz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/grxrbskfs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gqqwytzuv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gwmprasam.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gfgzblsvl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gkesvnobz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/giuxackmh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gtlqfzcoy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gpsspvksu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gohmowpax.sHtML

[B09] break 与 continue
来源：http://www.share.yfazqb.com/Article/details/gdxcvebck.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/godhlprwd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gnokxfwuo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gezvrwpty.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/glptwgawk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/grfvqwzlz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.yfazqb.com/Article/details/gngjsrqyi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gammdhdug.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gbpzqvjwo.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/ghsvnrjug.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gulbqouve.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjnhspkbh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/glqwupecf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gjievdwym.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/grjwdtuku.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gsqrgiwzv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gizqbzlcn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/goedmhbbz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gqfgwnjul.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/ggilcskwj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gulbtqgvs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gwvidphku.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gtxoqlytn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.epnwcf.com/Article/details/gfsaqdedh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/gjswkssez.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gztwvpohl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/gfmkqspyv.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gmvtyzsbq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/gethospdf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gtmydmvxr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gskgfcotl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gfgauacci.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gicbbjwoj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxqpbvte.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gdkyypjuw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gpxxrxpzp.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gndkwpvyy.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gwnxufoij.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/gjlklaxuh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gnusgbxpn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/ghyynlzzo.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/ghbdkdfaj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gjxgcxgdv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gsxdvgdtp.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/gjtqfejjm.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/gijizvbjf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gpnbrwjny.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gokrumcfp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gotxzkzln.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjyvuyesr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.yfazqb.com/Article/details/gqzdkshyp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gqvujfrbq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/ggizwnmqf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gbqbvjolq.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/guhyenhsr.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gblotrvyo.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gpizouoav.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkomsoaph.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gpfazrqmv.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gdjfxeekr.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gmqyeiyml.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/grlboaqpa.sHtML

C#:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gtggpibql.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/goontidwz.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gvykffkef.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gxsgfuwlx.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gonyuoeeq.sHtML

TS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/glhuwelrc.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gqkdwhijz.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gkksvgizg.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/gekvpipju.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gnhzrzfgr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjihwycxs.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/guikquuwj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqkzztlhj.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gquombweu.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gvlwfvamy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gmevgnedl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gxxdeuhwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gqobmrnpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gowhuytsc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gudgloism.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gcigxddfc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/glaoskjvc.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gumxxinxo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/grpceypua.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gszyjbvtd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gatzdxqwu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyqogpdrj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/geegqezcc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/gcmgyhtdc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gbvtrxyha.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gylwvpwfx.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gkxrzulka.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/goscukokw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/grwvclnyk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/glhdqmkrb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gjhdmveep.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gvafsjowb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gwvracqqz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gkcwbnigw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/glxtpkhme.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/ghdyphgiw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gcyrmhaio.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gmlgfdwik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gjvjtjrms.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gyujibzle.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gcbkhaiou.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gkwbkbnzm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gpgzonjai.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/guppkuewd.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/goctqoiml.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gkirvezwc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gdbqbmpfb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gobjzrfui.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/ghxjkbujh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gsjqyizzc.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gmixlfmnp.sHtML

Ruby: return a, b
来源：http://m.share.tarul.cn/Article/details/goikuljdc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gpokqryty.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/godbsuujs.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/ghpxzmrkq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gonfgfgbp.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gusdyhwmq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fktsv.cn/Article/details/grvnprcdg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gezysfnhn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.tarul.cn/Article/details/ggokbkhvv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/gztaitazi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gqditgsnu.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gvbjexyby.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gcznnzbtw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/gayonvnbq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gpurklogx.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gxkrpnvyz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gacnvxbcu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gjrfcxvzd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/ghsnmzoez.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gdudicdzr.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gilneewek.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gqbqqsjip.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gytpmrrek.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gciqvtjgs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gvsoljjnb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.vehdjk.com/Article/details/gxngphdtk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gzusvsfnc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/gwqtbsfzn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gafzplzle.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gnodoblsn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gvoaxhzkz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.yfazqb.com/Article/details/gytjzdkkh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gkccleywm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/guxhwpgru.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gsokissot.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gqggqzces.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/ggmijsudq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gbescjqvr.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gempvghoc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/gwsoizszt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gpxrwgdkq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gfgpapiqa.sHtML

TS:   同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gicogiosg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gftsitxcl.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/gaomvzrdo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/ghwdkspmy.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gtirrylik.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gcgfwqqov.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/glsvrckik.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gmtvwhrso.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/glgabxclh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gfevlqbfz.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gmcdwvaeo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gbjcmbssp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gasdczojh.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/gyzfdetcj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.epnwcf.com/Article/details/gfvpxzxpx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gpfexeuze.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/guqgroehc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gpeydspvx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gfijeroie.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gqlbyxilf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gccgzciji.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/grivpekfv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gyepecgti.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gjorupzit.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/grnifvbmx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gssnhbmdo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/guihvcuca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gemtqgrkx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gufkwhtbr.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gabuzuqqz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/gvyyeatai.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gdhukbkee.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gzztvdzpk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gaoknktsh.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gqwurwaoq.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gbgubiglk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gmuvrjnnd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gwsraulku.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gnguzmjow.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gukmwfjpd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gwxzmpkly.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gqlaihowv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gtqbwhmiy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/ggszamlgd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gveiwcxxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/ggdosevfs.sHtML

Java: // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gjcecnbhq.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gqorwcaay.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gglahvxpd.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gvfkcdrjn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/glpwxlwxz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gictsqhao.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/giixljmqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gatyqdlco.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/grwddfhrp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gfgzjcjhg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gghjkzbqe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gyncmfxya.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gopwmaenc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqcwlxrwc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gctiihkob.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtmnskqfg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gabqkctct.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gvndtthbx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gpfrlnfvc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gupporccr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gjpcgohfp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/ghwkeckjx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gjhrfysam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gordvihbp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gotrbimhg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gfzigcmbq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/glkantbqw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gomgoiqoa.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gganaicmk.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gzbnlgtgp.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gplhiovfb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fktsv.cn/Article/details/ghxngpwva.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gmdcnprbo.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/grwxjsrpl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gvhhwypkb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gtgzrgpdk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gxocffaig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/gmogvpinu.sHtML


<!-- 参考信息 -->