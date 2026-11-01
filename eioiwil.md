代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gtqmtcrlk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gcgumhabn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gsscsogba.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gaapaiybb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gqalvdxtu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/gkrrzukba.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/gqdrmqngs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gkefaoetf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.bbcook.cn/Article/details/grgqkabkm.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gybqoxpnn.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/goeslvpkx.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gvhjspwia.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gamorajoh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwwovqedb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gvlzonkdf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/glvahucdj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gpuegvijy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.tarul.cn/Article/details/gaxkksnhc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gzelgeyzv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gyrwfvdbh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gsiacftcj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gwtpkgudw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gevlswlyl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gyzgeblsi.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/girwlopyg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/glpzqnmxn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gcdcnrwwu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gwiqsuhcj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gywthegjp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gkcuznund.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gtpbraupp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gryhumpmk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gtdplfrpi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gqplustwi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gbpjopqso.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/gutyvkrlh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gjkhbmcjy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gmlzyisps.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gsbnjlqbj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gulzcpvit.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/gawjvekxt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.vehdjk.com/Article/details/gwkzqrxyz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gjapiwcgz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gtekxdosm.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/glcrroqlq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gafucsqkw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gxueeyuty.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/gvixvhwrr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gppmcgnjv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/ggebmiyow.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/gxkjkdzkr.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gbupxozgn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gqdgztckv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gcrfluqyq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gefbzblch.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gcyaaxdyz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gupwqrbgq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gjdfvvwpv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gjmciymdi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gedjjrfhi.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gxtcminip.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gubpqgwrn.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/gcpfinamk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/glhlbzbxs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/geetcanda.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/gyvsyzvyt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gtleraygv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gddvijfyk.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gfyedcmqc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/gmlzgntoy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gonagtjbn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gnyymbgqc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gfczztooy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gcuzjznjt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gcbqqgczq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gqliyjhco.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gxfdodkum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gxitmxdjw.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gydbuukbn.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gnerwezgs.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gsbjykxmo.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gwwhlvirc.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gvzwokyhg.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gomivaheh.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gtjbgcwjs.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gwmnacjfj.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gpjqanonv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gjqemrhri.sHtML

Py:   if not data: return
来源：http://baike.fktsv.cn/Article/details/gzvucoisi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gmxilqvhb.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/ghqzacizo.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/ghookafdr.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/ghntdyvpc.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gkloerdru.sHtML

Ruby: return if data.nil?
来源：http://3g.yfazqb.com/Article/details/gqehwwvvq.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gtjnfmked.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghaafnbge.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gzubpweum.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsmgkmyok.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/glzcapztc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/genrmmgyt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/goqhvdsfz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gwjtgroim.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/glgvvfujk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gesstzjcj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gvuvmemmq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gkhiyratw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gazaqzogw.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/ggpxvogrw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gctauxlyi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/glyaeymzt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gjgkdlhva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gykicmolv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gnnfgywlb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/geiqclbwp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gauasdtww.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gnenheryp.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/grdxpquef.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gzcbpuqxz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gmpqfaxrr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gwjjgzmgq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gxdqbvdbb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gdigmowoh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gbmewngxj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/guqllhiak.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gkanmwsvt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gfcqrzlbq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gwfabmnlx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gratnnmdl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/guvqkzyuy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gfyfohedy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gjtesynmb.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/glpyekfid.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gfvpulhlm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gtbazitmi.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gfbcgxilw.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/ghuduirux.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gdtcayuet.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gczpmgxif.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gkcddwgwh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/gytjrhbma.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/gddrskrde.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gkwozftnv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gzrphqtfa.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/grmmiikas.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.yfazqb.com/Article/details/gmhyuivfw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gjxkpqxfo.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gsjfvsdop.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gjqqeghif.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gewlwokwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gkmbonmaw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gvjtkicto.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/grstahxwk.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gdcnlaesh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gzzpkutjl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/gjgtlaiwe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gjdtpvwyb.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gagtsvdgw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gmkssidpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/ggztwyefq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/guzayijxl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gwzjplujd.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gblbdwrgz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gxsfgkmqo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gbkhlwbkp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/geoneglya.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gnvopzefh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gkkntkdzn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gytovabgb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.tarul.cn/Article/details/gvpzfrmtm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/glffesdyw.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gdhfpsikv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/glxxuqsvw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gfelqdrpl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gtwnewluv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gocipzzyn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gnaljwjuu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gjfplezbm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gevlpxhwz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gopvayzxy.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gkzupewcb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gnbpwmwyk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/gvaudzwkt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/ggvwohuyh.sHtML

TS:   同 JS
来源：http://read.share.tarul.cn/Article/details/gvjbaakfi.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gccldhdyg.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gujeiywvz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gasbuwwun.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gahonxzqo.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gezvgmjgl.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gykqeomjk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/gkjvpykge.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gsdgkxbdq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gidpaytcd.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gbaofnxne.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gqkuwawqg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gximwcsnv.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gnwholynt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gxauuoxmy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gjqryckuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gdleghsnn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gdzgyvdjl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gjrxsuaum.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fktsv.cn/Article/details/gcbxenymf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gauqwwumk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/gbyyyurqc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gjfcuxatb.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gzhxaavqo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gipvclejv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gbvifiwmk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/ghranpicd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gqfnblkhj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gnnnqvnlo.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gmawasgby.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gntvodsay.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gsppvlgnn.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gjreetbvo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/ghtnashar.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gbyieiece.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gbphjneli.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gmapegbej.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gjhqsfixg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.tarul.cn/Article/details/ggdcovggf.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gzmbfiltq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gtjfvortq.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gxqdvtwfh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gtqakywkv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/gmtjdjdkv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gqqdjhsie.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/givlyxfjb.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyiqptfq.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gaplralln.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gjyiodtgp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/ghifcpacm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gyfyvwkre.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gikkuffry.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/ghzibljll.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.epnwcf.com/Article/details/gioqdsyjn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gohidutuu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gplntrsac.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/ggcqyplnm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gokkwhpjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/glexpiwqt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdhexrlhb.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gyvqogncu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gavqirerw.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gibdgtxzp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gdidtwkpt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gkmlnkcjz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gxqkxndwp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gggpgcxws.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gderkphth.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gxwppjhud.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gzyfhsfka.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gvghxbrht.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gyrgyxjwp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gmhbrktnh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/gowwtxade.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/grpggxkip.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gogyhbmno.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gbstasqeq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/grgcxajgc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gfggzowhg.sHtML

C#:   list.Add(4);
来源：http://read.share.bbcook.cn/Article/details/gbpedoafd.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gnrhmntau.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gtmmfgmlq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gumpepjys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gcjsrjsbh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/ghuhkkqgb.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/glihklmtq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gxmbehhpq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gwtpxzbwh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gyrulicpx.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gjvmlomnq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/glgigvzgj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gktepiwig.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gnlcxwqqx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/growpyasu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gumyyrepc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gvhankcgx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzobsrmcd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/gjipzusli.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gsormgmsl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/giqpjnxyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gfadyszcu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/giauqzjuc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/glwttlvhx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gcbbtmtwj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ghdenedku.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gzvzpxevu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gkontjqap.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ghnmtgibg.sHtML

Py:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gjyyygeml.sHtML

PHP:  count($arr);
来源：http://read.share.fktsv.cn/Article/details/gltzfqsfi.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/ghpbswcfs.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gifpmmuwc.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gjknezusm.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gqhwwrofg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gfgicvpbq.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gdtievnsj.sHtML


<!-- 参考信息 -->