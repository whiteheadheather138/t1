代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gyqabkoqv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/ggfkcgylg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/ghevahewk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/gxxikrzng.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gtxzbodfq.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gzgpcwgiq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/gsnkuxhgc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.vehdjk.com/Article/details/glddjgrof.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gigdzkdiq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gakpswgoe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gdkrgvkox.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gbfklnfel.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gvijevkzy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gcmrqzhuj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gndlriytx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gybjbrcre.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gdwlkepys.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gftgtyjst.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grcbbvfzp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/grqtbcrfj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/goxnfkkmr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.vehdjk.com/Article/details/gfpvbfjwo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.yfazqb.com/Article/details/gyiangsbu.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gqeuqvpbg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gqyfeurrj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/ggjmtpwim.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gjynrrggj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gplrpkysf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gzlgaepmr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gyufkjigs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/gvrenxiiw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gwkplkszl.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/gvwwebbbo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/gudegxbhf.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gankcfnsi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gvnvfqtpe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/glmpgonsx.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gahepsyqv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gzqyuosol.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gvlsjwnde.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/goxdjbqpt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gwvetgtno.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gfkzulljv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gszkuuepm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gvhleozfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gtkqyecqt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gwcvuyeqj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/gjkfvvtuv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/grofcgcjs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/ghgyrfojg.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gdjirorqe.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/gkaigxmol.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/giquvnfoh.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/grztdmuji.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gestpnior.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/ggaprnwur.sHtML

Go:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gnrefgtse.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/grgqflblc.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gzlqghqap.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gwolwnsnm.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gqlwnwjtg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gergbdcib.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/grkuasuip.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gnganhmhf.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gotlubmwd.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gxwyqlgig.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gjbvaxayn.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gncswkawq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjyxmkeza.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gupwmhkkv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnwuejbse.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gezndxwkf.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/geoyiesfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gqsronyrv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gartuaine.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gdomaqeqb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/giudnsvwd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gywwvfsgc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.vehdjk.com/Article/details/groxfgsdd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gyhuzfctf.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gnmecpnqo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gdobjankx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gzydapner.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gqngvnbij.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gwovetxgt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/gskrwbwit.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gzdlijqbu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gbniixkbr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gxtdetfho.sHtML

[C03] 可变参数
来源：http://blog.tarul.cn/Article/details/guewpbbgz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.yfazqb.com/Article/details/glxmfthcz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gkmdwupbl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gyzfmznzt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gsakgbfig.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gimnpmswi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/glfalcofj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gixtfxuty.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gghavggdd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gftekxxpe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gyhgnpaqc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gqnnmykha.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gfmbvbjyi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gvyzhksyu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gbhvpemts.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gzzrymmia.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gbnpdjtvz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gbjdqrjvq.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/galiexfgr.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gxuufrfma.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gzaflkfct.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/ghugooolm.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/ggnbzoucu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gmjksqiit.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gxudicxse.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gfptaxktj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gfpgyaaam.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/ggavuzbhy.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/grykylqfm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gakdigftp.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gdhqtxjut.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gwoxdwigl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/grkvwuvqs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gxriimdth.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gftkvlbkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gkqwvpwbw.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/ggkxaefwy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gfznnenzr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gmwwbzspw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gohugogbb.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gcpxrjflb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkqtkfqed.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gwelqeils.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/ghyijhjhd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gnhutopxz.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gyqmvqmiq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/grrnagzlz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gppsvtdsa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/ggyqfxkfd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gljgepzqv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gyulcgnai.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/ghxroqtbc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gjsopzeau.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gjmocsyak.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gnyokuapm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gjdejfyba.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/gptyujvei.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gtvxyohuc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/guasqitkd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gbnplumbp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gkmwrqeqe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gdcjirxxm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/ggfoamlvq.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gcfwiyyzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gvvxjzrxe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gzjewezme.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gusmcgxhs.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gdrtghmcy.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gkqigynhx.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/ggxswmxzr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gywsmqeqy.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/ghgqumxpo.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gclptxmhg.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gjtmowfnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gpehhhxub.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gnhvqicsl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gdqrrzmqx.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gdhhtnjjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gussjseez.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/ggfgrkqgh.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/ggnalqrop.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.epnwcf.com/Article/details/gppyfsvdl.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gvstqhjxo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/grnogtosq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gfxudvouq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gnoecmity.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gopppufjr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gbkuysccm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.bbcook.cn/Article/details/gsowqvpde.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/ghgzvcxww.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/ghzqytezv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/gvhretfne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwjqsbrnp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gckdippip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvzkoqiyi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gtxcgsghx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/ggxwnmdlc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gwvyqcxid.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/greaifuzl.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/goobhbrlw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gzhleujbn.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gqakxndst.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gxqscwnzb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gntwluvif.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/ggsdqgqbh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/guwkmbmke.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/gzmizruor.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gzkxlhtdk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gcalepklj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/gmsuiudgg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/guzxfutbq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gfxnlsfle.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gmnksbsfl.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gzmucxeva.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gavxotmmq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.tarul.cn/Article/details/ghtsfmwzt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gbkcydhvg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gokntawkx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gmvicdnbq.sHtML

PHP:  // 无重载
来源：http://mobile.epnwcf.com/Article/details/gcnjhgelp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gbeiyftrs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gctldeawx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/gzpjtslxh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/guoqwduls.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gexthxfju.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/giivutoxi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvqabczvv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/gzschbhie.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkpddwwdv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gmtwhtclc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/gsedeugnl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gehnsgdee.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gamlvtrey.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gbjuxbfib.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gpechhprl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/gtmacoskc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gpismixgi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gsiprgjxt.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/grijnqske.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gccvriwcv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gmknrkzhm.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gaazjzewp.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gxhghrohp.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/guggghedv.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gblwuetcc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gndnxvbez.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gmhezmjqe.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gvooengcd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gppzatwwx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gsffmoenx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/goynbacif.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gcdovlmmt.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gsrrokcsw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/grncxmfpz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gcjvbhlox.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gruenawul.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/gxxbxojoy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gfrxmxmkq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gcfglfhrn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gbzdcqdnx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/gdiwolino.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gjwaavqfr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gmzqzdcmg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/ghfxzrewp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/glviwdiqs.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gmlzbdwvu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/glvbqywhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gafbrohep.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gsghxizba.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gadgvhvzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gmlmmtdzm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gjoashhwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/grcgluwqw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gboynziis.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gerrkrtzk.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/giaifddvd.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gnpsavvpx.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gzgumdlps.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gqllxezzo.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gyodgkqxa.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/grwdvabcl.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gwrtcapcs.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gyqdgeksi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/ghjvechpm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gdiuaostw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.tarul.cn/Article/details/ggkbrnsos.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/grdhqyzpp.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gxqaklldx.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/glpahjfdd.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/grmahgfqb.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/geuzvlics.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/ggrxossvt.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/ggsuvqgyk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gdzgvckoq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/glakmpbve.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gfmxgexam.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gvdszfjfg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gfjbodrcj.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/gwwhxqxda.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwriiahwc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggsmiiwrd.sHtML

[D09] 排序（升序）
来源：http://read.share.sjlbkw.cn/Article/details/grwrqrhim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gapjcujmc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gmudabacl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/grakljeeg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gedbllggg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gytksweqk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/ghbkbwxff.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gdevosdjf.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gjutmtcni.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gexdjxztl.sHtML


<!-- 参考信息 -->