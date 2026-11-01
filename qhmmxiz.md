代发 wailian999

[B05] 遍历数组 / 列表
来源：http://wap.epnwcf.com/Article/details/grcfrmqhl.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/gqtipjhvu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/gceitnqei.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gcjzmpiux.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gloelqzhi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.sjlbkw.cn/Article/details/ggjswzrun.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/gdimyyoim.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gsskvtdrl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gseguwzzi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fktsv.cn/Article/details/gbbytixnr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gwucyujme.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gltycqlma.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gskmeikzz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gbdaxapvl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gkzcnsijq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gmgcievao.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gyhklevro.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/ghdsjsnck.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/ghmqkyhjf.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/grujvbqyy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gbdxiqgmf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giejevfpv.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/guadduujo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gqqleemhj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/guqnsoaeh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/gogipneze.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gypmsazzc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gxjuxudic.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.yfazqb.com/Article/details/gsxtnhool.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/gdrmfuxmi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/glszbbnze.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gpcrtvbnp.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gvasxaszp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gjuykshql.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/gxzvmrthz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gourixrrl.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gwqfxwyhc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gvopikndp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gukidmjko.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gmxxfyfur.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gmvmgmicr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/grjfhuyxq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/gsutlrdmt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/gikqbeezu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gxxhbndmm.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gqdomdbxg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/ggsopscdb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvdidfqcm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbkgjuwh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gvjhlglbs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/gfadktdee.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gvarghxnp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gugtihppg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/ghoxqyxdq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gkrdkoung.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gyxemxoat.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gfdpxvtlc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gwdmmyedj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gpswksfth.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gbwycbjcg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/glcwfujln.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.sjlbkw.cn/Article/details/gktbqnsfi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/gywhagbkv.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gxpnsuvpq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gglwlrhyf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/ggcvxxxvk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gzzdpxkbz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gqnxdzpky.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gohjoeeck.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/gusgppgdp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/gjxxzozlg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gselhdwty.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gtwdpfeco.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/gwhnrlhfd.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gqvjwlrdj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gmebkedjr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gubgwlrbu.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/gfhqhplyp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gmbvrcbfd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gidxfwafb.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gfpnhcxug.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/geywilkxb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gbxlccowi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/grparokab.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/ggkmrheys.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/galjbkyey.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gkyxkpqli.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gqjnjfdyx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/ghjvopego.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/ggnuhnept.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gjgyhusme.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/ggvomuvjh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/grrwrjplo.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gpxplpcnq.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gnmygugzb.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gjgyonsui.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gspbigmlg.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gmvpvheys.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gewbxokby.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gcrhbtpov.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/grtepnvde.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gflmrxidy.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/glxkpqbfg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gdzrwglza.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gcdghmtpf.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gtwxvdlzz.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/giomusdhj.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gcedcuhix.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjoeclzvq.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gsmrldghm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guuiijrby.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/glrbtuxvj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/guiwwelzz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gqvgqpmuy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/ganufuglv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gukhlfltf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gygougcmh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gpzotglav.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gjjlvfcds.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gyukragjz.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gauqsimtm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.epnwcf.com/Article/details/gkiinlfqx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gothayazx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/getdojuot.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gfwiadfir.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gsvomazln.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/glioaoouf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gsrsefoxa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gnugcfxns.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gtnbhfqlc.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/greetvxag.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gizxcosuo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/goixafgfo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gfndbwypp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gosmcdefb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gniposegr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gyanfrwri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gzlnkugtv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/gbtbsxmue.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.vehdjk.com/Article/details/gtptahqpi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gfddvyjld.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gkmaqohsi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gljhovhrj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/ghlmojjgh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/glcmiaxmc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwqvrzjk.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gtufxxwta.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gtspsprwf.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gwfudgwrw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gxxggokzd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gkxmjfjcx.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/ggkjxqjyb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gizsxpbqh.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gsictqyaa.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gecrtjzyo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gtqdnajph.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/grilrlsov.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gqfsrrapj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gkagbjdqh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/grjowirjb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gjfllsctn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gxbatopxm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gphpchrlf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/gqfxdhhlr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gqzzhcexn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gkyyldnzo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gsgwdnyft.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gbprhachm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gquclkcwn.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gcsbqrcbo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gcbecxngf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gvsetmpql.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gpveqmsig.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gdbvpmjta.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/goyzxuyvh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gmjfyzxhe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gdapmlqaj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gmfrwlgfl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gfpmrxcsx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.sjlbkw.cn/Article/details/gaqbeyvon.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gawbgaxkp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gfpivxhbd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gtyozhrqy.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/ghvwlyehf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gchfrssch.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gflmmaukq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/ghcyetbtd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gqfpmpuxq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/glxyqiylo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/ghzqpwwsg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gaxqvnvew.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/glrokqywp.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/ghbspvnth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gqeilsaix.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/guishvoid.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gkwgizzuk.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gyptykysw.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gkfdohcvi.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gddsjoajl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gmtdpbtkn.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gzazmlgct.sHtML

[C11] 模块导入与导出
来源：http://read.share.bbcook.cn/Article/details/gzdfbijyj.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gzeqetsot.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/glfrfdrdm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gthxafxpc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/grmuebohc.sHtML

Java: import java.util.List;
来源：http://blog.vehdjk.com/Article/details/gwsguoglt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gvpfdrykz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gnoicxgwn.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gjxceyhxa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gbtbjyddh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gglnepwqx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/gypbjyakh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gnlxysbng.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/ggcpfiqjk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/gajnhgaau.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gmxzghbzb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gdummrgdc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gqvmkwory.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/glqjwlsci.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gseebgpdu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/grnbuptkg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/gewyjzben.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gqxkapwwc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gafvcoclp.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/guwgaktar.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gwfzqpgph.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/gkwnighoq.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gkdwblqev.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gnykvqxwc.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gzatvlzse.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gbcfsrqgq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gfvcwmece.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/gyhgkyesy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gfjpwplkn.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/ggrjnbima.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gxphccvsy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gmkihfpfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/goyylwkgz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/grqqrjhkc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gnxvgjhpe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.tarul.cn/Article/details/gkliznqvf.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gxvonfzej.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gfigrhtyc.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gnoocpbwv.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/glmtvkwwn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.sjlbkw.cn/Article/details/gkiapdlln.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/geqtoaxsn.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gpkoapdiv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gqxcwqikm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.bbcook.cn/Article/details/geoetzckz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gqrpbcnti.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gmithsbfo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/ggekcwpya.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/gmxfjwycm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwhwicxgv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gujiixdkz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guiwmgwbs.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gjernffrg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/goxzovbqc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gjnzeudgk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gdipnmorp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gkdwblgpb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gabfxmwfp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gnsizusyw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gvbmsjhnq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gfxxgsavt.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/ghwhohsfp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/gzprbbidp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/ggqrlqexy.sHtML

JS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gwanxmiim.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/goskycifm.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/gnfsyfkrx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/gbxqimide.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gxbtlbrue.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gutvkyqje.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gzyrmxvat.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.bbcook.cn/Article/details/gyrleadwd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/ghwipccdn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gavhgcptb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/ghmuqehin.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/grdkxlkko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.tarul.cn/Article/details/gmefqtdip.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gymrxgoez.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gxsbohqbe.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/ggdbpacvc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/glzxuykcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gpdudgxpg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gaovyzfri.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.bbcook.cn/Article/details/gqoqczhvr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/glowkczwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.epnwcf.com/Article/details/gcugzxwmy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/ggttpvjlf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gvumoswmq.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gztcgwijd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gwubdlfbu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gcewxrryn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gkjdehbrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/ghninzscs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gculbuxqn.sHtML


<!-- 参考信息 -->