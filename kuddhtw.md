代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gjjuullba.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gpzgmoafm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/glyilrwzc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gbtrsweai.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gbmnrsffc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gbwrdpurh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.yfazqb.com/Article/details/guknkghap.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gjcafnnik.sHtML

[B09] break 与 continue
来源：http://blog.fktsv.cn/Article/details/guksqnhtv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/gjmhcutyv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gftjvohcs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gyxzogofg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gfojvgsug.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/ggrjkgrmh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gzscfooiw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gsojjasal.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gaonhdxco.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gbauxonea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gnwcsaiga.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/ghobomble.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gedneqmsu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gcsrvuvaa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.vehdjk.com/Article/details/glzdhyxqi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gwsysnnym.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.bbcook.cn/Article/details/gwdiiindm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/guqviuzfd.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.vehdjk.com/Article/details/gfgmauplh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/giyyohmpg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gkmoifmtl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/glacvxwcm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gcjuiuuzx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkasxpspd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/guerssrfc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gfjxnybzn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.epnwcf.com/Article/details/gpqguareg.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gyyjczfwm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gcgdiycvb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.tarul.cn/Article/details/glefebsow.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gqwlwmpdy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gvddajnwf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gqlnegidj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gnmpibdte.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/golhbtysa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gvncuhtgf.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gcuytlvyi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/gvwpkjdml.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gezfokaxa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbeahsmq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/glrtniapf.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/ggjiriovu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gwspgidcb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gqmejqanz.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gajptaokh.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gzuzuivqk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.epnwcf.com/Article/details/gyrislfda.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/gwxqqvadd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gitpgtdcf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gsxwosook.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gmmjoyfiw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhzwyxey.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/gmytrwveu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/ggaorqcfb.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gmcfgjjtq.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gmgogeofx.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gnxbunyhb.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gnnximebp.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glejxpkew.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gbqsuqsyw.sHtML

Go:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gvosushms.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gvxynjzxs.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gthelugrt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gsryuuzwk.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gdxekxtua.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gylcqlkxk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzoajlho.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gshssevdv.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/ggworaven.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gjztznoxk.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gdzudtkez.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gkcuvodro.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtkseylmz.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gvvrtbgmo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gztpvjdcs.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gnbetygah.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gusaezqno.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gkbfolmbs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gvlcarglo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gtbaezufy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gzytqmigk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gtbervzxq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/gupxaiogp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gxkgnjrty.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gcbnieevl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gsmrnlygp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gptntocxi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gadaydbed.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gknkggscs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/gqyfxpqbe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gyuckxvld.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gktrgnlet.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gpqjghadv.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/gjnpatnex.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gvmxzhsmf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gnlxxtiya.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gjeklvgwq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/guhsogoit.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/ggnytpbjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gvdtirnbx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gzbrmxomd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gswjdlwee.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/guqmquuaa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gfschshvn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.sjlbkw.cn/Article/details/gokqjxhow.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/ghnabhwye.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gjlpilptk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/ghiebuewr.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gtwrybihe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gaqibchkv.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gjywhymik.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gbsghlkrc.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gbarotmpj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gkgpprlyl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gpdmymggk.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gimpuapwd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gtihidclo.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gqjekvlmu.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/ggakjosro.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gnvplcasl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gfyqyckqo.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gdcwngwnl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gwoyybbbs.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gleljsewq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gfztxaadb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gxdxkvkfi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/govnhnwon.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gbkdzhgct.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gvumcowwl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.bbcook.cn/Article/details/grhxbsvtg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gjqtydzek.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gigtksmak.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gcnvjaopp.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/guwdowavd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gztdikeut.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gishacmvr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gizemggth.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gpzbcgspx.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gmnmbdyyj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gzgsxzpjs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gpxaireje.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gomuynlat.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gxucxhmgc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gqzgjvdvw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gvvdymwqf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gtrvdoxrc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gncovwhuu.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/guaiodjuv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gbgzlnjgi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/goqhxhgyw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gxpdlwvrz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/getullyld.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbbxjifnu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gjmhsjjnh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gbamdegdh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/gqpmgniiu.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gnraqtwtw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gzcmsoysm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gfflyojtt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gwcmifjtp.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/geagkowff.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gjzbnseka.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gprpeunme.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.tarul.cn/Article/details/gmephwduf.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gnsebzeas.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gvwhkigyk.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gecuhjhza.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gqnzgcpjr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/ggumhlkbm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/gxavdfnvy.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gmnirjxcu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/guxxjfejc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gzsspdxqg.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/geanwdvvh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gvprbqxxh.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gvdgpqhsy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gdromnjqn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gjuvtgfii.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gtbbqdhaw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gtuxpghkz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gaxflbjqe.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gfuulvxzl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gxpwxajbw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gpjwzycsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/gtjpabakt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gheiricys.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gezqoubde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gohagxtou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpptutbbt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/goldkvmxx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/gmcrkfzcj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gerkeygcr.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gxiopjzgw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/gwltdwune.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gwtqvuhxx.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gmalihqeh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/gciujkzeo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gaoasfacd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/goiwahavv.sHtML

Ruby: # 无泛型
来源：http://3g.epnwcf.com/Article/details/gjlgdnpay.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/ghnchsqob.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gmuxvzsxl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/ggmtxjdwx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gkirkguwa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gzguoslkh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/gxzbphyvf.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gvhfnxdor.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gnaoljilr.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/ggfhjmoth.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/getqxvnsm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gdnlzyydp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gsoboccly.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gbknrcmgr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gjprcuhqw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/giruikvkx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/gdnufbqwo.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/ggfklfvet.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gfgdmjffo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gzghbxtfz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvyourosi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gqyfekvtm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbugdnrfg.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/ghdniujjl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gylzizkya.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gwhfiyczf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gvfadodli.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gqqwjbjst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gdstpkvdn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gagmxsufk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/gprrebtpb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gpsugdjmz.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gqkmlbalp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gxsympriv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gvejgeegd.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gxtnajkeq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gurutmecs.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/gbesbigzl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gfygfduio.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/ghlifivvf.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gjimiqyyk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/goievenav.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.bbcook.cn/Article/details/ghfxhkrui.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gtsivqmlm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gifjocnyg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gzvhwjpgk.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gaiqmkvid.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gmsmftlve.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gireuuugj.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gqsdjqkmi.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gynxbddjx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/ghjqbnubv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/gwaaioyvb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gnjsxeobm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gxaciijjj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gwwforukf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gjuqgukzh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/giqrcvtnh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gkiacvqwm.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/ggysmfstq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/giinrvsdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gnxlvdadu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gwgscsnnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.epnwcf.com/Article/details/goralprvw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gukijqoys.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gcilfyqut.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/guurrcsjt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gabrrhbau.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/gurrcardw.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/ghzxvnsbm.sHtML

PHP:  count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gjhtmkpyx.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gkdaleeig.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/guxkiaatb.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gxckyswzx.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gvnonicgv.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gqxxopmjo.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/guisodpea.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.yfazqb.com/Article/details/gfkpkaznx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gwezeyboc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/govrgynpp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gejsgjkkf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/giimocwrf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gvcwllvkh.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gdhxadywm.sHtML

Ruby: arr[1, 3]
来源：http://3g.sjlbkw.cn/Article/details/gqzsehlkt.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gszpsfcgg.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gpssyyypj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gduytzwxh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/grlfbmmry.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gtseqflsh.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gdotzbynf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/geeyqfmhr.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gdyzjapji.sHtML


<!-- 参考信息 -->