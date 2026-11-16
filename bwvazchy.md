代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sxa.0kj1m.cn

================================================================================
来源：http://wra.xuetiantiany.cn

B. 流程控制
来源：http://rni.ppjwa.cn

================================================================================
来源：http://jsu.zhixingplan.top

[B01] 条件判断 if / else
来源：http://jui.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://inf.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rib.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iuo.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fdw.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ujq.xylfe.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wiq.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sbf.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vmd.wangdashe.top

[B02] 多分支 else if / elif
来源：http://oxz.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cuf.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hzy.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cww.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqx.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hlw.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kwe.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tfk.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzu.bbcook.cn

[B03] switch / match / case
来源：http://fae.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://flh.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fig.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yqk.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spn.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mld.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oog.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ibe.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kfd.fengsongda.top

[B04] for 计数循环
来源：http://ewe.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://zui.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oii.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://npq.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cex.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gik.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sgg.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://nzf.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gjj.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://yiq.c1oappe.top

Py:   for item in arr: print(item)
来源：http://tag.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wan.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zxt.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://prg.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tfw.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://myo.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://cqp.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vst.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://dxo.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ljj.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zvz.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vby.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yrt.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://atp.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yfp.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hok.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rbr.quarkkingdee.top

[B07] while 循环
来源：http://jcv.zycfv.cn

Py:   while i < 10: i += 1
来源：http://bmo.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uef.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://glh.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://iae.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://bvr.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kkl.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://jfn.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://jnf.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://nds.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://rjw.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jir.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://xrh.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://hzz.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://dee.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hkt.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://xbu.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://pdj.sweek.top

[B09] break 与 continue
来源：http://tkg.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://okr.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jun.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssx.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcn.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzk.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ipe.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://msi.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izj.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://naf.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nij.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dre.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nnn.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://upj.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ubx.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dqo.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjl.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pnr.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://ygd.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://ilc.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://leo.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qod.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jwi.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lcj.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://skx.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://wbf.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sli.aibaodan.cn

[B12] 跳出多层循环
来源：http://njv.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jex.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqn.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kep.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cgy.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://roi.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqo.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vum.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mtq.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://mvp.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://nwg.vehdjk.com

PHP:  is_numeric($x)
来源：http://pcz.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdp.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlw.zhongyouzk.top

Java: x instanceof Number
来源：http://ugb.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ndv.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://ixx.cqqwz.cn

C#:   x is int or double or decimal
来源：http://luh.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://zqy.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://emy.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hyt.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://rxq.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://oad.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zxt.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lqy.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jny.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cye.gotoacloud.top

[B15] 布尔运算与取反
来源：http://vaf.jiagoushi.top

Py:   a and b or not c
来源：http://ssc.mhx1999.top

PHP:  $a && $b || !$c
来源：http://ayn.wangshuangyany.cn

JS:   a && b || !c
来源：http://col.daria6918.cn

TS:   a && b || !c
来源：http://dqe.ydzc1.top

Java: a && b || !c
来源：http://iei.gzhubu.top

Go:   a && b || !c
来源：http://cuf.iojbl.cn

Ruby: a && b || !c
来源：http://xso.epnwcf.com

C#:   a && b || !c
来源：http://vsj.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://czy.ehwqpu.com

Py:   if not data: return
来源：http://hio.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://qog.ehwqpu.com

JS:   if (!data) return;
来源：http://ips.jinqigfzy.top

TS:   if (!data) return;
来源：http://uns.yfazqb.com

Java: if (data == null) return;
来源：http://umg.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://knh.yongpay.top

Ruby: return if data.nil?
来源：http://dft.xziqi.cn

C#:   if (data == null) return;
来源：http://jnq.shzxlz.cn

================================================================================
来源：http://eut.hywenlv.cn

C. 函数与作用域
来源：http://rww.yj202588.top

================================================================================
来源：http://nir.zhiwuduotai.top

[C01] 定义函数
来源：http://egs.cashguo.top

Py:   def add(a, b): return a + b
来源：http://vro.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wtq.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://dwr.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yxd.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xve.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://zuh.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://xdp.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dgp.tanke756.top

[C02] 默认参数
来源：http://vgf.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://qrv.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lzk.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://gfj.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gaf.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wsb.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://als.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://yzx.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://ifg.cucudq.cn

[C03] 可变参数
来源：http://zdp.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://nof.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wbf.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xts.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdq.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jar.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gqb.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://nlh.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hro.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://gtq.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://azy.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lll.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pcx.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://veq.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://jyv.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://azo.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://nlh.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://ldv.havefunace.top

[C05] 返回多个值
来源：http://ebz.zhijiandao.cn

Py:   return a, b
来源：http://jks.yuxming.cn

PHP:  return [$a, $b];
来源：http://jup.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zcl.bjfxy.top

TS:   return { a, b };
来源：http://nve.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sqc.meibo888.top

Go:   return a, b
来源：http://tle.jianghu66.top

Ruby: return a, b
来源：http://kln.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://yab.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://exl.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://wmm.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yds.dianchejie.cn

JS:   const square = x => x * x;
来源：http://efv.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://efh.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baf.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://vsn.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://rlo.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://afv.hnqzz.top

[C07] 把函数作为参数传入
来源：http://jay.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kqm.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://edk.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pwe.jinqigfzy.top

TS:   arr.map(String)
来源：http://hgq.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://llo.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qie.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://ipw.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jju.yanxiufei.cn

[C08] 闭包
来源：http://lma.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rrw.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ioc.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uim.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kgq.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hcy.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gme.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://git.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kbu.bjfxy.top

[C09] 递归
来源：http://nai.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://owf.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://evm.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqq.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvu.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kcm.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gme.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tjn.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dni.jqgufenzy.top

[C10] 变量作用域
来源：http://tet.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dwu.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://shu.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vur.52xcode.cn

TS:   同 JS
来源：http://rhb.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://ozb.sjlbkw.cn

Go:   花括号块级作用域
来源：http://wxs.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wre.zhongyouzk.top

C#:   块级作用域
来源：http://evg.jiagoushi.top

[C11] 模块导入与导出
来源：http://ilw.xylfe.cn

Py:   from module import func
来源：http://fqk.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sbs.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zbi.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hwh.ybcxt.top

Java: import java.util.List;
来源：http://nkl.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://irr.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://xlo.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://prg.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://ykp.316326.xyz

Py:   (lambda: print("run"))()
来源：http://afv.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://ubm.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://teo.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://dcq.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://auh.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://nxt.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://skg.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gee.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://jqf.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nln.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mvt.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ykk.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fnd.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://iso.hcnkem.com

Go:   func add(a, b int) int
来源：http://qdv.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dge.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://xkl.yanxiufei.cn

[C14] 泛型函数
来源：http://lkm.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://snc.gaohongyu789.top

PHP:  // 无泛型
来源：http://bew.hcnkem.com

JS:   // 无泛型
来源：http://jnw.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://llp.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eyi.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vdz.gogol.net.cn

Ruby: # 无泛型
来源：http://zkc.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tyd.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://qql.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rnn.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://vjz.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vkm.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://akv.zycfv.cn

Java: // 无解构
来源：http://vzp.jianghu66.top

Go:   // 无解构
来源：http://uec.jlsjyb.cn

Ruby: a, b = pair
来源：http://ffp.316326.xyz

C#:   var (a, b) = pair;
来源：http://qsj.tanke756.top

[C16] 函数 / 方法重载
来源：http://uch.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzc.vehdjk.com

PHP:  // 无重载
来源：http://khf.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hel.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://xsj.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xgx.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://mpq.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://qkj.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hoi.cashguo.top

================================================================================
来源：http://gml.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://ljg.zdqjudy.top

================================================================================
来源：http://yoa.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://dvm.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://urx.feifeiyinyue.top


<!-- 参考信息 -->