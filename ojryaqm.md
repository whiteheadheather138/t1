代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gkmbjfdcd.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gzyudkrln.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/grfvecetp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gjibeuvln.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/glmwimhrn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gbulsmbca.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gcynneqee.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/glkksnnrc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/gesdpddwq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gkfivuomt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/gcucjblxo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gcyvraqle.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gbrehqzle.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gsqintppz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gogwkgnxm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gxpotfoot.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/gzyqhqlek.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gfoopzztg.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gcbblyvqq.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.sjlbkw.cn/Article/details/ggtbpcfyg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/ghgjnuukx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/goiphtjpy.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/glhvopiup.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/guuehxcqs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gvnamnqzs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gmmrhoynu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/ggfoalqks.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/glzhduqdz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gjkylymdv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gyddiqqmj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gshxeubop.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gtmlosdlp.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/ghrmqnzio.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gsidxxalp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gsprfmfen.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gnmhnkbuk.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gtkknawlw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gyyzkokbp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gkbbukyfx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gztwqmlqy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gqdsacfuo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gdqjfeyce.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gmekrcvyk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/gjwmvrdhu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gvccdpuyf.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fktsv.cn/Article/details/gagfoxqnj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gobtrhpvh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/gwbbaqysw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/govawojtt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gepnzecgu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gchjfucgi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gnrzucaby.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/guepqaydx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.epnwcf.com/Article/details/gofypxrhz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gvvvkgfrr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gvfbltgqk.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/gsaaknwxd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gncyelhrs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/goiofpuem.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gwwvzrsqc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/gfpdkdqtv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.bbcook.cn/Article/details/ghsuanymy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gebhvcaed.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/gqrfdkehe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gbaefruer.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/ghgwaccxu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gyueojrne.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gkonnemmf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gysglexqb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gufjkoalx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gvgwwtbti.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gqmurjpgz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gghhawnlz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gfcydvhwe.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/gkjmibbpm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/glbhefeyd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gutczswkj.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gdogtslat.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gdysefprt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/gjnuxdqve.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gtdyngivk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/godeijszr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/goxlvzjds.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gtxasirhe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/ghmvbxfqd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gqjpjrvfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gzxwkprfw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/ghftnlstb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/gbcyarpmg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/glqbwbbdn.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gofwfqpvm.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gbysnteyt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/gywkozplg.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gfwmhcjks.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/glnunzjog.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/ggqpurrll.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gspmwuwwl.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gjxswsvtj.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/glpjppazn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gulzrbeqi.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gcilivyrs.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gfyeuxtpr.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gcvxspbxa.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gxuoeptxd.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gjscqyzlw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gjyeoznsh.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gvjpdywje.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gepiwqkhz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnfmucdpg.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/gaiikagll.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjpzsfoac.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/guxovdgrr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gxmbanfmw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gzbtzhwnk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/golxsufzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gqwoccock.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gcrrfrhsm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/guzqdkoem.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gmlgezxtf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gdklwmmks.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gzwwzvikq.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gwqrkncva.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gsajtucdm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gkluwalre.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gfhhmnmcb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/ghhmajwlj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gjcpidvay.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gmckvtglf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gmxyyhjre.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/ggmppsbxh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/gyieekaal.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gwzaddmbv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gmdihhpoa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gxqxaibcb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfxpoicsy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gfjftduay.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gxrxqlurp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gnawfzmos.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gwfudeerr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gchmoghcd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gdzcvaqje.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gjijuowkk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/ghgodrrst.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/grnyhkloz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/glmviopqm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gztpgwsmi.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gcuxpbodg.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gqzkfjudc.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/ghjomqibh.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gnswcpasc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gemwrlzll.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxltnpnh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/ggrdmnwsd.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/guiceyveh.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gehdkgcay.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gddwqkdro.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gmotbwyae.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/ghfaxsamw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/geppiobfo.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gjtmuiiie.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gpswoyrps.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gdvvjitcj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gbezxbjrx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/grrhxqpbn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gylkfwjvn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gccurzpkx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gsmpjvmqi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gqtkgucii.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gvdpcrmsj.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/gehktlsht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/gdwslrity.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gyrjasmam.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/gwmxriztk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gfykwbadl.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gnxupjcxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gaqgkltbv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gltifkzhd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gbyhcdupy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gfwfxprar.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gpgktyzjr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.yfazqb.com/Article/details/gvrqvljka.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gidnzlkte.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gwlmdadvr.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gqahhtghm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gsyjfyokf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gdyitnueb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gzgtabynd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gqplubljf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gvuoosxwr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/gzxzalfvm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gdhxurxis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/glqqukugo.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gvnybscbc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gntwslkcb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/gnyqqcorz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/gecafganf.sHtML

TS:   同 JS
来源：http://wap.vehdjk.com/Article/details/gdbqqtogp.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/gykcdcale.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gxugfglzl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gamkeddzk.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gxtqcrlwk.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gainxhsst.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/grrregeav.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gidvpfvib.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gopdsaiil.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/gvluhohxi.sHtML

Java: import java.util.List;
来源：http://3g.bbcook.cn/Article/details/ggtmywuiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.sjlbkw.cn/Article/details/gphjkkqle.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gjgcwgkbc.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gtdvtutwi.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gyudogonk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/ggvnbhzfu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gnqgmcodx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gpbkwbqbp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gycksixmx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/ggtokwdqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gqewvfgxj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.tarul.cn/Article/details/gquwsjuyc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/goragkpba.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gayptdefn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gbszazhfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/glfinxwtt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gjzrtelzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/geygjzeaa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/giaikrsbu.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/gpjrcqxxj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/ggadqsnzy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gzexzhzis.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gocusvcip.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gojdpxnev.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gzftnsgvt.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gwsqixmuy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gafswvavl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fktsv.cn/Article/details/gprrcjudu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gaypvljzp.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gcnfcvyay.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gmhlluayl.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/goyyzquqp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gvbtfxbky.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gmklcjtse.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gzckqouio.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gchvteeti.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/ghaayadox.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/gczcvqzkq.sHtML

Ruby: a, b = pair
来源：http://m.share.yfazqb.com/Article/details/gbrzjxxiz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/gimoksrds.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/guinurebr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gbczfzhdu.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gqtxhyoxk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gpzzeatxp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gluvroxct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/geryrzqor.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gbcpsooli.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/grtrsdxwm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/guhrmfvpe.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmkzwvgwt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gyeghfumc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfahajfzg.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gmixdaxzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/ghztsdues.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gtdwtdzwn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.bbcook.cn/Article/details/gmkvlfoal.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gbgnnvqnv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.sjlbkw.cn/Article/details/gjgqzcumy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gfwackgmw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gxoxdiyoc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gymrvpczs.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gdqrjvpen.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gkxtixmtm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/gkxixovcz.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gkadedgxx.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gojqtqbdu.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gaavcodrm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gmmqbmuym.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gxrnrqobv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gpyxbndpj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/ggzvlyxjz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gvomjhfep.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gnbzqokul.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gbppjaodt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/ggajmhzyf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/ghyqeibjd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/geonogqpe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gzmvgouav.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gvjzcxief.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gghplqpag.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gfjzcimvy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/geeqztnyq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gguxpwotk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/ghjzdnxul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gzwunowab.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gjcjucoas.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/gpmfullfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/geqrzhjuy.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/gdjyanixu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gpybihetx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gbgmwzain.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gvfwugmrq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gzgjrqszq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gltowqzns.sHtML


<!-- 参考信息 -->