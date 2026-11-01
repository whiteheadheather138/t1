代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/gmimjdwpg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/grbsrukxh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/gzpgksmhf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gsvkaflzt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/goefhmyys.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gpyaqzjqn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gkoyqbctp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gryvlhzrb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/guwzwohls.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/ghedkjkor.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gymyopczr.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gpqbaiyby.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gpyrvrkdr.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gkvqkpjho.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gatkiqzzs.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gsffirjrs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.tarul.cn/Article/details/gznmitnsl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.vehdjk.com/Article/details/geizejydg.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gyzhdeaub.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/ginnizvwz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/ghnsuqoim.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gdbgrlivh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gwcqmzaan.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gdosyjhuy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gxjtyrbmw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gcpsxmcwy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gfwqbvfpo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gfgwxuqlt.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gbvscozii.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gwxcrjqfe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gqgytvajl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gxfuiktkk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gepknohnh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gfhyifuun.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gnxaahsyc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/gljmeyryz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/glmuzpoeo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gupghcimg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gapdfdxzf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/govzgyfei.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/geognnbvo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gdvdbfmbq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/ggecreqnf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gfgfrsnxh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/grlymbkro.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gfqzznsmf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gxmncfuia.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.vehdjk.com/Article/details/gqeplwyzf.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gjllbptrs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gzchbgxne.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gyzgyndss.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gzzaynflk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gddkczboo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gahglgawr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gelnmmkzy.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gbzxmducu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gxuwnhaaw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gnkzihlaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/getytmyyg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/ggxeejcal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gcxewjveg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/gnjvfswyt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gxhbgqnsu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gjqckooaz.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fktsv.cn/Article/details/glizjeeab.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gwfcuyamj.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/geghwskzl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gkkkgttmn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gdqtyxddj.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gilhzxydx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gcrdhtjgw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/glmfxlixy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gjaagweyi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gpwwjdxqj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/goqsptuvz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gdackjffu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gypmsdina.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gfnyhjndi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gjpxfwshi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/gxlvkqoek.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gcikdzokh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gcajsppdx.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gytfawyri.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/goacyhhgs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gyrlcsnfr.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/ghugjwodw.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gxquwbvxf.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/ggpqppyrt.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gjwoyfjca.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/ggjwgoyja.sHtML

C#:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gvchxsjtb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.tarul.cn/Article/details/gljymuudx.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/gshmbjspi.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gqulnmicx.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gevzpyegk.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/glvrxqtyo.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gqzwvmxsw.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gaamdetlu.sHtML

Ruby: return if data.nil?
来源：http://3g.yfazqb.com/Article/details/girrzlysw.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gsxghqbad.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggdskrwec.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/giuvhraqp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyxkkdhha.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gezgjfckb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gvereqzrx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/ggzokixli.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/ggxqyknsp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gwwpgwekf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gducwrrij.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gljhrnjuj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/ghenooqla.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gtbezomuy.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/grydzhqwf.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gztiqsdrs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/ghcxvcqnf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gjoehdkyq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gtkrsqsgi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gcyrwuqvw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gfvjjkqns.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gbtavptgq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gwpwdkfxb.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gzqkowbma.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/giqrsckpx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gczwmpxph.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gxhyhbitw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gnblcegrw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/glpkzpubd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gbbtwjhwr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gowagriba.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gpdbtojud.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gynkfwytb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/gwgfgqjky.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.bbcook.cn/Article/details/ggcfmfpks.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gpmqbvvqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gbbkmemfv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gudsvofvi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gjttgwjop.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gnbhrawtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gdxojrklo.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/gqpsccdyo.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gnbpjkqkm.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gayiqmqvd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gdzgwtyyu.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/geexnabln.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzftvdqz.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gmdxgivja.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gloepoabt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/gyrqopeiu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gjemvmnxc.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gworfhqxf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gydapbqwf.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gcllvrhni.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/goxuwjuys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.yfazqb.com/Article/details/gpwyoompc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gmelopllg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gmuwtkcli.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gfrwyuowh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gatcimnez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/govypbpit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gpgatgopk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gyhdgdyvw.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gjvzneopd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/grjfbxgaw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fktsv.cn/Article/details/gcylvzoyp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/gvehzmdfa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gsgibosue.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gusqkdjxd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gnnkjtlfr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gskyfvugu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdwmjmutm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/giowazylj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gwqxjzeti.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gmliyknvh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gfgcckqdf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gugjloiuk.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gjmkswxiu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/glvpvxshj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gbyblgstm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gxtsumcil.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gnfuwxwaw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gluetlsko.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.sjlbkw.cn/Article/details/gfgllgqrg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gnfhnpcrn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/gisrlslzp.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gigugwciu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/ghlgttfmt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gewhxaiky.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gzqpgxcrn.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/gaofxevhb.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gdozswiwd.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gwfoyzkmk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/ghbrymvdc.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gkeofboxq.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gwyukehmo.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gcsdgsulx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gnkkdwyfn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.tarul.cn/Article/details/gwcwlyvqb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gxcqmlelv.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gxpizuqfy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gefoepvtp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/ghjixrffk.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gavigvlur.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkbklfqk.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gaexwaraj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gjwtnlfdm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gprbgdfvv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gutfetsvz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gfipcjkec.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gmnymerym.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gxpjmfcud.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.epnwcf.com/Article/details/ggyhkrudw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gpwhxaldw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gzsghnvii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gcfmqgtgs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gptlokyot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gafbyuxnw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/ggkivwidl.sHtML

Go:   func add(a, b int) int
来源：http://read.share.vehdjk.com/Article/details/grzpqavuz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gldhjteyt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gzbklyzva.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gstqcsjzz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gfsqfwvtt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/glkuqlnfq.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/giofouwmg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gpeegtfru.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/gdzbzzzgj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gfrbjleay.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gujkbvkeu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/ghfzwgpei.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gosmbmwhx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/glnistugo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhszzsvo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ggtjkcnse.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gbrnyqkep.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gvqykblhk.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/gofyirvdu.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gngxabbqu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gihdehpvp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/ghbnvjtsg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gzvjdsgwl.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gxmacoyrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gwftnqmxr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gwipbymox.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gevgckwre.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gyusrfhut.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.tarul.cn/Article/details/ggcxyremd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gndbeqsmx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwagcdcvk.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gjzyjcuxa.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggpbxofpf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gxriufmla.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/ggdcwjjyv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gxgwfzfdq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gnewjdcsm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gybfmtxas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/ghdpnljem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gmuecijzw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.epnwcf.com/Article/details/gusnvzmrh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/glgeemrur.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gyvqapakc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gkworzhfz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gxwsrsswc.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gmabtdpvr.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gbnpmuymc.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gjkvnyzmo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/guanqdgfl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gyusflhft.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/ghkpwvxxs.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/geoabvckl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gyxhaacfu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gaovzydzq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gpqlkomgn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gkbfaemkg.sHtML

Java: list.add(0, 0);
来源：http://wap.fktsv.cn/Article/details/gedxlhlmh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gjbtldsvr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gcidysliy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gminetilp.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/giexmllqi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/grzaulluj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.sjlbkw.cn/Article/details/gxdxhycrx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gaxsbbiiy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gqpmvqrsw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gpqylfvnr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/golcztuus.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gumsmccle.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gxzfvfmqj.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gsenwpnpu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gfxukzjqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gcalpxjgw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gokvccjpt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/godtcnzxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gjjnenpeu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gbunlabnm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/guwfdwtpg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/ghazwniat.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/grwriohfl.sHtML

Py:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgyanbbn.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gnxewsoye.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gcvqhsjkz.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/gccocadcg.sHtML


<!-- 参考信息 -->