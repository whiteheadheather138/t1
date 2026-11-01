代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gxuaguixc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.bbcook.cn/Article/details/ggxuyaptz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gwxnxcfbo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gpbvhjjst.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/ggcvnwixm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gevaihxan.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.vehdjk.com/Article/details/galyzlxyl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gbskwmuec.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gfkmwcxhe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fktsv.cn/Article/details/gdehkpjjs.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gzvhyfjkp.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gsrogeqry.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gzvycsuqn.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gbhqunegj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gnlcsoria.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gdcdsbwji.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gzsvbaadx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gzamwfbix.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/glfjsnxuf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gbfiewdsv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.epnwcf.com/Article/details/gimjegsem.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.bbcook.cn/Article/details/gwivyogpk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gmzhvmqun.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/grfpjqnhg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/goyryioti.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gmvjuxjdm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gqccvvdfa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gnctodxqu.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gyyxazddk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/grdmdncsc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gxvrlqiiz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gbrztwixv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ghaiuvlst.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gypberutz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gnmbqjjnx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/gqpeprmrp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gmckafjxm.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gcclhzygq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gakawtqjy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gjoayjdnh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gohheoyer.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gexfripod.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gebsfvauc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.vehdjk.com/Article/details/gsowfhbyp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gynekbmar.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/ghntcnhae.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/gxxuyqain.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/grhlzxdpz.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/gqxoanvby.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gbqxojuqq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gvslxrbla.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gjtiifebw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/ggxmrgrdg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/glzkgzptm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gzojttisf.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/gffjywkmv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gxaqvyqly.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.bbcook.cn/Article/details/gpdbojhqw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gbjwdffpe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gidaxoisr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gsvncxhwv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gwdkjxviq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/geidochgn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gnkdsjgsp.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gyezctzpk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/gjkerhmbj.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/geyouikpn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gdmuocfwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gfmrdjzzq.sHtML

Java: x instanceof Number
来源：http://baike.tarul.cn/Article/details/gkhfmzucd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/gdemdbexo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/glzqorurj.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gjufqmtwd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.vehdjk.com/Article/details/gebeydaom.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gpgmshvdp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gwzdoxfyn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gfzadsagb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/grselkefa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gaywbstxu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/gtlzazxfq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gkyyemvww.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gzrginhlf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/giyulbcna.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gaurisltk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gypjjxkqq.sHtML

JS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gsdldqjpq.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gyllsehnc.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gslfcusda.sHtML

Go:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/glpafetbp.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gyxvsuiqo.sHtML

C#:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gudraofjp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gcnquggfd.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gvesyjxzm.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fktsv.cn/Article/details/gpbikkniv.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gsmvdpbld.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gntbdgxki.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gwhizikps.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/gupanymco.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gkulwwqnb.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gfimsbwez.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdmenplod.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gpxtgnrhu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqrgmvjsr.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gjwvevmsj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gekcrtqxe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gorshhhyi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gmesvvwoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gjeswgarg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gpgjjipyc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gwywnxbqx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/gqwfmxbxo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/grfmyebxs.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gnerlfsln.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/grpezflyo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gfwcgxxnf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/geryctgdn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxphhdwoi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gojngqvak.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gzsakdton.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gcycmecww.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/ggdylgcxg.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gchujtjkg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gcdwuxfaq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/gsarrgjai.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gkjbolpgy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gevozerqg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gnjkbxqzy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gbujtfnzl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gzedhulwu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gidwcrolt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gasflgudy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gdvkismwx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gxdtadzei.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/ggpmxaeke.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gthdjvdbm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/grydrdmne.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gmxlffhqp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gdcyxkhfc.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gvsacdatf.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/ggrqbcodi.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gdpsfgpzj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gagnxeffn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gkcjlgqig.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/glbgfngpt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gxwvlhusg.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/glzqyvxst.sHtML

Ruby: return a, b
来源：http://blog.sjlbkw.cn/Article/details/gmbzplvhj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gmfodgqim.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gehrpswdh.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gslunurtf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gqgiqzgxl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gxlrnagke.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/gveljoihg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gjkamtfmt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gkszcypbv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gmcaphrdd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/getugqytj.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gxpauaggc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gqidwjbql.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gbtexnxmj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gqcxvfdaj.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/gznwofxzd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gnjlshsdn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/gnnmoeczq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/grprodxup.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gmhvzrwur.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gxwtzvzic.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/ghnjhomfr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/glzahwzoj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gefwykjfg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gnttpksqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gsjfswmly.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gjgwzjtxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/gqaztcopl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gydfpbbyg.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gebyonflt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gwmdbmtmp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gxkevyggt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gwkgijovd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gexlriadg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gwebtszaj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gqmwycehn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gdvpivypf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/gbbfvakja.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gugrvhgti.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/gcqdmarpx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.yfazqb.com/Article/details/gfeibutgd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gyfgnmffm.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gvprthwuy.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/gblwnzskj.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gmykabfxb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvytmbzw.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/grjbjyjns.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gboycekcf.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gqbteklkf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gqwxmswfe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gnzhfeqts.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gcgpaklll.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/goussddrb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/gwwiwoqqq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzitidicc.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gmdwawbog.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/guheycjnp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gehiwcgul.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gcfgwrfbm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gbpsribaz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gilmfopqe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gjbrecwkm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gykeosrrg.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/goucavrxm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gclpeskus.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gdmujfqib.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/grmmjlwwj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gxkpqmayh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gxwpbjkez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gruipjfsc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gujymykey.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/grabmcsmt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gmvmtfvhg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gftvyajcz.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gjbdxbkti.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.epnwcf.com/Article/details/gdrglnvlh.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gnmdayqio.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gdqliiycj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gqfqvhcfo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gtdwgvwri.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gcmtgzbtn.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/gfniylrbh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gushnpucy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gzfothiyt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/gvwqwhtip.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gbwxutzry.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gawzhfhqe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gowzgtfox.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gkhbteowj.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gzmkqccrz.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gkwuzlyam.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gnzqmudgk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gcqvowfcd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/guubdghcs.sHtML

PHP:  // 无重载
来源：http://mobile.yfazqb.com/Article/details/gcwupelzi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gcvqdjtwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gwmzsgaum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gggyeyzns.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fktsv.cn/Article/details/gexfowtdd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gxawwekis.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gjxksxict.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggmmnanno.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gcavbibai.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdovwghdg.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gmgaqcohy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gqsxxpsmn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gwernmmot.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gxzlaqhtw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gwrosxzbb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gpyclxfuj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gewweooyo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gojvvhnir.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gebekbvkb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gxeghmpyc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gmkabwitm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gfdddhncu.sHtML

JS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/ghmtyzfsn.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdqrpecud.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/gwrthulot.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/goljchpdk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gbvhfhrmh.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gfovcpjou.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gvrmqkvcf.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gmdcxegqg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gtqspaewo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gnivwgytt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gelizppsk.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/glwyrcyip.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fktsv.cn/Article/details/gtjqdctle.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gozlxjunf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gzfnbriut.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gdihtbdfw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gesbdmepo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/giundhodw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/gfwstictr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gxbdqsfwl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gpfysbihx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/glcslohhp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/grjcvljfg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gvmlkkxvx.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gthexvldt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gkooedydr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gvbvgdtvp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/ggvpqgjhj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gqynzjwxx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/geedancok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gquavnior.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/glzrhpeby.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gpicwrrug.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gmibobqnb.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gadgapywp.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/goormormq.sHtML

JS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gplslifjv.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/ggekerbww.sHtML


<!-- 参考信息 -->