代发 wailian999

[B01] 条件判断 if / else
来源：http://yln.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://llm.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nnb.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lxa.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mre.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cye.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zig.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cgf.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lwa.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://dqu.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qzs.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uob.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vkr.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bev.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sax.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pkg.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xrk.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkq.zhengqikj.top

[B03] switch / match / case
来源：http://qky.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ces.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://spq.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yza.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gpu.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nxx.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://smm.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nmf.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wwc.yj20258.top

[B04] for 计数循环
来源：http://yqq.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://nwy.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ygl.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfg.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dxl.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://poc.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://awk.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://goj.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wif.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://vuf.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://umk.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tag.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jpz.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hyw.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dlg.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://azv.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://hky.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://agf.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://fhq.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gjl.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://txi.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqx.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fkk.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zrq.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wel.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ltl.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xaz.vqdsnc.cn

[B07] while 循环
来源：http://uce.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://ojn.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://aon.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://onb.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://eat.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://itx.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lry.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://yge.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://qrz.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://tom.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://vvn.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gvt.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://zxt.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://qqk.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://qpt.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jhg.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://vui.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://tbs.hnqzz.top

[B09] break 与 continue
来源：http://bic.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgy.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wcq.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hph.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wez.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vmt.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vtd.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pvg.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fka.xziqi.cn

[B10] 遍历同时拿索引
来源：http://kdd.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rnr.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://phe.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dfu.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wmp.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrf.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uzj.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://byc.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bwd.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://eha.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://hyt.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://ihb.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://seq.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epx.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtl.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://spv.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://gcr.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eim.fktsv.cn

[B12] 跳出多层循环
来源：http://diq.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://khi.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vdr.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kxc.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://apk.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jvd.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xoo.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yjo.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cvk.havefunace.top

[B13] 判断是否为数字
来源：http://gmc.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://mue.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://wnu.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://duc.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://llc.52xcode.cn

Java: x instanceof Number
来源：http://gdq.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zog.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://hsu.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://fan.c1oappe.top

[B14] 判断值是否在集合内
来源：http://oda.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gdb.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ptm.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://gwz.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://qyj.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ddz.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xva.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cex.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xur.sxryk.cn

[B15] 布尔运算与取反
来源：http://tpt.hesvh.cn

Py:   a and b or not c
来源：http://jmv.yj20258888.top

PHP:  $a && $b || !$c
来源：http://yfg.yj20258888.top

JS:   a && b || !c
来源：http://rka.chenjidiqi.icu

TS:   a && b || !c
来源：http://pla.zdqjudy.top

Java: a && b || !c
来源：http://hlv.tanke756.top

Go:   a && b || !c
来源：http://qdf.zhongyouzk.top

Ruby: a && b || !c
来源：http://plk.52xcode.cn

C#:   a && b || !c
来源：http://sew.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uok.andypj.xyz

Py:   if not data: return
来源：http://rbw.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://skh.chenlongwang.top

JS:   if (!data) return;
来源：http://ana.hysaishi.cn

TS:   if (!data) return;
来源：http://jym.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://vvx.xziqi.cn

Go:   if data == nil { return }
来源：http://oej.quarkkingdee.top

Ruby: return if data.nil?
来源：http://riz.yfazqb.com

C#:   if (data == null) return;
来源：http://xbi.iojbl.cn

================================================================================
来源：http://dsq.mhx1999.top

C. 函数与作用域
来源：http://yqv.bbcook.cn

================================================================================
来源：http://nop.yvedp.cn

[C01] 定义函数
来源：http://sow.meibo888.top

Py:   def add(a, b): return a + b
来源：http://cpi.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xos.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://vmy.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gkh.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gqk.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://neh.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://cjd.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nnm.chenlongwang.top

[C02] 默认参数
来源：http://pan.uphjek.com

Py:   def greet(name="World"): return name
来源：http://jzg.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dia.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://jhi.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ggg.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dxp.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tug.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://psv.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://yvc.bbcook.cn

[C03] 可变参数
来源：http://giy.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://rqk.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eom.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozf.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yrf.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bmi.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aza.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://hov.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nqn.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://prv.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hqr.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pzi.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ryo.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wqw.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://zff.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://rnx.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://ugs.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://wud.jiagoushi.top

[C05] 返回多个值
来源：http://qci.ivvv.top

Py:   return a, b
来源：http://xfu.andypj.xyz

PHP:  return [$a, $b];
来源：http://vba.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qpg.wangdashe.top

TS:   return { a, b };
来源：http://ctp.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xqa.quarkkingdee.top

Go:   return a, b
来源：http://dqt.cdnleiting.top

Ruby: return a, b
来源：http://wuo.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://wad.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://bpm.yj202588.top

Py:   square = lambda x: x * x
来源：http://qlw.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fxv.uphjek.com

JS:   const square = x => x * x;
来源：http://kcd.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://usr.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qni.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://xyw.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://yyg.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ywd.vehdjk.com

[C07] 把函数作为参数传入
来源：http://rdm.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpa.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://vqf.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oad.sweek.top

TS:   arr.map(String)
来源：http://hcd.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jas.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sdy.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://sml.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vzc.yangfankeji.com

[C08] 闭包
来源：http://swb.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vej.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zil.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mmk.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://weu.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rrf.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://duj.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cjf.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://roa.nwbrower.top

[C09] 递归
来源：http://kjl.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mfb.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oli.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://czp.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://thw.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qkk.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wza.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qic.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qgc.vqdsnc.cn

[C10] 变量作用域
来源：http://pdw.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qza.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vxt.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qnv.xuanzx.com

TS:   同 JS
来源：http://gqk.shzxlz.cn

Java: 方法内为块级作用域
来源：http://hrz.sufxvd.cn

Go:   花括号块级作用域
来源：http://pjs.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cnq.sxryk.cn

C#:   块级作用域
来源：http://mnn.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://eiz.nanxinkj.top

Py:   from module import func
来源：http://iui.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uia.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xar.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kau.cucudq.cn

Java: import java.util.List;
来源：http://rbk.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xve.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jtt.jqgfzy.top

C#:   using System.Text;
来源：http://oxq.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://khl.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://kfa.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://nwq.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://xol.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://gnq.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wor.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://shx.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://vjx.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kia.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://kpu.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uht.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://psu.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kqd.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hze.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://izk.tian-w.cn

Go:   func add(a, b int) int
来源：http://vho.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgs.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pak.hcnkem.com

[C14] 泛型函数
来源：http://kqm.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cfb.havefunace.top

PHP:  // 无泛型
来源：http://sep.bjfxy.top

JS:   // 无泛型
来源：http://nvl.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://utx.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hct.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bsz.wangdashe.top

Ruby: # 无泛型
来源：http://whi.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nkz.sysykeji.top

[C15] 解构 / 展开参数
来源：http://ppd.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yhp.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://nky.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xdm.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hjs.tarul.cn

Java: // 无解构
来源：http://uae.0kj1m.cn

Go:   // 无解构
来源：http://rbg.zdqjudy.top

Ruby: a, b = pair
来源：http://poy.yonumen.top

C#:   var (a, b) = pair;
来源：http://feu.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://snu.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blb.jinqigfzy.top

PHP:  // 无重载
来源：http://ohp.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wtm.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://xra.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gbe.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://wzl.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://mvl.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oac.sweek.top

================================================================================
来源：http://jaa.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://tsz.hcnkem.com

================================================================================
来源：http://doj.xylfe.cn

[D01] 创建数组 / 列表
来源：http://cqd.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xnn.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oxw.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wui.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://acp.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jqw.shanyushiyangtech.top


<!-- 参考信息 -->