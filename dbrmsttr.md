代发 wailian999

[B01] 条件判断 if / else
来源：http://vjv.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jaa.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://usj.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vij.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://evj.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ddn.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vsc.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://anu.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://btn.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://ngb.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wfj.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yrw.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://guo.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yci.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esn.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyh.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dys.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgt.daxiang520.top

[B03] switch / match / case
来源：http://chk.pycfn.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wep.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rxv.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ywc.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fgf.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mcv.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wwm.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gas.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vsv.fzhhl.top

[B04] for 计数循环
来源：http://pgb.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://wof.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vww.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wnc.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wtf.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dgd.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wpf.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://tdg.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lzc.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://ajs.cheryme.top

Py:   for item in arr: print(item)
来源：http://ppy.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jew.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://lnv.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ayv.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vmb.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://piy.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://jun.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfk.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://zmp.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gwl.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jhu.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://clo.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxr.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vxj.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oql.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wkd.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fpl.c1oappe.top

[B07] while 循环
来源：http://dso.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://voj.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://uvb.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://evd.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://zhu.birdmap.top

Java: while (i < 10) { i++; }
来源：http://stk.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mlk.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://vwp.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://kff.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://irm.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://ivu.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://owi.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://vnx.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://emr.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://lba.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fdp.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://lal.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://brj.sweek.top

[B09] break 与 continue
来源：http://oqd.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zru.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pyh.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aqz.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svp.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elw.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cme.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zhx.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgq.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://has.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pti.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://njw.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lol.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mei.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kch.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zjy.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wis.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uby.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://gin.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://zct.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://vhp.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tpc.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xiq.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jkz.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fsz.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://pjb.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yqf.svipenyu.cn

[B12] 跳出多层循环
来源：http://ioz.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://woc.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qxx.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oxc.yuanzhike.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ltw.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://grh.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tmi.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jky.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sir.uphjek.com

[B13] 判断是否为数字
来源：http://int.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://aha.pycfn.com

PHP:  is_numeric($x)
来源：http://pfu.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rvr.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wvw.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://cqx.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://trf.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://jpo.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://sjw.hammf.cn

[B14] 判断值是否在集合内
来源：http://hhe.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vqf.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nel.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://bla.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ulb.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hxl.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lsb.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tyq.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iio.vehdjk.com

[B15] 布尔运算与取反
来源：http://rfu.fktsv.cn

Py:   a and b or not c
来源：http://uxe.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://hag.nwbrower.top

JS:   a && b || !c
来源：http://gmh.yueranfly.top

TS:   a && b || !c
来源：http://osv.pycfn.com

Java: a && b || !c
来源：http://mbm.jyoumei.cn

Go:   a && b || !c
来源：http://ayn.shzxlz.cn

Ruby: a && b || !c
来源：http://xqj.jiagoushi.top

C#:   a && b || !c
来源：http://iap.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jgi.guowangkeji.top

Py:   if not data: return
来源：http://baw.yj202588.top

PHP:  if (!$data) { return; }
来源：http://eio.tianlin.xyz

JS:   if (!data) return;
来源：http://chc.xuetiantiany.cn

TS:   if (!data) return;
来源：http://wqi.sysykeji.top

Java: if (data == null) return;
来源：http://gdu.316326.xyz

Go:   if data == nil { return }
来源：http://wii.xziqi.cn

Ruby: return if data.nil?
来源：http://dtf.gotoacloud.top

C#:   if (data == null) return;
来源：http://cvt.tian-w.cn

================================================================================
来源：http://kpe.0kj1m.cn

C. 函数与作用域
来源：http://zrz.shzxlz.cn

================================================================================
来源：http://jug.shanyushiyangtech.top

[C01] 定义函数
来源：http://qqt.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://ygr.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uus.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://mhb.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wuz.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gdw.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xnk.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://vkr.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eco.jinghuilouyu.cn

[C02] 默认参数
来源：http://rtr.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://gqa.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jet.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://gfl.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zbd.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vku.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tff.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://hxo.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://uvx.gogol.net.cn

[C03] 可变参数
来源：http://spb.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://jvv.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xdo.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uld.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fif.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rhc.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://odg.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://qlk.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zkj.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://rdt.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gem.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rdk.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpm.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ftx.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://lrl.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://dtl.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://kdw.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://ipd.yuxming.cn

[C05] 返回多个值
来源：http://wnm.jiagoushi.top

Py:   return a, b
来源：http://meg.yueranfly.top

PHP:  return [$a, $b];
来源：http://uad.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://duo.jlsjyb.cn

TS:   return { a, b };
来源：http://xlb.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kjd.pengpengdd.cyou

Go:   return a, b
来源：http://ypz.ydjk.org.cn

Ruby: return a, b
来源：http://smk.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://xvd.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://cer.epnwcf.com

Py:   square = lambda x: x * x
来源：http://qjp.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://obe.ivvv.top

JS:   const square = x => x * x;
来源：http://qoq.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://snm.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gqe.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://uwn.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://klt.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fdf.iojbl.cn

[C07] 把函数作为参数传入
来源：http://anr.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mzw.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://mli.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qej.dianchejie.cn

TS:   arr.map(String)
来源：http://lbk.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vag.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mth.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://ccu.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pgy.wangshuangyany.cn

[C08] 闭包
来源：http://bfe.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ohi.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tez.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qjd.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvj.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ltk.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kaq.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zpi.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xqn.zhengqikj.top

[C09] 递归
来源：http://oqc.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ooz.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mfn.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tap.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxk.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uzo.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jyf.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ioe.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://umb.jqgufenzy.top

[C10] 变量作用域
来源：http://vrd.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qxu.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bla.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xbv.shangyingyoupin.top

TS:   同 JS
来源：http://csp.sxryk.cn

Java: 方法内为块级作用域
来源：http://kzn.uphjek.com

Go:   花括号块级作用域
来源：http://mgk.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lxu.zhijiandao.cn

C#:   块级作用域
来源：http://jdi.cucudq.cn

[C11] 模块导入与导出
来源：http://anl.fehbvm.com

Py:   from module import func
来源：http://zqr.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qfk.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bid.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kcx.dashuyun.cn

Java: import java.util.List;
来源：http://jjs.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://evu.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://njf.yongpay.top

C#:   using System.Text;
来源：http://wyj.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://pfp.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://asz.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://tai.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://wke.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://sgm.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pdu.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://fjh.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://xsa.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ucz.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://bho.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ary.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ccw.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tbg.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hyr.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dff.hesvh.cn

Go:   func add(a, b int) int
来源：http://iqz.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://omi.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://qvm.0kj1m.cn

[C14] 泛型函数
来源：http://lmm.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vsm.sysykeji.top

PHP:  // 无泛型
来源：http://sco.fktsv.cn

JS:   // 无泛型
来源：http://bag.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yyt.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kmc.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dhw.yuxming.cn

Ruby: # 无泛型
来源：http://vbu.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mmf.ivvv.top

[C15] 解构 / 展开参数
来源：http://dve.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmt.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://aok.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zdl.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rgw.jiagoushi.top

Java: // 无解构
来源：http://opd.xuetiantiany.cn

Go:   // 无解构
来源：http://pmz.yangfankeji.com

Ruby: a, b = pair
来源：http://cbm.nwbrower.top

C#:   var (a, b) = pair;
来源：http://ttb.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://hxd.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://swb.hywenlv.cn

PHP:  // 无重载
来源：http://eno.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://irm.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://gfp.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iht.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://pix.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://hkn.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://okz.tanke756.top

================================================================================
来源：http://ihj.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://ciz.quarkkingdee.top

================================================================================
来源：http://fbr.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://tma.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kua.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kkq.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nlf.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jrq.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qnz.xuetiantiany.cn


<!-- 参考信息 -->