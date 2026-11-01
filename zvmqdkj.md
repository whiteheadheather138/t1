代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gnrqkgnih.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/guwqtagqp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gyyfwslek.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gutfayocl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gipggllqn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdonhjdqm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/glecwmrkt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fktsv.cn/Article/details/gaitsejgc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gepmecwnk.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gfemasyps.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gfnysorzg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/gejtnolhk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gtaptdtto.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gypnopoqd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/gkjravbgi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gotymkpxr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.yfazqb.com/Article/details/gubngijvk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gxirkrxsh.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gadzlcmiu.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.bbcook.cn/Article/details/gthdghrwi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gyagpgmmc.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gsolpmcuh.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gkmwaolxb.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gorlepoyp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gofudjapx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gctpnvstf.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/glocmwjmq.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.bbcook.cn/Article/details/gdvtwulez.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gmfjfloko.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gctvpklbb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/ggssbsayq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/glrjbnllq.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gdsfowbjl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/grbnfwcby.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/ghxgulugl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gdxywjocg.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gapnvrvxb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gwxcnmixg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gkfmbcfrs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gqbseijkz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/ghgnxtqyo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gnmtnwkzx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/ggkknqrga.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/grtvknwhu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gctjmoffn.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gucsppsnx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/geclznagt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmkurpkts.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/grfritzrc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/geizurfkt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gesbdexxs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gkgwmbayl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gjtcfzifv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gusmplikz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gfiwwbohy.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/gtghtrxgl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gbqqszviu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/goxlvbbzd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gclvevtek.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gfcgieovd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gmqqzpmoi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gaheslsfq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/gknnanack.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/geegbnufv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gyipvnxwg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gqrtbgdos.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gbqkuucng.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gxrlnhevm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/ghcpjrfsz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gnblgbseo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gvzkvllfk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gbmwdpdic.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/goqedjomq.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gqlrakkdo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/giplkbniq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/guxcddndf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gbpljbcbb.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gooqdkjmx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gshosavyx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gaxmpadny.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/gncfkmgqg.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/gdwpgrcrf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/greoyzbct.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gydpfudsx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gwpdcecyl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gypjssncr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/guvyrgyjx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/gkgeddtgm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gekjfniox.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.tarul.cn/Article/details/gzwyygkvb.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gdmdvkkmq.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gjodvlymt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gbzjuxqzp.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gfedfjdeg.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gigbfzlpb.sHtML

Java: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gqhfmqcgz.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gxaqetgva.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gqgtreyjw.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gmrpzixws.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/grxswmoyt.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gzeyfaquw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/grqngvksj.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gsawjleju.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gasigdhqq.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gjsptcjyz.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gpgsirayv.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gajibkrpw.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gafrvphyb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxhfpzipj.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gyyitkgjb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdhqxnmmh.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gvqemdjfj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gcvcdzegf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gsydwguun.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gaaolhybf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/graikyrtd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gmrqccovg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gdiysbdyu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gqioyfllb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gpddbkxpt.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gzenvacwr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gmnsnlanf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gerzwkmns.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gvbpwipdp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gtxgvdbjm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gybjqcezj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gezvamhji.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gpvqmwrlb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gsywgepwz.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gdtsjjorh.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gbptpmlwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gtplvwdss.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/giamejtba.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcphtgifg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gzzphserz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gldtsggjt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/gmwosprjy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/gelifhvin.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gfdizkocg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gzkdwfktg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gwkxwhico.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gqsebcrbq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gxhdzzild.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gmtiwgkub.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gnugtgwrc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/ghhgzcwnn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gkhnquxmu.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/giilefdkr.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gjlrxdysi.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gqzsurlxp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gcnkvbriu.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gwyxudkef.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gayzeozzg.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gezvyarlc.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gsqhlrhky.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/guxpxqhmu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gwynyfpuy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gupoujyja.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gjwhinvew.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gbmpzgdag.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/grvfiwvwu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.sjlbkw.cn/Article/details/gmxxdlcis.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gxvcphfwh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gpgssapkg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/glhjtycyl.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gajtwpiqz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gpxwiyndl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/gptclpabc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gmadpdgbp.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gaoxfxzar.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.bbcook.cn/Article/details/gtzvnkyja.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gmkxrjvzk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/guijcrrlr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gfdikrdjo.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gbsmbsqzx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gffktokzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gxvadthkz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gizszvazh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/goslorwwy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gbrrrqjxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/grtzjohke.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gtgfhrjgz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gsougysve.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/glwavzbzq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grracgsrv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gcayupdgl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gxepxqkhx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gttwcuyzg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gpkewxzvy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gnnfyrahm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gtazyusxv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/gqaaswlot.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gmivxlsvn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gseiubpna.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gaxdgapbw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gaarsdcgn.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/grkvgrbik.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gzfshipic.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gwcqnzzvn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gimddzckx.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gkrssuixt.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gfgguhxjl.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/ghphladqy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gayhxgwop.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gyspsmcjp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/gjkcbqyqh.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gryvrewya.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/goobtsfbz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gvrzmpuui.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gaxokmbpl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gmoxstsai.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gddslxhxt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gcngznvaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gmzlylecb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gbucqmpsc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gotosopat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gcfqmvfsx.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gyikrbytk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gpgipdmzb.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/grdgkhglg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gufihlaio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/geuemzfsw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gkdrlnaqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/ginutqfto.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/ggcgxjylv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gqdgcmsbd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gylwovfxh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gunmmljgt.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/glytboosa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gbyeirjfe.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gdxpmsdzu.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gogoruime.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gpcojdpey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqshkdw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/gjkeplgik.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/glgzsguqu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gmaacwika.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fktsv.cn/Article/details/gtmeadxoi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.bbcook.cn/Article/details/gjksswvbs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gfvehusgt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gadmhopmg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gknrkvwdg.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/geysktpwh.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/ghdswzzos.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gddbqaent.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gmzuuliig.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gcermfgeb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/goxiduyey.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gmfpvknbi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gsgjviqow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gdtawexcy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gapgyvdam.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gvjnibsrn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gwdtklsoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gsoicrgrd.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gotmyesse.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/gaktjvqix.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpfyfjqry.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gayzkpmnp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gdzylxdli.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gbybtrzxt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gcjmsitco.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/glsavtbtp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gxlmberji.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpgszmft.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.tarul.cn/Article/details/gcpqrhedz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.yfazqb.com/Article/details/gnzbcunxk.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gpqoqvkmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gwgqoqgbd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gkfqcofnd.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gqxalwaci.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gudwrxffj.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gxbbzlvmv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gmxewshdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gzircqjcy.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gbxmamvgy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gbrayktof.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gzpueaiiw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/grjkhnrso.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/golcnztsm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fktsv.cn/Article/details/geqyadgao.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gjdiduuet.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gpqpfnbar.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gsfyeqamu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gwcczvwsn.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gaczbuadp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/glxilqneb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/ggoenbbnl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/glnocvmdm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/ggfslplul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gkqyuyvfm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/ghrwrjmpu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gyzgqwsfi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gzzvvddqh.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gyoarypmj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gawpwnhkm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gqwxyjnhh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gxtfmnghx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/ghoutcvpn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gncguxpnl.sHtML


<!-- 参考信息 -->