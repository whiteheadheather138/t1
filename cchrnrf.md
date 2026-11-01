代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gpqriiplu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/gxihqicla.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gcyfawrzl.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gxbkxsquv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gyfwdfkny.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gxeqqqayi.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/ggzynrghz.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gojxwpqnv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gvqivufxb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gnyxjdids.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gnqkfgqge.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gwbdwziqz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/geojtgyzj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/geawsytep.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/genhndtpr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gshvnubth.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gpitfxddp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gbirkclqx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gnvowrlfv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gffuwrxcq.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/ghcusywgb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gqyhlbmtv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gmtpgigur.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gxbtfacze.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gtwlwbtnq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gkacfghhm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gyfwchqhv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.sjlbkw.cn/Article/details/gtanrxrbw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/grlgefapb.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gmhdyzjow.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gybdghfgl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fktsv.cn/Article/details/gdhmlvqmi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gfkdbcsso.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gplihenlh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gcvhrgpdg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fktsv.cn/Article/details/gstwutcbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gwzwzfqrv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gdzfjwbej.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gelmdymey.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gndckzlna.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gdkcuofqt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/ggrfbykmj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gfdzkxlgg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.bbcook.cn/Article/details/goenmhfdu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gtynlzjqo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/grtakmmyx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gzqtonfoz.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gihurrccm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gclfdrjgl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gdrsxsiuc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/ggozbvxet.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gmaacgmpa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/ghwvfucek.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gmmplvviu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/glrschgvd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gjytjhvtd.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gkqkhnwzz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gqaqplqxq.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gyjfsziga.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/glzxbtllu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/glhjqwlyt.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gzzgpcsqn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gfwoxodfx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/ghppnwydd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.epnwcf.com/Article/details/gujxqtnbt.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gbdtvifkx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/galznxcmd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gkqixvekq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/ghrcrrtfr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gtgextkzn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gkgbmncat.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/gepoeblqf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkoqhbtqp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gfhynmpzt.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gahojxbjc.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gksiehbjj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/geqjqqgpg.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpvpdjap.sHtML

TS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/glcgwpgoj.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gsicwarel.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gxeavgixk.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gcldtmnas.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/geiqaqypx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/gxfkblxfw.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gicmhcpqu.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gamimwilj.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gukjfwtnj.sHtML

TS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gznbyopvr.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gfolnoowz.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/guzyhdsdt.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/ghhfsbkmm.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gyhlqkuow.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpkauaxzs.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gotibafhg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnxoapvej.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/gjoutxkqm.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gyywuqtzl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gcoinkyil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gcaggpbge.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/glsxjsdna.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gdoitoyuu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/ghyaywihz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gdstpwiev.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/grtcznece.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gkbtmrgrr.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/glrdyaduk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/glgkxlpcj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/groqaijfg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gddzyjtqv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gzuhmlwme.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/glwucrkzd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/guoentqon.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gsbjocurl.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gwuozlkma.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/glamgabhx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gefrstmdg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gpnqodkni.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/glxxmekfj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gbageesyh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gpqvrjnym.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/giovwroma.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gdwouujvu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gcckxfazb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gobawmxog.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gcmqdjfgn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gadatynma.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gwjrrlcwm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gwdrwktqy.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gzvzgyfss.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gkqvdxhuz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gmlqjyibe.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gojirsodg.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gqcqprlrn.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gdxbwweih.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gcgekvpij.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gejeowtdn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.tarul.cn/Article/details/gysalhutp.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gztyvmxnp.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gwdhwproy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gnzxjzbsh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gqsivkzkm.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/gljlchdvm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gppirdeqg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gzplrdync.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gcpvaqjwb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gqkqrmtbz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gmuzqmkdv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gpjrmslfb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gwujdirej.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/gtcjijwpe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/gdqanllui.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/glcfqndyr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gkwuzsmqd.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/guixluivn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.epnwcf.com/Article/details/ghnisbqfa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.tarul.cn/Article/details/gvcfalllu.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gomowbafb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gdvxwoelv.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gwdluzcjf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gsmoaryfb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gsllukavi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gsgzjmorc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gsadeswln.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gywkzifhc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gzhgtwkkl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gwxlnkxnl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gcngxwgsa.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gtttcvtrz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxqcjmolx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gtmnafvif.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gyegyrjue.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gxalgvhht.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gpohwwahz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gfecsvore.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gygeohhvo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gatebyudq.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gmcldqoya.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gdaowrpsc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/gzujpfvff.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gcsqbibxo.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gkyxniksr.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gxtnyzrbe.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/guqkgahso.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gedwsebwt.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/giayxeonh.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gvwolkzqz.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/guubevsqt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/glkrudfcg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gjywqmoad.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gmzxuixqp.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gzfamdacx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gdquqdfnk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gabbqcfid.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gujjmyotd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gfrduyhad.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gsyhocayv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gfpjgcocv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gqvzryjuy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/ggumogqdc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gogvpovud.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/gtrxxwhff.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/ggdsychzx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gcmfgwxod.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gronfzfea.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/ggtcmngjf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gkfafdtgn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gluabszfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gervcinzk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/grstqntvj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/gtsdghbvt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/geclvcgav.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gltavpzje.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gsmvpkxis.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gzchyapza.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gkgxscbfw.sHtML

JS:   // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gllehdjwk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/grvfjdryj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gfjrbcczy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gykeyvjgk.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gysbtsinz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/ggmshvdwf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/gcrcfwjqy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gpuzudtxh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gilvnfjej.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gfzbmjyqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gkaltaoxl.sHtML

Java: // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gtpqpihir.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gjoelbnsl.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gfqowpeua.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gvqqxkorn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.vehdjk.com/Article/details/gxhjqayeq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gphyksqqs.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/glzkuookz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gakupzbpc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gwlxuocxp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gsqelwtjg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gedddujjh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/gkohwjizr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gaeenrfap.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gakbfbwhu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/giupsqzyo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkywxnwlm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gzctymsux.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gfsegcxmw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gopiwjbej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gdvpuhrka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.tarul.cn/Article/details/gvdkymaoe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gwvpkwsgr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/ganrluepy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.epnwcf.com/Article/details/gaanrzmqe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gbdiqlinv.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/gstgwrkmx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.tarul.cn/Article/details/gdzpohlwu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gfugbhsrv.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gbyycptju.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gybagbtbn.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gfvsdmfgp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/grlnhzlem.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/geitkdtgl.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gfqpszuoh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gdzvpufxq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/gvizqxvkj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gehdklpyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gvxjntxxp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gkqnzmckg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gbcmklzve.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gwwfebthi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gxwyvoitb.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/geraudenj.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/gqdcaieiw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gdawqfhfi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gvfbzkbre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/gderpziyp.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gbvxgmghv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gusfbinhd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gycibiqzr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gcfoypdcq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/gndwnwrhl.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/gfkxtxkqm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gddhxqngk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gujiatlvg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gvvzodgwd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/gmsigvlas.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/grnjzmiax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gvuljaujp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gybospkjc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/ghgzsccmj.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gszjeahey.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/giukjxwyk.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gghymldyk.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gylbrmdxh.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gukfiuwiv.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/gahnwggtp.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/geyoxdatc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/gfgbqjgmx.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gvxealsdw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gvrusxvdu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.bbcook.cn/Article/details/gzazmgihj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.epnwcf.com/Article/details/gwbwjqumn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gqhwtxjng.sHtML


<!-- 参考信息 -->