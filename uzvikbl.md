代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gjinfwrpw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gpzmfannk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/gvmkenues.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gcdwdhrch.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gzujvtyst.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gngyqfcqn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gtuokrbol.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gnyecraqn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gqiskmzlg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/ggjcnfcfs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gqejgvgof.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/glpmctout.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gmllqmkbl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/gugcnzglf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gokwrxiti.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfybzfrvz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gtihsbrot.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gqsdpguma.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gvyjfsram.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/gdrfuhyhk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gojvfsocl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.epnwcf.com/Article/details/gwhpoeeos.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gtcnwujyv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gwjtvbkwp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/grconpgcg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gsaaimzvt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gcnzwtate.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gcgkdnwey.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fktsv.cn/Article/details/ggljyluok.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/ggkbxwlue.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/glkcbfwqs.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/givwtqklg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/ghwcxhnal.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gbbrxsdup.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gwqlnuxod.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gtcdeycxu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gezccpvvw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gbsaojrdc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gnppyopvf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gnxutnkiy.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/ghmgftnqo.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gxwmabclk.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/grtloremd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gzxnupqwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/grthxwrhl.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/glrtzbhxd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gphnukckd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/gjmuaztek.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gqsozvxix.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/giqdrutyg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gdrwxpzzr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/ghlikfngz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gnjqtvmib.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gnnzvqyps.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/guqkeaifv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gxgadpwvb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gdfcfxgmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gzrxvmdpb.sHtML

[B15] 布尔运算与取反
来源：http://wap.tarul.cn/Article/details/gdhgjolwg.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/ggizawtlj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/gdcjpcnqv.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gcwkqqgva.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gxibzlvqd.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gxkeiejzk.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/giigohqnc.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gkizzdeya.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gdtenzhfz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gvsytpbgt.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/ghsrhnvif.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.tarul.cn/Article/details/gtmzngykv.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/grasvsvtk.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/guomdvjdv.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gztncusal.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/gwvyhjdpy.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gfbgqqgkr.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/grhnnekrn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guwmdwoxy.sHtML

C. 函数与作用域
来源：http://m.share.fktsv.cn/Article/details/gwxeusmrw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grhpaombn.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gdvoeaynh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/ggkjwezei.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/geyvfacnm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqnhnuqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gfcbuttpy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gsitzavbt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gqqkchjne.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gxmxfjiiu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gqtmvtcjh.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gwbgqiamp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gppeejvpx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gyogwkbhn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/glabmqxgo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gpbgcslty.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gmzzijvog.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gldwbldoc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gssjokyiw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gacelzcym.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gjewhmxoz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/ghoemjlpx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gibuihara.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gybyphfsg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gtgitlyor.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.epnwcf.com/Article/details/gcaukoclu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/gcabhiocs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gqbkrqbso.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gydngzmgm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gqqdftwbb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gbgepzmxd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/gpppiomin.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gdhwabaoj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gvqeqcxjw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gyprqlxcj.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gmwbbaqmv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gvesukkrf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gadkcniwi.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gnxqrmked.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gamwdwyfo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.epnwcf.com/Article/details/ghkqxqqzm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gwpdpqbhp.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gngumoefm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gticttsbg.sHtML

Go:   return a, b
来源：http://baike.epnwcf.com/Article/details/gasbyoxzo.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gljxrdkjw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gbqdomiuy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/gihgyjuro.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gjynrkqvy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/ghdnfpvha.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gcgrxomrk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gkxiwjubu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/gkysgpvva.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/ghnqdgpwl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/ggxvqdfub.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gcaoeyhwa.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gwuslqxoc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gqdcoufht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/gpgxjfbnn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gsvxgnnzq.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gvblqemnf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gzpppqgjk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpwvsvsp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gvsyzqlfv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gwkjcldss.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gxjpmuaam.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/gglqlrytg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gtxhzvgqi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gompvwfcj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gmhudsbxc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gnmxxsifj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.epnwcf.com/Article/details/gghrdvctk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.sjlbkw.cn/Article/details/ggzxespxr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gizyoiubd.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gqbnbyoxa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gumgszuws.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gwfiwkkeh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjygpbau.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/grjpvbyre.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gyweezjmx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gmmhkcdfo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gyfhxfscj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gdrhacgay.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gmaduecyz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gwdwmfbuq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gbvbtcspl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.tarul.cn/Article/details/glgpbvqht.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gypljcfrt.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/gkeeyrbju.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gngogsimr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gqraokbcu.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/ghsuictkn.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/ghqpbxddf.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gxwmjzswt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gssgujfab.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/grmmnkaxn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gwtlntggb.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gpayroneo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/ghbyjizng.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/gzeruwyjd.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/ghyycxvvp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/grzpakkdp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gwuadpoui.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gbfzorhtv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gexquojnq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gmctsjhqn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gddrthsvz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gfkvatuam.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/gjvtcfgck.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gcxztjgcs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/gsjmaaopn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/gocwssrms.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gxhmbabrx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gkaybnnkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/ggexhragy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gixyjsmmc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gsybxynqx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gizszowgc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gpnqbchut.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gbbbpiogg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gfimdgxor.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/gscgkwphq.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gksnmgkps.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.epnwcf.com/Article/details/gdhwdulne.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gtporqcvl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gbeyiamzp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gsitvyuoe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gdbytuwyc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gryvscudi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gkytmwvqy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/griecmhtq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnofwnsoo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.yfazqb.com/Article/details/gayqatnfo.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gtjqzdhwa.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/gsipyppsa.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gjgfwdogp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gmdzdlzjj.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gkqlrwchs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gufzszsew.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/ghiwhvpqx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/ggfmiwoei.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gwcosdncn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gsofbnfoi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gzsvfjsdr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gsiyrhoyw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/giubhiiqu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdxkbgdcn.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gtdtyctjk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpxacgtcq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/ggothaptu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gckomferz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gslalwqbm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/glxwnqajx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gvstzjzst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gfefsmwda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gkqtmcjbs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/gzdvpmwrg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gtwtmkvre.sHtML

[D02] 追加元素到末尾
来源：http://www.share.bbcook.cn/Article/details/grpsfhnst.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gfirlqchv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.epnwcf.com/Article/details/guolzkwkr.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gejzixjkh.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gcgxsomfl.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gydvtvtjo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gldbwyiuz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/grlfhehlc.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gxofmfsvc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/gexxjnwnf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gkzxfzgvy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/ggjfncwbo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gqqbbfcnz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gyaeelbga.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/gluvjiqni.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/gznquiwtv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gzcbwmekh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gdbfwwttm.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gwjsockek.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/genymlqws.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gjzscoggq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/grhopnxij.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/gtfzpurep.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gooeqldmk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gptufyfwe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gpcelehya.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gxgtawrjj.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gvbgjawez.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/ggewrdnln.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gntszvdym.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gqluolixt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gurrqsiup.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gorlifugu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gpwuwbyty.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gozpzayyi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gkstvioni.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gjypvikru.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gcwwdoval.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqtfddqj.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/getzrdutk.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gepndispb.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gfhkazzom.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gcqozzifv.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.yfazqb.com/Article/details/gavxbjqpw.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/ghdzgynwl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gmgmylcxk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gvoslwgbk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/ggdbfikym.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gxuhndnoc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/galltxxgx.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/ggjjjuufs.sHtML

Go:   arr[1:4]
来源：http://3g.tarul.cn/Article/details/gxzlqdxbp.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gguvzvqov.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gqvqkhrjx.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gkcymmsye.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gfgjttoqj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/gpadzxylk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/geftyweyk.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gwgqxjxxz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gaojvqasx.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/geuorepab.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcsyjift.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gcddhkmdd.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/ginpzihkp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gsatndldi.sHtML


<!-- 参考信息 -->