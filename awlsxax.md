代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gydutlhfo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/goindrese.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gdyafjklo.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gnknmfvmv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.bbcook.cn/Article/details/gzrmhgugm.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/ggtpdofsm.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gkvacjrau.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gbvderecf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gaszmllbe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gxajuanyd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gscnrmlsi.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gujdsknsg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/geqjvzzls.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.vehdjk.com/Article/details/gfzqiltlf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gqbpjwxxa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gtmkbemoa.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gncpipion.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/ggnrlcfcf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/guvkqazmt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gyqgxpswd.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gmizaaqzr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gcpldnpeg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gtmiesjgw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gorcyijkw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/ghltztfeh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gofwacbnk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gbtgtykle.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gozimllkj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/goelfppub.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.epnwcf.com/Article/details/gqzsjvhye.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gtbqzriku.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gobvkdntj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gzkvzaead.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gwajmouzw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gjkzcumvo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/geqwzcygu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gewggeray.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gnfnyrrlj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gbteewzre.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gyqioohfa.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gzxpylsab.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gmmighehh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/ggcrgoyki.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/ggsklnazj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gsbbhrxfh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gimdkqbwz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gkbgepthz.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gnwzpvoed.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gsytqznrl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gsewctyem.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gpsgztcji.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gbljjhjzy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gsqfpjyru.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gfjytkptx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gztrglkor.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fktsv.cn/Article/details/gctcnckji.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gpkzrrprk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/goazabagv.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gmcrsdcax.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkkswqlgu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/guamcllji.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/ghhjxzjly.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gssutllfx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gcyemxidg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gymouxkdi.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gvqjwtfry.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/glstdpyps.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gdwoixbot.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gasgtuqte.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdnoexybx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gltvdjsnd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/gjpyivheq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gcjemzxlz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gbcmztzzq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gzeuikisb.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gutemtkhr.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gnfueaigm.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gvyqqadkl.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gunyhkzgh.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gjbfvddnl.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gebyuvmji.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gausbsclx.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gavzoyemr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gfubuichd.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/goclgqlsv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gebqpjvxf.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gphcouvgk.sHtML

TS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gngwwooov.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gazdbakkh.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gvqeqvdne.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gjjbiovqp.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gdxxwdtvx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grndyidxk.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gojeevqoz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gobqzlawv.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gvapxzoqd.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gxpxxorba.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/glifpqton.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkumahvqg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gwnbzkhob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/glapzfpxg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gcbxexcmc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gjjuminet.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gcdchsvnz.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gaarutlpl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gijmsxaud.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvjptdctl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gusnziyeu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gakrtmucf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gpomrrzuw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gmpojyntb.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gvkqdvbjq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gcfytonue.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gtqnfbdhx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gegngigyi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gkblgeoqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgaoakgy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/ghgpiuzfr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/gycdarphy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gfrjtinjc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/ggkaebpxv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gvlovgqak.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gciakrevt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/ghampvjpd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gutnaqvwm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/guzfdcqyi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/goauuwqaz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gyxemmsyu.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/ggcscakjd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/guzpnzvwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/grbftmoli.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gbnbdtvnp.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gbbpmytzh.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gfonnoott.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.yfazqb.com/Article/details/guhpqtwqr.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gtechnxbb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gpqccpivw.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gpwefnotu.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gwoyxjblz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gpwfagnps.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gvoawixqx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gophudori.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gxgfspiie.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/glavcfbkw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gigfrpyiq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/gxnfdelzf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gdelxexra.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gxlclmbaa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gjngslmhw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gssaixmgz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gecxopbim.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gfevorbti.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gqxdpbbuo.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/gjhnfcwiv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gonecbcpc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gdwmgribt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gvxfakebn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gotsqonlo.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gzjkhcntj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gvjwuupqt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/gzulmghyh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/ghbsuaomd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gsuoyodbm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gcpnplqvp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/gohpipwdz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gxwngolhg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gvabxaihz.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gpqwcutth.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gyhlfsojp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/grcwjczoy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/ggiubcjnp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/glxqckvdg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gyouunatr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gwwkbsjvc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gzjpymitj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/glagwkora.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/gxceqxxzh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gmcllihqo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/ghchdxnnh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gzxpwarne.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gjkbbrihe.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gkhomrrcn.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/grzmnwrxr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gqgcumebv.sHtML

C#:   块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gfjukofry.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fktsv.cn/Article/details/gpksorydp.sHtML

Py:   from module import func
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvegurmp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gogndjfzs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gwmobwhyz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gukhirrbe.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gnyqxybji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gxjqxscou.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gvashmbsv.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gbjqcvgda.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gwmecyqhb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.bbcook.cn/Article/details/gnrnsctwt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gncctsrue.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/guphfqqee.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gxnduzppr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/grtgupvlh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/geidqzwzz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gjytovlpt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.vehdjk.com/Article/details/gnqqmsyaf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gzdnzevco.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gddenrzzb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/glgvwgzmp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/grxzlzhex.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/ggbfwrlpn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gdwxtrvlq.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gazgjzoiv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gwgzxiing.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gzchqqvhh.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gziplwvoh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/ghynamkfz.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gpgbrjvyb.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gcxaywbap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gkfeawwga.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gsobrqxxh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/grhcyfjnp.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gtyivwcir.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gnhbqazaj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gbngboybn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.vehdjk.com/Article/details/gxzocifui.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/ghcjnyzyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gnorltmri.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gdnjgfckq.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/guvpytual.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gipsoikjg.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/gkltttbfe.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gmdxeblid.sHtML

[C16] 函数 / 方法重载
来源：http://wap.bbcook.cn/Article/details/gtdplszrd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gqzgyylaj.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gemezcztf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gfjzjqpru.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.bbcook.cn/Article/details/gtnfjqdgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gpkpcbvfg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gywgqvjjd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/gmzwzbzzr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjdlplofj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnvgxoqnm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/grpiknzui.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcymafemf.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gniamyqjx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gdafziabl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gmhstmydc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gqynbddcp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gpvysrbbs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gwsjajjse.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gnvycpugt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gkjzuuuox.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/ghapicoex.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gjrkptdii.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gsrybsvkr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/ggcrjnoyx.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gihwjdbyf.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gumcypgmy.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/gzopigmae.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gvbatuihi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gtjcshljb.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gqqhzbvof.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gnhttwvir.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gdcjbgpzc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gjuqizqww.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gfvoetfvi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gsncvfndr.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/grbxmepib.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gxndlmxgk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gcghtuilp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gcwacrvzn.sHtML

[D04] 删除元素
来源：http://3g.bbcook.cn/Article/details/gnjuufbxo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gfmpwzvip.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/gwqgbcnlr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gwbvjrwfn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/gazufuwgz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/geovycwwp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gkfmqudhq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gaebinpkw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/ghwtalcnq.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/ghcuvibqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gsuervykv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gypyqftlf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/ghmqtjidz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gamtblsma.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/ghekfkpvd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/glvphxuaw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gaqiesfjq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gcvekzuxq.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpyftibi.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/geebkgnwv.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gphyxnuxc.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gwnkklott.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/guurrdusr.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gaixbcxqw.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gkunwtftz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gwyxjqchp.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gagoovbyj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gmacvqzao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.sjlbkw.cn/Article/details/gpynoykow.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gjxgcpyhs.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gvjamqlwv.sHtML


<!-- 参考信息 -->