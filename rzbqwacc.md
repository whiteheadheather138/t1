代发 wailian999

[B01] 条件判断 if / else
来源：http://ihl.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gas.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wiu.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ljf.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ctv.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://yvg.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uyj.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fnp.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mhl.cashguo.top

[B02] 多分支 else if / elif
来源：http://nik.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kzt.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://abf.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eoa.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxu.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txi.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tpr.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bet.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwb.yj20258888.top

[B03] switch / match / case
来源：http://cbh.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fce.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vda.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jtt.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xyo.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ifn.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://haz.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lrh.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bpn.sysykeji.top

[B04] for 计数循环
来源：http://vxw.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://rur.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qun.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nen.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqz.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://chp.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vwi.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://qfw.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vit.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://pbs.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://imm.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aax.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xsw.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iam.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yll.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zyy.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://iil.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://crj.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://ksi.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zrt.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bzj.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zll.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xfs.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://agc.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mqd.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pqs.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwk.sweek.top

[B07] while 循环
来源：http://jgh.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://tdr.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jyf.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://eqz.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://ows.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://dmx.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://loy.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://kgo.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://xik.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://euo.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://twe.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oon.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://bmb.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://mmf.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://zyl.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://fkl.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://kom.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://sry.yongpay.top

[B09] break 与 continue
来源：http://uij.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rju.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sgn.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbp.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgj.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iaj.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zup.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://orj.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwb.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://akx.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ncg.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hvl.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ghp.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rie.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://juw.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mda.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jpw.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://olm.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://bpf.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://roo.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://ike.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mzm.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rwb.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://thb.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://okr.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://plc.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mlc.aibaodan.cn

[B12] 跳出多层循环
来源：http://efo.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cix.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iva.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lve.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhp.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jhk.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aav.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vjt.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qgf.iojbl.cn

[B13] 判断是否为数字
来源：http://ffy.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://cxd.meibo888.top

PHP:  is_numeric($x)
来源：http://kpy.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvm.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://viy.shzxlz.cn

Java: x instanceof Number
来源：http://vru.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qvy.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://kvu.svipenyu.cn

C#:   x is int or double or decimal
来源：http://nam.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://cbu.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vxi.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bir.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://hko.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://ymy.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jtg.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xkk.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uys.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kmq.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://mea.hongshengwenyu.top

Py:   a and b or not c
来源：http://yjw.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://lvy.jianghu66.top

JS:   a && b || !c
来源：http://myi.zhengqikj.top

TS:   a && b || !c
来源：http://vch.birdmap.top

Java: a && b || !c
来源：http://pog.316326.xyz

Go:   a && b || !c
来源：http://hey.pengpengdd.cyou

Ruby: a && b || !c
来源：http://anh.hnxiangtu.top

C#:   a && b || !c
来源：http://nmi.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://iqk.wangdashe.top

Py:   if not data: return
来源：http://oti.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://hnm.jqgufenzy.top

JS:   if (!data) return;
来源：http://iou.zycfv.cn

TS:   if (!data) return;
来源：http://edf.xinyue.icu

Java: if (data == null) return;
来源：http://wuf.xylfe.cn

Go:   if data == nil { return }
来源：http://umi.daria6918.cn

Ruby: return if data.nil?
来源：http://ouf.cdnleiting.top

C#:   if (data == null) return;
来源：http://tae.52xcode.cn

================================================================================
来源：http://ymx.fanxiaobao.xyz

C. 函数与作用域
来源：http://kwd.dashuyun.cn

================================================================================
来源：http://tho.ctjpmb.com

[C01] 定义函数
来源：http://vah.yj20258.top

Py:   def add(a, b): return a + b
来源：http://mkz.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dip.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://sht.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fes.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ylo.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://tur.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://hjf.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpc.chenzaomai.com

[C02] 默认参数
来源：http://xeo.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://nyw.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zav.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://ymj.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://opg.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xvs.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tum.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://cjy.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://cdt.zdbjq.cn

[C03] 可变参数
来源：http://vut.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://myr.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vpu.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fpj.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqi.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hra.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://etd.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ibm.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xli.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://zml.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nau.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://frw.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bbk.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ipy.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://rmt.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://xhs.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://kqv.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://klu.wangdashe.top

[C05] 返回多个值
来源：http://iyv.zhengqikj.top

Py:   return a, b
来源：http://vuy.hysaishi.cn

PHP:  return [$a, $b];
来源：http://lae.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://kro.jlsjyb.cn

TS:   return { a, b };
来源：http://lgx.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oyr.quarkkingdee.top

Go:   return a, b
来源：http://sas.xuetiantiany.cn

Ruby: return a, b
来源：http://tnx.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://xvo.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://dzh.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://upu.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://flm.cucudq.cn

JS:   const square = x => x * x;
来源：http://lcw.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://tvi.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sqe.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fnm.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://odu.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://rlj.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://bda.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jie.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://gyb.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hzv.cdnleiting.top

TS:   arr.map(String)
来源：http://zji.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rsm.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ylm.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://qyz.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bvx.dianchejie.cn

[C08] 闭包
来源：http://dls.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sem.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypt.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vgp.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ddh.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dfs.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://taf.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jjo.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etg.vqdsnc.cn

[C09] 递归
来源：http://jvb.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lqe.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pla.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://but.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jjq.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yvf.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oat.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://acc.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gmf.yuanzhike.top

[C10] 变量作用域
来源：http://etb.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iie.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qes.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nwe.cheryme.top

TS:   同 JS
来源：http://lzm.cqqwz.cn

Java: 方法内为块级作用域
来源：http://sgw.svipenyu.cn

Go:   花括号块级作用域
来源：http://qwp.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vtf.hywenlv.cn

C#:   块级作用域
来源：http://kjw.fehbvm.com

[C11] 模块导入与导出
来源：http://dcl.xingfuxueyuan.xyz

Py:   from module import func
来源：http://sli.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://noy.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qwv.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yfv.bjfxy.top

Java: import java.util.List;
来源：http://azb.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dea.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://sdi.zhongyouzk.top

C#:   using System.Text;
来源：http://aua.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://fiw.uphjek.com

Py:   (lambda: print("run"))()
来源：http://xgx.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://sfg.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://hmn.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://ccj.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sqi.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://gis.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://ibb.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://myt.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://twu.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://btw.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnv.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kqu.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjz.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://otq.cheryme.top

Go:   func add(a, b int) int
来源：http://lxa.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gqr.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wwg.jqgufenzy.top

[C14] 泛型函数
来源：http://cop.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gqf.yfazqb.com

PHP:  // 无泛型
来源：http://nzx.sysykeji.top

JS:   // 无泛型
来源：http://dxm.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lyb.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ntu.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://idz.jinqigfzy.top

Ruby: # 无泛型
来源：http://aol.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eaa.hnqzz.top

[C15] 解构 / 展开参数
来源：http://ppq.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eqz.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://bef.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sml.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://myf.tian-w.cn

Java: // 无解构
来源：http://qrz.tianlin.xyz

Go:   // 无解构
来源：http://ube.zhoulong.xyz

Ruby: a, b = pair
来源：http://ict.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://jnd.daxiang520.top

[C16] 函数 / 方法重载
来源：http://vjw.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zlj.bjfxy.top

PHP:  // 无重载
来源：http://zxk.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://qkl.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://fpt.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qua.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://wvy.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://bcz.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kdj.vqdsnc.cn

================================================================================
来源：http://iww.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://ocs.epnwcf.com

================================================================================
来源：http://gnt.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://dpp.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hzx.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kkq.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vim.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://iva.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hhz.meibo888.top


<!-- 参考信息 -->