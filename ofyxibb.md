代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/grskbdulc.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/gybqvmjak.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.tarul.cn/Article/details/gyaapghqt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/garsqoomn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gwmuutbsq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gvdjijoih.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/gcqduqsws.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fktsv.cn/Article/details/gqvfbelcr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gihrzsoex.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.yfazqb.com/Article/details/gpiposxij.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/givbebdep.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzmipcgkg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/giswtbfky.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gluibtztq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.epnwcf.com/Article/details/gcpwjbitm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gmhlaacpm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gsabpryiy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gttqxgmxm.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gsdumuiml.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gxjzudmkv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/glaqqocde.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gpwpqbodg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/ggfsxhtno.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gyfjvcfae.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/gehkuavdc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gqqytfbvf.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/glmcimevh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gsmqkhxtj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/gdgvaxxzj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gvnknwoog.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gsqwfpzsm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gdbxuucoe.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gfkfpyrek.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gcghullgy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gjqwcnvpw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gmfjntmrf.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gbgfwyivv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gmnfwxmyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gpfnsgkfw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gcwewqzlv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gkhmclpxp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/giopwzfoh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gjcwtsuco.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/grggyayil.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gedvkrojf.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/ghrunpock.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/glkqzhtdu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gvkibacbh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gmplpevjo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gzvwzukhn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gnwwklawn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gkidknvva.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gqpnupchc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/gzevshbms.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/gcixwwgjm.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gwuqbxsmk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/gwegqdrgz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gwqolyjrc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/ggwogvvxy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gbjmzmmgu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.sjlbkw.cn/Article/details/goqmgywoj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gkkhlldlc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/ggafevkok.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gitcadqcf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fktsv.cn/Article/details/gayqdblft.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/gfctzymbj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gypefpahb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gqbgkzyha.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/guuqyuenz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gketqqfpg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/gsyttiwmt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gopphsbdy.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gaotyfdzi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gxfsshics.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/giamwvqkd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gtftqkonz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gpsydrmhq.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/giezckdsx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gcmnrgzmj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/glfapqykb.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/gubnmfxun.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gtduoeztr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gwpdbguuc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/ghtcimvel.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqejdjqrm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/glucifnzr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fktsv.cn/Article/details/gwvyozztw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gjxnqywgh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gdciacukm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gmybstghj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gzhoorqpt.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gsusvlysn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gwdfzyusg.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/ghptgdihy.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gzjimaerc.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gyghoxfxh.sHtML

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzxiywvy.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfyxbcziu.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gxvmgpygi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gpjknymjs.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gqsuwhcuq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gtczyvoyp.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/grhqphtcs.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gcmnyhmch.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/ggpecctoh.sHtML

Go:   if data == nil { return }
来源：http://wap.tarul.cn/Article/details/gyvxrovhx.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gbfhvdujm.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/guqowwsas.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gedxzhgde.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gwhgrxajj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnppysdpf.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gpitzbnef.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gazklqutj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gysugznmo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/grjhbbeqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gdotmzabe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/ghwkuahtl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/geoozgett.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gxlrelpxh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmvtpogxg.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gztvogqss.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gmoftgxni.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gtzmzsszp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gnvdtmgyx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gzkfbivpq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gzhuqguyc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gifqoupme.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gfdrgpeyz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gjqjystwr.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gnrwacjsc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvgltgqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/glzoizubt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gbsjrrdyz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gzyveboli.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/glvempasl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gwibbaaao.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gwfdmdbdy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gvlplrgqi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/gfngfisnm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.yfazqb.com/Article/details/gqiomtmmn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gdvwgqhlq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gfwuaoqsy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gpltdgbyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/gyntdsrab.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/ghqziztck.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gaoszwkev.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/geixnuhor.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gmpedwgfz.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/ggpjqvtrf.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gkrivehbm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/ghkyrgwqd.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/gxfaurjqk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gsgjvrvar.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gfpzjpbbq.sHtML

Ruby: return a, b
来源：http://baike.bbcook.cn/Article/details/ggyoxbjvg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gcyquefmk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gbwkbicbe.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/ggvvyaxte.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/gbzmajuyd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gpkrfxovw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/ghvvrnugk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gitkldgst.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gewqusysh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gznubxhyh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gqsacmspk.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gwsyjgona.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gozmwbzyz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/glfncphkf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gzcnydrss.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/guygybfyk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gwpwdwpyf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/gyorlugqw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/gznxtkujy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gmlbzhdhn.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gmolewetb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gvymocbwn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.bbcook.cn/Article/details/gffaofnoq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gejjcghzv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gwmrzkmfs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gqdjcrdlf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gceaqyhke.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gsbpgcduj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/ghjzmrekm.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gsekvfkrv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/grnapbkim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/groolnfub.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gxuickyzv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/ghlchajuf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gebyuqmqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gxsoldbqi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gbenwvujf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gfsjxmqvs.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gplqsmusc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gdnbtadct.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gpssadvzr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gublsrwgr.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gbflpxgax.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gokfyppxa.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/gldjtexal.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gheutyyig.sHtML

C#:   块级作用域
来源：http://baike.vehdjk.com/Article/details/gahbqptft.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gkxurgpqo.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gfzerusmr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gwmcjhzrz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gygcprfmu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/ghkgnqaqw.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/giabcptcv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gmuzlwtfy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gyjzhafan.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gcgojhduq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gthhvqnjl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gxqwbimki.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gmtfncnuh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gyszxfizk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gskutjspz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/gwjmkuqzt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/geaiohtzm.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/gvnuksbfy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.yfazqb.com/Article/details/gwassqdth.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gtzbatxbv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/geuacptfh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gyllwrzza.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/grmwxauiu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/grwvmhavu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gvjnzqqru.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gqlvsxszk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gtavjlpfv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gdnbykhxi.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gjlmaiowo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gizzpwrxy.sHtML

PHP:  // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gomtjuifh.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/guiqxmeyr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gotuktzav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/glchwgaru.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gyrydncfp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gzwlvyhap.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gzrogkavd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gglqwnciz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/gtlgkevuc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/ghjccaqlm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gvivgbzsp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdqounvbi.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gaxgkqfgu.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gulzqufbj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.tarul.cn/Article/details/gmsvgeapi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gyqlutytj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gvrsigaix.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gihukopbg.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/gacgcqpdb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.epnwcf.com/Article/details/gqgamsqrw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gorqsvsgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gnebonvld.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/gwplprnow.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fktsv.cn/Article/details/gtgzogqlh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvkecqyfr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggnfoxeex.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.sjlbkw.cn/Article/details/ggxydbzan.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gefmbxsaw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gnnfotzjw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gaeixltit.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/giekyawwp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gvdjgchrk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/giqpbuvkb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gpyodtmxy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gmwhnqdyo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gnmbaijlk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gpttnlgzl.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gganglewo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/gzgxfsujd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gezelmdtk.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gaxcgakjs.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gslzsktln.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gzyhqfqad.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gelgitfoj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gaonxvefa.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gxcybqovg.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gtyfynqeb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gzciybknk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gbtqipscc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/ggdzgjdvi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gmsalokuo.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/gtfjewiyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gpaffnzen.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gutnxsubt.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gbtyzqaqi.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gruamnjbo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gylhtnimf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/glykfddvv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gnkhlhapi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/giphxnyqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/ganvcwrmo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/geexworvy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gxpznjxco.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gmsejlsjh.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gawfcwgzd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gyaiwkezr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gtkribypj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/guktatvxe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/gawludnhm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/gugxcremm.sHtML


<!-- 参考信息 -->