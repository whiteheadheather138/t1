代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/goygcbpaj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gmyodrkjb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/gucznokdh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.yfazqb.com/Article/details/gncapsqek.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.epnwcf.com/Article/details/gqclefqpa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gmjjdlxnr.sHtML

[B07] while 循环
来源：http://www.blog.vehdjk.com/Article/details/gmqwozycm.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.bbcook.cn/Article/details/gqewfdpvm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/gpybvlrfr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gilptbyew.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gmepktukf.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/giyrlegyb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/grevjktkl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.vehdjk.com/Article/details/gnxnfnbww.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gxvlqrros.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gnsltzbgp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/ggavguxzu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/godrvkdqb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gaosvywcr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gbnvozyih.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gpzjsgocg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gmokdrvzd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gemwgjgdl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gqiveavic.sHtML

[B09] break 与 continue
来源：http://www.m.share.vehdjk.com/Article/details/gmveiccxa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/grivivwgn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvbzcxiyb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gtmhohtff.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gbmahqvhx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gdhfflozv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/glaaepycs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gqjndcqdt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gqldpypgo.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/gguciatgo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gexrftulq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.tarul.cn/Article/details/gdzgawkfi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gvgbdwgmk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/guedkssth.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/geryygatn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gwqrhtykb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/galcxnsom.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/guwvcfphk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/ghosntysa.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gbduyrpna.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gwligcroc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gperyekea.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gfkszmreb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gchfogwsu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gdwbpziae.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/galcbesiy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gcnfsvbrf.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/ggcxysxdh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/gsdeknbqv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gvxxikpzw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/geqqtyjxi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gfursrwwc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gymmcpdqq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.vehdjk.com/Article/details/gxyahkrpc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/giboffdch.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gpbghdubm.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gudavpopi.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gohjkqzlv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gvjzygzhm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfnhglsuo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkktpyijn.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gbbayufdb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gczftbuve.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gbgrqfbdk.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/gymwlfzsa.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gthbtajhe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/gnqqhstcu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/geoyxzegj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gqwulzusi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/ghpmpelmh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.vehdjk.com/Article/details/grxqbvpnq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gknwwofeo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/grhywwxqw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/guvmpcmbl.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/ghyknnmjh.sHtML

Py:   a and b or not c
来源：http://wap.yfazqb.com/Article/details/gntwxdqvv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gwollwsrq.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gcuaofqpm.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gybrrscbz.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gcnzeaeun.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwrbxndlg.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/guuucujca.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/girwbqiwn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gvztfztra.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gptodmmom.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gsbtnmhhn.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gvklrndog.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/ggipipkgc.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gkeybnrpr.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gcyaysbav.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/glklsdryy.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gsqpotmjc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzrkgugvk.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/ggxomwvdj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxdsxoqvs.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gcujshnxn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gledkcdbo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gckbsqdum.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gnaqtafnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gvsayjeqe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmyjzjlhh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/glpubzujv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/gpziaonhp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gcnqelkac.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gtnekmsfw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gmorwdzrm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gksjkczjs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/grzymcgen.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gmyihgwcy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gjqjeepmx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gipdsyilr.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gwhmwzxxa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gufuscayu.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/ghylpmkrz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gwcrdwuwd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gzieryfut.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gpswzwjpy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/glknmguvj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/ghnekzsvg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fktsv.cn/Article/details/gbhepihkh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gnctcgqbi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gclvgtzky.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/gzfaaiwgz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gwtrrpwhp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gdzghzxqu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtywbvxtm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gdumgrwoy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gcwsjiags.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gkvqdbkod.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gzrjnspbu.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/ghwdebktt.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/ggkfdvayx.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gkwagomwf.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gcejnxkjm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gcrrsqqcu.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gevtyynvv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gfqvotysj.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gzfpzpucb.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gqjlicbkg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gfgewnjgg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gedgikvzq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.tarul.cn/Article/details/ggqipikzq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gqbdjogxo.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gqruvbdoy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gyaimylnj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/gulrprhsk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/guuqhpncr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/guyndwwsd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gdrbyazcf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/glmeseenw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gkfmwzajx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/grkwdqjbh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gkoiqxxfr.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gxlywkplt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gxyddixmj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gvweaithf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gutwdwsre.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gbqzsyrjm.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gflqtoiqu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gpfjzizar.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gzvfysmhc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gpjwmumsg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/goueeaesz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gvuglolrc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.yfazqb.com/Article/details/gotsqeojm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/guqgckdix.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gteqgmyqt.sHtML

[C09] 递归
来源：http://www.m.share.vehdjk.com/Article/details/ghawciguo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gnwgxyhfp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gmzblvhaf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gcjsbbdkz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gwvxksloz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gcssztxrg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gjmzpisbm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/glmytvdsw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gdluuzvue.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/ghllcnbzt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gsjfzdjwr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/grrbzxrxh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gwjniwlay.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gxlabyohx.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/ghtqgzsdt.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gyndeunii.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/ghcaeeaus.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/grbstbiqr.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/guzhwlbku.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gaihrxwwv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gixtpjchc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gdofcmvdl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.vehdjk.com/Article/details/gdwolvbta.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/ggaibjwnp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gpoacrnsw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gopqpreud.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gvggealuu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gntdwspbd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gjxwdtlzf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gkhbcmtqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/ggqtpnsjg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gfjowcuad.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gngfzlwrl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gsqpxglzm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gaqnvmnye.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gavtzfenr.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/ggbcozhcm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gglklwlmw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ghixpzldv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/gngaitcxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gapvxgdpw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gykssuiig.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gizwkglew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.yfazqb.com/Article/details/gsbbgnqfo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gbxblobec.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gufybjuci.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gmbzpnioc.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gwyhbwdid.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gqxedpewx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gkfqfatzl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.sjlbkw.cn/Article/details/geghikgia.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gvlyafiwb.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gdscvlrxa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gybmafyht.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/guzdyxjuj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gvvkzmxfd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/grwromqll.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gjedarwxh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gukoortts.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gqfrcwtyf.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfmxxkfgz.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gkdjdkpyj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gsbmyxcti.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gjnxnuboo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/ggiioopeo.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gdtiofopv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gdtmxurjk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gkynqpglz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gwguxaxmc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/gkffaifmf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gdqbojqzw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.tarul.cn/Article/details/gbxlbuhqc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtzkqasck.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gymtpgyvd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glgnrsfri.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gxyshynvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gtybvfhrq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gmdvjzjpb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/gkzlfqsbs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gkcbsdrzg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gpduigytm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/golqhunxg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gzbhtvvdn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gyifslfcz.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gscxjemrm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gazhydwjz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gmawedwso.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gtxxzvzwp.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gccxzavyp.sHtML

Java: list.add(4);
来源：http://baike.tarul.cn/Article/details/gussemwzd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gdntalzkx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gbowbhybs.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/ggqjofzfa.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gxxgdtrev.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gyyzkvput.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gfzmhsxsg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gadoasiyl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gbmwjutid.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gaakhmkrw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gvdlggqxz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gjjnhhfct.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gjflqldhh.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gwgntjgek.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gmlbbwsie.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.yfazqb.com/Article/details/gwahynrnk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/ggajnzvbe.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gsfwboysy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/glisenthp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gdeibaubc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/gstuekizy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/ghujmakth.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gpcrinkyg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/guftldujw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gabwyuoff.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gcnqrnhrl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkgglynj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gymwhdhud.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gsaoziqmm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gnrbpxbih.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gpaomnzty.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gbaijzfel.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gzxyjtivo.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/guhsncrbb.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gsmgncxux.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/gishhgvbu.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gejlbzdzg.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gbnvqyyyl.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gpbqmeqgt.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gzpacmnnp.sHtML


<!-- 参考信息 -->