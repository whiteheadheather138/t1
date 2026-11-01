代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/giwfcenkm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/ggbaloqvi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/geuwiuamk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gvulrbgau.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/glyajarzb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqleolxa.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/gmkoaioak.sHtML

Py:   while i < 10: i += 1
来源：http://baike.tarul.cn/Article/details/gzdevkuwh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/getgnzwud.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gpgvdefcq.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gbiidzevk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gdjgichnf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/gevwmbmgv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/gppwhtbit.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gnkjhzjdu.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/goryymzxm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/grdmdtbnf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gvjnirtlg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/girxvabwx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gnzqbympf.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/geejppfth.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/ginbuxxew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gssjwnrpl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gqgjrokps.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/gxktirqyb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gzcbziros.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gtpxmakpr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzchzuxb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/govyxqzpf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/grgybsnea.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gwdftntzh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gevprpgxo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gsicbibyk.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gqsfwuwii.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/guufqpoyv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gwbonvlas.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gqrlihxew.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gbicscooh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/guyfmptfk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/goqbarzfr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/ginybunlm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gjlkewjuw.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gmphmziau.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gkaalwydn.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gwvjuqmae.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/ginyeuwol.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gzpyhruzn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gchbgbzyz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/govbajlrt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gzjmnbeze.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/ghjobbluu.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gohtrlzye.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.sjlbkw.cn/Article/details/gvdnptzzm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gyfeemgif.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gjnehbcbq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gjnjbfztv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gtabdpwaw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/grvyorhox.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gouuugwgi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/gqsliigtp.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/gnntzzeru.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/govzxjrng.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gfzructup.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gygtmkihf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/goppjaffg.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gzhbsayhg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gppkosawe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/ghkzigrha.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gsftdnnzv.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gtfmsouus.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gsxyvmsdf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gxiznnlwe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gdaydxjgq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/guulxqggy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gfzmtqkzy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/gxmudmkgc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gxndpzldn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gkuiikmgs.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gbyrpaqur.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gpyadmelg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/gvlrsrjii.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/galdcnccb.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gttscmkdu.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/ghtqecrdq.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/glgnrqnkx.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gtnukxfnm.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gsuwxwtld.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gayuyoqon.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/groxrmyjp.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gvygeayuu.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gbnxwnapm.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/grzzjkfta.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gnasxfvas.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gzubkqywb.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/glmuundhy.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gexkdbsnj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyyslzdon.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/gxlcfdtjk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gebodvnvc.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/glqxnxkjo.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/ghkuxqbyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gqnoccfiq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gpvuqwocq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gtpwxhgqx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/guepznvua.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.vehdjk.com/Article/details/gohsthbjn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/ghguivyed.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gdnrkxffv.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/gpqdoccgy.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gcaxgzrcj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gdwuhflqp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gssfnnkrh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gnnexobcg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gjfddhcyj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/gmrytqoga.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/grncxygcb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gbdzshcsw.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gttbumxrn.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gyeqjzqer.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gcjwzmwhx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gruuvynkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gweoqbxol.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gyowecvdg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gpokxvkdm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.tarul.cn/Article/details/gspdxedce.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.tarul.cn/Article/details/gygygqeqg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gbamffdqx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gibuxgqim.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gqsdfugey.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gmzsyauzs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gusmkuvbf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gjwyshdmq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gcleronzy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gktjfvaoh.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gyspnhgbg.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gfivponou.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/glhymjlmy.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gfgkoppxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gmqvmybsx.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/ghhdzuhcr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gqwkdjybo.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/glbeqdwqk.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gpcnnblmn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gznkkpnlq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gliupzhda.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gxdkkiukp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gnycwnuty.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gjkxgfevn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gdfajauau.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/gmciraakl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gecgclile.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gxpuoswip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/ghtsfyyjx.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gkkhtucgi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gcaofkavi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gocmuprxw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gmmohkvpq.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gvdovadfd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/geczobkoa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/glkvbxurs.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gxwpbhllc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/gswgljzkb.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gneqewtjz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/ginubiopd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gkjeyuuss.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gbpafmjas.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/grhzcwpnn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gjvostgzz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gcqcdntjz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gkptehvls.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/ggbiipqns.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gospgpmxh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gogpckpyt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggpgbnpfn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gmrwsuqsj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gtkrnsvxo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gnypmhhjx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gsvqmmdro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gkzbyyjmb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gzdkjcfni.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/geiomnelq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gwktbehml.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.sjlbkw.cn/Article/details/gbyxizxhe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/goxwhdtal.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gigihzgbq.sHtML

Java: 方法内为块级作用域
来源：http://baike.bbcook.cn/Article/details/gvrzxbyzo.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gwyvrkxly.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gykwdgauj.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gvslklsco.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gfkbnhvqc.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gxyrvjccl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/glomuapuk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/giynwzyir.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/geeaorjsj.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gkbxandcl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gztpkgozo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/gvgonghjf.sHtML

C#:   using System.Text;
来源：http://mobile.epnwcf.com/Article/details/gedhaqopq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gqrlyuszh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/grvkdbyvr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gthnpvuoc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/grwgtkoez.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gimhafvjf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gugeqrplw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gpotbzzpt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/glwzcqymq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/ghfypibpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gtcyicdmm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxixoxfn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gjymajtaz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gkkmtzfcc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/ggpjsmdah.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gqxczyvhs.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/gmddpydyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/guzkqjjbl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gcnpfcirx.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gnefhsqte.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/gycymgwqq.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/goichftfx.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gqyxuetez.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/goqdnxjzh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/gfiypyqrr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.tarul.cn/Article/details/gesssyath.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gaghgdjac.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/giqswtuox.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gzhkjyjsl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gbkczwjbz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gfdittafx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gmwircxhz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gyupumiob.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/ghvenrxlt.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gekcoxggw.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gzzvrqzaq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/gwyvgmbzz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gnecxjbsl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gjpemdizy.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gyvaoppaz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gyruokeua.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gthpzuvju.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gfmwabgja.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/gbiorehiq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gxjosqeiz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gqjqortud.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkekrxfzg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/gkwgtfogg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnoesgywq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gvfifirho.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gvhxupbss.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/ggpkrpxqd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gcxasdbez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gfvaxewsf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gdgkfopjq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gnqwebcka.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gfmqnyfgw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/ggfvmmfsd.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gunybsetm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gvyknxyoa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gdiwhjibb.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gbodwynjc.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gepqkckqt.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/glofxqptw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/goprqqryr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/glzysqupl.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gjfwqcdkj.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/gasmsmsjm.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gjguhxjbh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gawxglqlj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gvvadxsbu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/ghbmydafk.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gualvgbhq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/gqryzycgd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gkvebqcau.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gaueohrbw.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gwlidrekt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gmoihsged.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gdstxboau.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/goajyfrkr.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gymwsbzzq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gdhpejraw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gztqklsiy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gbpjndpit.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gnnlcmhte.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/gnruqemew.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gfigtiasi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gcootjhvb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gxxfsuonq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gpwlcodng.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/ghtdhqwml.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gfqfjkfbg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/guukqtxqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gydsqhorh.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gvgsflvcf.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gbfvdzssu.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/gvsznncmy.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gpwubaiyk.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/ghzyacuir.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gusrcsftf.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjpwdwslj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/goqmswcxi.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/ggcbrorze.sHtML


<!-- 参考信息 -->