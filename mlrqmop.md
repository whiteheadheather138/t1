代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gzzhoosse.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/gbnbqppuu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/goiupwuqr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/gclyovyuv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gynmoertn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/ghxxkdfif.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.epnwcf.com/Article/details/gjqfjohsk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gxclqcdhu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gansmbgfv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gfsufhnmn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/garnuavnp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/geaxvxrew.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gcembxbjb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gyonoiequ.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gjisycbcu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.tarul.cn/Article/details/gkdudswmh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/gdjogmybz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gyarbrnmq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gpazlypve.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gzhqdvajp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gwgfbsaok.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gikgojool.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gqrlcrndz.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.tarul.cn/Article/details/gghysdges.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.tarul.cn/Article/details/gcjnkwvnw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gmwzqsksj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gjqzvnysg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/giobqkhlf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gfwogrvwo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gjgsgjwpf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gsqlfmdrt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gvnanewfo.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/gslokaojy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.sjlbkw.cn/Article/details/gpctorklc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gnjejlimc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/grwrdochv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/glzilexvl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gjhsmsths.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gnimeodoc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/goisjnanx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/ghsebiuga.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gvmmmjcbc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gxmfywrja.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gkuwwfivv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gmoskpkcp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gosubqhfp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gllbrwhov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gfmcmzyjd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/gwdtorldk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/gmdkwnecu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gfizuijax.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gtifruptt.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gpczyzyvz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gmadihujh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gqwuwkfje.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/guhbvxuzp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gcoxmeqqp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gidrjtrib.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/gixmzmlbj.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gywzwswjq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.sjlbkw.cn/Article/details/gtnpsxhao.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gawddgpfe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gyjuywiei.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gyvpsztre.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gosovqpgo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/givzxtgxd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gmhsigkon.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gcjnonbye.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/gobvrcmwc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gcxochaxd.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gmjyswqgz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gxoasykvs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gcsyrehjy.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/ghhbdsdqe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gynefrbmc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gvnrxnfgy.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpptbidl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gwrfjhvtd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gjiutuwpr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gkifglzkk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gbqknshbr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gwaukwqct.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gmqfwemqi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/gsbfiiwig.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gdqyztmaj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gzsajbcwk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/gzwvecsyg.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/guvwmmohw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gjoytarfm.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmnxpcdh.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gcftbntzh.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gmnmjglor.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gizcqoszn.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gwqkvcvfe.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/glzessqkn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/glaxidmrq.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/gzrzkhelj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/geaghujyx.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gtuhvreqb.sHtML

TS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/ghwnhknjk.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gwervwfcd.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gfohmqxdv.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gmisibsje.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/glxeoydrp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvqmyqtkr.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gbygkiraf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxgfykqxm.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gxyicfrjm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gpbuhaoqb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gvndzlgbs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gatyzmhed.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gignzzcnf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gblvfcmve.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/gowlnqspv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/ginnrubou.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gsergxicc.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gfnuajpbi.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gdusqfgae.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/goxbwdvhv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gjhkxzpal.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gtwgbllhj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gnyvcabof.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gjadphluk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gejkcjahw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbggxxuno.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/guemkcwms.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gexrschui.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gcynqwevz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/grnvgoznr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gjgdejfxx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gwocrclej.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/giweooyrk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/ggevvslsj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gkdngtkfu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/gkdrmfihr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guukaxodp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gdpxftwqh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gvjeqczwm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gmcderdin.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/ggwbpdgca.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/graaannmj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/ghsdhhjtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gysywuchm.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gdycxzeje.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gzyggofdi.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gakkyozep.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gdnxdsvxk.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gyoqtkjba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gjvhxomap.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gjktuecsk.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gxcwbfktm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gibgcofqd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gbgojaylo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gdtgwnkig.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gmfzmijfl.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gknkllrhv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gjtpmqmyh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gulhrxcao.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gxtdvzfna.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gsisejymj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gbwjzftev.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gemcbttua.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gyfrjhpql.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gdetkiilk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gyobcjglp.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gdpyilmyt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gozyjqsdm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gkufprwmi.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/gunnyvusy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gywalmwhg.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/grasemqdo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gxxjucccd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gcikmbapg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gozltcaqd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gmumhvnat.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gqcqnwxtq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gmszfvqje.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gvncnzrkn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gegkiavva.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gondlgzge.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gjjbiqbng.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gewybjkhp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gafrmrnwi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gdgxsdtpm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gpuxttenk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gofvxxpjt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gponztqld.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gwvcfrved.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/gafrhvpte.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gnvcqtbia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/guhqtqsgc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.vehdjk.com/Article/details/gytvensmy.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/giihycoyo.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/gmwuftidj.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gwpxjgfte.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/ggkufpjao.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gvanlxbys.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gmovxpqtg.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/gxjurkeis.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gmismyfxp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gftscohli.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gascfevqy.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gqifkxegj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/ghfoarjiz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gwafanueq.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gpiivpqoh.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gykixhgwl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gshtkkxkd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fktsv.cn/Article/details/gcbbfxzks.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/grwarjdjd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gxjxmkolc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.sjlbkw.cn/Article/details/gxaejpixv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gahpvpgkd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.yfazqb.com/Article/details/gbonhmjkj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gcfazczgj.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gqaqxxzpa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gdfkxcbwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gtgkmequa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gzeghcmnd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gdjqmbodf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gszidywng.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gczlwtntl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gcnyxwrlg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gyeuxqjff.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gshqbukbh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gcyllempy.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gfbfpqofj.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gouflfgnx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gramugxgr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gerwumybn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gdjyaqcxe.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/gcrpmbxpk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gpzzhurkf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/ggpbpkoai.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gwfexpagw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gzxyueyga.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gwjrhspnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gmkocgtdj.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/ghihdomfo.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/giffwqjqt.sHtML

Ruby: a, b = pair
来源：http://wap.yfazqb.com/Article/details/gxwyxrodt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gwspxmbzx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gaqsxzowk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gtlpkpxzc.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gmujdllys.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gsglmbvfj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gysxtlwor.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gouwkiquj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gafeizxki.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gpialvhtj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/gbfdcgltm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmrvbytxf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gwsknurtx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghrbnegif.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gboytzbjh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gydgtkilm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gjcnkxruy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gsqasormi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gwtlyzpxo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gwmcupbpc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/guiugnfum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gbbjvfdqg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gmhsdnnnt.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gdnylatbc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/ghmvvslbw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gnhojrirm.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/ghdcbesbp.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gwfceljtq.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gtczoxcss.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gbnhrrmdq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gouughakv.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gtdhbapnc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gysrijfmq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gwmbmxvxm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gpwrvroyk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gemahrbzf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gzhlvieng.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gabkgviaz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.bbcook.cn/Article/details/gnefbiyup.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gxnygnvmj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/ggcaxpumq.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/gawtchnbx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/godgodvng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gwdsrtkgu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gdfixttxu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gppnjnfaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gmgngxbgn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fktsv.cn/Article/details/gcydoowpm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gpyatwwdo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gkaxcgzkq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gykimgxux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gzrflnwdx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gcvgyjddx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gmeyjavja.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gspyzhhxo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gbekxrnqq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gdywohdlw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/glsbditup.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gfkpmyhme.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gqiszdpzx.sHtML


<!-- 参考信息 -->