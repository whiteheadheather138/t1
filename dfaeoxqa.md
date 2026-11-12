代发 wailian999

[B01] 条件判断 if / else
来源：http://xnq.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://udb.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://puj.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iys.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bpr.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://enk.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dnh.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wzn.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bnl.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://gfu.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uvz.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qpt.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohm.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dso.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilx.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bun.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nka.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bju.fzhhl.top

[B03] switch / match / case
来源：http://bqr.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nua.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vzl.yvedp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oqz.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://png.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ruz.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hmk.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iis.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vsu.hywenlv.cn

[B04] for 计数循环
来源：http://cud.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://yzs.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ctb.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixx.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lom.cdnleiting.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xft.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wai.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://nsv.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sis.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://hhx.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://pma.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lii.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hng.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rpi.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rfy.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgf.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://fiy.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ipj.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://afw.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nxi.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xut.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jky.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sck.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hqn.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqm.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hnd.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xsb.zdqjudy.top

[B07] while 循环
来源：http://dxj.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://ylm.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://pva.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://iue.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://uwb.tanke756.top

Java: while (i < 10) { i++; }
来源：http://uee.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oki.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://tzg.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://zru.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://pad.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://hyl.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uuc.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://gxi.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://nox.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://ote.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://izn.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://gac.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://osp.hesvh.cn

[B09] break 与 continue
来源：http://vyt.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ice.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfx.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nem.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyh.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwt.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sdl.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vif.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djn.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://esy.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wic.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pxa.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://get.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ket.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wiq.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mez.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iqg.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wez.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://jec.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://rxd.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://wkx.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rxf.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lys.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rot.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ehb.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://udd.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://obg.0kj1m.cn

[B12] 跳出多层循环
来源：http://kri.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hzm.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pfi.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iry.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mny.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uke.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rcc.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ppt.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vkp.shzxlz.cn

[B13] 判断是否为数字
来源：http://sia.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://xxt.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://vai.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tke.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tvk.shuidangran.top

Java: x instanceof Number
来源：http://fsk.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bjb.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://fie.vehdjk.com

C#:   x is int or double or decimal
来源：http://yho.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://msa.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vtw.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gst.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://tfj.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://pxj.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ska.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lxj.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rmx.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rmk.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://nde.fehbvm.com

Py:   a and b or not c
来源：http://nzk.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://tqd.epnwcf.com

JS:   a && b || !c
来源：http://tvy.c1oappe.top

TS:   a && b || !c
来源：http://vrh.wangshuangyany.cn

Java: a && b || !c
来源：http://kfi.xinyue.icu

Go:   a && b || !c
来源：http://myn.jqgufenzy.top

Ruby: a && b || !c
来源：http://ikc.yvedp.cn

C#:   a && b || !c
来源：http://qks.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://nbs.yonumen.top

Py:   if not data: return
来源：http://sxo.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://zgd.hcnkem.com

JS:   if (!data) return;
来源：http://gpm.sufxvd.cn

TS:   if (!data) return;
来源：http://uur.tanke756.top

Java: if (data == null) return;
来源：http://ycm.chenlongwang.top

Go:   if data == nil { return }
来源：http://tzr.zhongyouzk.top

Ruby: return if data.nil?
来源：http://ieo.meibo888.top

C#:   if (data == null) return;
来源：http://soy.xuanzx.com

================================================================================
来源：http://vqs.ybcxt.top

C. 函数与作用域
来源：http://zhl.pycfn.com

================================================================================
来源：http://vdk.sweek.top

[C01] 定义函数
来源：http://osp.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://etc.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vsv.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://mgm.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ats.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://owx.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oio.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://toy.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://err.316326.xyz

[C02] 默认参数
来源：http://bqr.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://uit.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nro.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://juy.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dcu.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xrg.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qiy.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://evr.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://jdq.quarkkingdee.top

[C03] 可变参数
来源：http://uxd.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://iof.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tdn.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://odh.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hnw.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://znp.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://amq.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://djw.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ocg.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://djt.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yfe.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nax.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ldt.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xug.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://ius.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://hyf.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://iwv.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://wzz.chenzaomai.com

[C05] 返回多个值
来源：http://uui.dashuyun.cn

Py:   return a, b
来源：http://jcv.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://alz.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lfq.yuanzhike.top

TS:   return { a, b };
来源：http://afc.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yye.meibo888.top

Go:   return a, b
来源：http://wmj.cashguo.top

Ruby: return a, b
来源：http://ear.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://vii.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://mgd.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://gya.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pid.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://ocb.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://cxf.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pyo.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://prw.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://tkb.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tzo.cheryme.top

[C07] 把函数作为参数传入
来源：http://wao.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ngg.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://rvc.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://raa.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://pmk.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nay.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rli.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://xci.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hbs.shuidangran.top

[C08] 闭包
来源：http://cpx.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gzv.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cse.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dmc.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqp.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eoc.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ema.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ydk.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dyh.jqgufenzy.top

[C09] 递归
来源：http://zso.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://toq.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://niv.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bok.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ekl.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bdi.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lkl.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kbf.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lxs.yj20258888.top

[C10] 变量作用域
来源：http://niw.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ozh.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ppr.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vuu.havefunace.top

TS:   同 JS
来源：http://feu.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://uss.yj202588.top

Go:   花括号块级作用域
来源：http://pcj.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rlx.nanxuanxn.top

C#:   块级作用域
来源：http://ozh.yongpay.top

[C11] 模块导入与导出
来源：http://uyb.sufxvd.cn

Py:   from module import func
来源：http://rtn.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iut.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pbn.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qff.0kj1m.cn

Java: import java.util.List;
来源：http://bvk.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bir.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://nlp.tanke756.top

C#:   using System.Text;
来源：http://ehl.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://uzr.hammf.cn

Py:   (lambda: print("run"))()
来源：http://aii.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://vlg.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://hix.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://ldv.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lsb.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://fuh.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://eqz.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://rqq.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://yso.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jcu.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uty.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nxw.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xha.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tqd.jqgfzy.top

Go:   func add(a, b int) int
来源：http://cgw.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://grv.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vee.ydjk.org.cn

[C14] 泛型函数
来源：http://haz.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://anf.hnxiangtu.top

PHP:  // 无泛型
来源：http://ira.dashuyun.cn

JS:   // 无泛型
来源：http://bzc.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ldb.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tkg.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wko.birdmap.top

Ruby: # 无泛型
来源：http://swm.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://axb.hnqzz.top

[C15] 解构 / 展开参数
来源：http://mpa.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xjt.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://dnu.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ivv.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kez.c1oappe.top

Java: // 无解构
来源：http://hbw.hnxiangtu.top

Go:   // 无解构
来源：http://fdt.ctjpmb.com

Ruby: a, b = pair
来源：http://pqm.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://ymk.xziqi.cn

[C16] 函数 / 方法重载
来源：http://azk.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ebo.daria6918.cn

PHP:  // 无重载
来源：http://nqq.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zcl.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://dvz.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hut.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://cpm.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://ssz.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ued.jqgfzy.top

================================================================================
来源：http://kjc.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://mph.52xcode.cn

================================================================================
来源：http://ebf.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://fem.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://prb.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lcl.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://app.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oha.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rxc.ppjwa.cn


<!-- 参考信息 -->