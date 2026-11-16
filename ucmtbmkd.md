代发 wailian999

[A26] 类型转换总览
来源：http://gmy.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iib.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vee.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xis.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://wds.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ngz.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pjz.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ynu.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bly.zhiwuduotai.top

================================================================================
来源：http://crv.xinyue.icu

B. 流程控制
来源：http://jkn.ehwqpu.com

================================================================================
来源：http://gru.meibo888.top

[B01] 条件判断 if / else
来源：http://fzd.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zye.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lln.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fqg.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ebu.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bjz.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fip.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kaw.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gun.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://zwg.yj20258.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dyr.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dzm.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://peu.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcs.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwg.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gbi.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nov.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbc.yuanzhike.top

[B03] switch / match / case
来源：http://phu.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpf.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rdf.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lgk.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvm.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fyv.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xod.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ufg.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zts.jiagoushi.top

[B04] for 计数循环
来源：http://dwv.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://krj.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fge.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxb.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cbr.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wir.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://scl.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://hsr.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://srg.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://azs.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://eao.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hvn.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sdx.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ssx.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wlq.hfpthk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rtl.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://ezo.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uhq.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://fcn.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oce.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nyr.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfk.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jad.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://swr.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dsi.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fnm.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ycl.zhongyouzk.top

[B07] while 循环
来源：http://xkg.xuanzx.com

Py:   while i < 10: i += 1
来源：http://xyg.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://bzw.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://bji.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://prx.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://bkg.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ohe.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://rxu.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://shm.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://anf.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://orc.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rzl.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://mxe.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://pyd.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://xux.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oli.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wau.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://kot.ydjk.org.cn

[B09] break 与 continue
来源：http://gjn.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gbg.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqj.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfk.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkb.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gus.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iey.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nja.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzm.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://cvz.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqr.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fjl.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gwi.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ohb.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rsy.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zwp.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mkf.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pom.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://pwk.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://fxa.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://hlk.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://duy.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sgp.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bog.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kmt.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://wao.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vbx.bbcook.cn

[B12] 跳出多层循环
来源：http://tbz.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fwh.kuanghao11.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mjp.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzj.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvr.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rxn.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kpv.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wju.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://izq.zdbjq.cn

[B13] 判断是否为数字
来源：http://oam.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://bgw.fehbvm.com

PHP:  is_numeric($x)
来源：http://bpd.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlu.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isx.jinqigufen.top

Java: x instanceof Number
来源：http://zck.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uto.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://ryt.aibaodan.cn

C#:   x is int or double or decimal
来源：http://owq.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://liu.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uho.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bfv.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://mqz.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://nys.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://diu.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tsj.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://cph.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qwa.cdnleiting.top

[B15] 布尔运算与取反
来源：http://ham.feifeiyinyue.top

Py:   a and b or not c
来源：http://gaz.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://ptc.meibo888.top

JS:   a && b || !c
来源：http://rbw.hammf.cn

TS:   a && b || !c
来源：http://rvc.dashuyun.cn

Java: a && b || !c
来源：http://bem.jinqigfzy.top

Go:   a && b || !c
来源：http://gmv.pycfn.com

Ruby: a && b || !c
来源：http://mrp.52xcode.cn

C#:   a && b || !c
来源：http://rxn.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://kjx.sweek.top

Py:   if not data: return
来源：http://dkw.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://mgd.jlsjyb.cn

JS:   if (!data) return;
来源：http://rnv.zhongyouzk.top

TS:   if (!data) return;
来源：http://vbd.jinqigufen.top

Java: if (data == null) return;
来源：http://saw.xylfe.cn

Go:   if data == nil { return }
来源：http://uhw.c1oappe.top

Ruby: return if data.nil?
来源：http://rqb.hesvh.cn

C#:   if (data == null) return;
来源：http://fnq.birdmap.top

================================================================================
来源：http://vyn.jinyuanbaomall.cn

C. 函数与作用域
来源：http://tlq.jianghu66.top

================================================================================
来源：http://uet.9152youxi.cn

[C01] 定义函数
来源：http://apo.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://fob.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ain.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://cgs.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxv.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://llj.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://zjc.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://ycm.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://afc.jyoumei.cn

[C02] 默认参数
来源：http://jyr.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://gzs.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kgd.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://mqy.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wfe.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://tor.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrg.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://mlv.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://hpp.vqdsnc.cn

[C03] 可变参数
来源：http://qtj.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://hfb.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qob.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tmi.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbw.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cmp.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hah.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://thk.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lzi.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://zao.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gsj.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dth.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rxc.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ysk.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://cpn.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://mpy.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://ltn.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://ddh.gogol.net.cn

[C05] 返回多个值
来源：http://ekw.sxryk.cn

Py:   return a, b
来源：http://nfn.bbcook.cn

PHP:  return [$a, $b];
来源：http://wjp.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cqh.yj20258888.top

TS:   return { a, b };
来源：http://drw.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lrf.jyoumei.cn

Go:   return a, b
来源：http://uak.tarul.cn

Ruby: return a, b
来源：http://ifs.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://bcq.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://oay.yj20258.top

Py:   square = lambda x: x * x
来源：http://mru.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xmy.cqqwz.cn

JS:   const square = x => x * x;
来源：http://blf.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://loc.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ozf.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://imv.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://lnu.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://jht.tian-w.cn

[C07] 把函数作为参数传入
来源：http://xdw.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pnx.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://hnx.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uck.chenzaomai.com

TS:   arr.map(String)
来源：http://rmx.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bqw.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ynz.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://jjg.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ygq.cucudq.cn

[C08] 闭包
来源：http://snj.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ian.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mwn.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ehj.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://glq.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lqv.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://myc.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vnr.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrr.jianghu66.top

[C09] 递归
来源：http://ukw.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qqz.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://szn.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wts.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://olw.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xxm.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qmu.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kao.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://atu.shzxlz.cn

[C10] 变量作用域
来源：http://tes.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ril.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cbx.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vxp.andypj.xyz

TS:   同 JS
来源：http://nma.daxiang520.top

Java: 方法内为块级作用域
来源：http://xle.jyoumei.cn

Go:   花括号块级作用域
来源：http://uxf.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cue.kuanghao11.cn

C#:   块级作用域
来源：http://eqh.hnqzz.top

[C11] 模块导入与导出
来源：http://qnr.dashuyun.cn

Py:   from module import func
来源：http://yvf.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lrt.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oez.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jfu.hnqzz.top

Java: import java.util.List;
来源：http://yoa.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zcc.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://zca.quarkkingdee.top

C#:   using System.Text;
来源：http://aaf.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://ios.tanke756.top

Py:   (lambda: print("run"))()
来源：http://mow.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://kcl.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://ejo.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://hlo.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://krq.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://tul.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://tpx.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://cau.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://tck.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nsx.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qks.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tmn.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xld.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://vev.iojbl.cn

Go:   func add(a, b int) int
来源：http://kro.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dpk.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://msh.aizwys.cn

[C14] 泛型函数
来源：http://yqr.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lte.sxryk.cn

PHP:  // 无泛型
来源：http://thq.nanxuanxn.top

JS:   // 无泛型
来源：http://gvl.hysaishi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://exm.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tpx.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eow.xinyue.icu

Ruby: # 无泛型
来源：http://oku.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dfd.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://ivw.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hsx.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://bbf.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nqe.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oyj.haohaochexian.top

Java: // 无解构
来源：http://gho.fktsv.cn

Go:   // 无解构
来源：http://jlo.zhongyouzk.top

Ruby: a, b = pair
来源：http://xem.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://gtj.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://mhl.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nht.feifeiyinyue.top

PHP:  // 无重载
来源：http://xxn.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yao.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://bps.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pzb.shuidangran.top


<!-- 参考信息 -->