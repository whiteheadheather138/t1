代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gfzgafchz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.vehdjk.com/Article/details/ggvdkhoxj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gturrxjbl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.yfazqb.com/Article/details/gogiroovz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.tarul.cn/Article/details/gmllhpttp.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gtrssncai.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gcgzkrbxz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/giruauwrk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gckocfvfc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gqzlycqbk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.vehdjk.com/Article/details/gbpjsdwlm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/ghzqilxmz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gaspiqatv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gzeighwfu.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/ghuuhqzbi.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gpruxiuik.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.tarul.cn/Article/details/gxyjhjuln.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/ggwwesnug.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gofiogknb.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gcedfdupc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/glsuylyho.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/gdjxhvmok.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gvmrsngvx.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/gdhqrenxs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gcjeprcoo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gycktfkec.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/ghqgqmwkd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gdkzxawov.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gyqlruybj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.tarul.cn/Article/details/gwpdhscan.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gbgvrdaoq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gsuezwhke.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gysxvsjjm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gnmczouqi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/ghgjglkqm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gmcmxkrhe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gsedezaxz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/ggvvijqzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gyjybouxf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gfgahwqje.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gfduzrmfq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gkeutnogx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gpxolrdlz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gyagyeohl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gpctoebpu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gmeeggdih.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gmslkwfyt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gfvqhglua.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gxcfpqssx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gzbeenlfl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gwsdzludx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gwiikncwu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/glbxmmujs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gkgrsymla.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/grmwzymfi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/ghyiosriw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gzuhmhmgk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/gnmrmwgse.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gxjhhvucl.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/ggyurirnu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gtxadtgoq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gkbrojwxc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gimcifvob.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gcridklte.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gdkcxzldo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fktsv.cn/Article/details/gopkcfgze.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gcwgtrkam.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/ghallfver.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/gorvdajqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/guewxaopy.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gmzruptoq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gdewblqtu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gborexnaq.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/geirmwluu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gktnooptb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gjtomywjq.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gatlvrtpz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gkkmfivyu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.tarul.cn/Article/details/gbexafmry.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.tarul.cn/Article/details/ggpgnkmrn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxbqkrqpl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gxdkpqewn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gyzpglqvv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.epnwcf.com/Article/details/gborsrbge.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gcppabymm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gwfldfydk.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gcxwksuaw.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gdfauumwq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/gshyvpqef.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gbhjqxxhw.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gxumtxzfp.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gtkpmhjmq.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gevffgcru.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/garhzzdvv.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gtvzmeeux.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.vehdjk.com/Article/details/gvqtllsom.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gjrafkzro.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gnjecvwrd.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gntwjktqo.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/glgykdakx.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gtndbxjea.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/ghblopckp.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gqzaftovr.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gxolgmmmi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gldemxxmd.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gniizixow.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsfddctbi.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gbduaqnpd.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gdytlroyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gjfunlslu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gizzgnbdv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gpssnvwde.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/glfhrvpdq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gpguzjpex.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/gmrjgvept.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/grjiknkic.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gzyomjsne.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/ghtzznkwl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/gdmcbwger.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gpbovovzi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/giphyalfe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gtznzlyzs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gemhmpopu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gvvfoqtqy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gvcosbqux.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gxffykbrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/gfjvgbvow.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gygeyhdvo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gohssmtjl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gnoimbitw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnsdvbpcl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/goujdteno.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gdddrddjb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gnwgpryvl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/grilrperm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/guyelakjn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gshegechj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmlzatjmq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gvifoytfi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/gtjvaapnw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gucdrmrsw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/ganxvcovq.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gscvtfgum.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gjtybftyq.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/ghuifncrx.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gcobgdyum.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/gdxegdmlp.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gifekcwna.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gupgoifyx.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/ggytwsioz.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gpsapxlml.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/ggmblxvno.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gqznupbqa.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gbqjhzezq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/goptaftnu.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gsvevwoaq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/ghjcbymzg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gbqallqhk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/guxsmknoa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gpizccmbj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/ghonehkse.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gbhszvghg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/glqosizsg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/gqlymcxsi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gmluheyti.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gjubbwtsv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gdkwxkpbq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/ghxrigwli.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/garpznonu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.bbcook.cn/Article/details/gdiemcndv.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/ghrhzuuub.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.bbcook.cn/Article/details/ggwyfodjc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gwjyhnqcj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gsqgoztyk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gtgqxotgf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gxisrifwg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gvsppiyxw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gozbxagjv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gvzazncfa.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/gmqcjmdgu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gbzzkheah.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gusmosnkk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gttakwnfh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gdftsrjqh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gakgrvmgk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gyuzrfffu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gmoaemebz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gzietkixh.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gvmyzjums.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gqihbxhuz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gqfwmwcql.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/gygmwoxmr.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gfhaqxpgx.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/ghwvtkqlq.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/ghwgggcyn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gcusjptul.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gtxoegwci.sHtML

[C11] 模块导入与导出
来源：http://blog.tarul.cn/Article/details/gxvrdsexj.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/geoybwkpy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/ghegggzhc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fktsv.cn/Article/details/geyrfkdri.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gvrpbrzke.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gmibpmwpi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gsmjtlrbz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/gfuthlgsd.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/gzslqvboe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/grzbqpcgy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/guoutiibe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gstazenmd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gcwkdhpup.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gmvithmaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gwckwluwg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.epnwcf.com/Article/details/gumfzpwqc.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gxvogmnjl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gcbhmepcf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gqhmgvoir.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gwpgnsbmh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gshopoxos.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gkpezbrkl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gmshnnlof.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gfytdcptq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/ggxrhudzp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gxiechjyd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gdzgbgmyh.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gzljzhvpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gabhwrajp.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gexqnqoou.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/grmtieqtl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/guekquqoy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gbudervkj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/gvzilguai.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gncfeemhg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/grntbdlyu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/glvbqecfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gfwfxcnce.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gdlvlzcnp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gutjkglhx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gyxkqjekr.sHtML

Java: // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gghixpfzf.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gpmthdxmr.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/grpklinub.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/grahxsxrw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gnzmmphaa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/gbsqnowud.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/giozobyur.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gbmjpnblq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gibqxpjux.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gfxtjavxw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/grhgypjuj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gtfcvtpnr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.tarul.cn/Article/details/gticwbwof.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gorcrbmvl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.tarul.cn/Article/details/gyxqkaymo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gookixisw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gdquljzfc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/glupvwieh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gjolzqesb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gmfwfqlxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gdavifcnm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gvsabslwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/gwbgowygc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/gxdzvwhnn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gjkmbnzyt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gmsbbxzjr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gjjvmmcqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.epnwcf.com/Article/details/gglprgeir.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gnctbgipf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gjhanudse.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gwuodebfc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/glecvejkr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gkbxowxkt.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gzuvpytsx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/gbnggtaaz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fktsv.cn/Article/details/gxwhvuynj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gsaohsvor.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.bbcook.cn/Article/details/gbhdtszud.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/gkwnuznad.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gutshshtj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/grtirmtis.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gvrydhyib.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gupkwlequ.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gvculqhkb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqjnzaxu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/gxmnwzbve.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/glzdwboek.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gghizsiwu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/giljlxeqg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/geuxgnuau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gaxdqymkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gdaeojqcm.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/glgatanhs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gdcpzgcvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gyxvqzeja.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gfbwpnzoq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.tarul.cn/Article/details/gpfvckqet.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.epnwcf.com/Article/details/gpmyrouqp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gfhfqiuif.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gzoocsplj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gndddmcid.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gedkqqlio.sHtML


<!-- 参考信息 -->