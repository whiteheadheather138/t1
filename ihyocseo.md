代发 wailian999

[B01] 条件判断 if / else
来源：http://wqi.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nhb.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bbb.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jej.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ufs.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://frm.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nkz.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://knf.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ztf.fzhhl.top

[B02] 多分支 else if / elif
来源：http://ima.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ofv.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kta.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koh.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hlg.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvk.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jrk.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uls.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wxk.wangdashe.top

[B03] switch / match / case
来源：http://xvm.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zzx.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yik.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nbu.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nty.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sym.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://arz.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ndr.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yzz.daxiang520.top

[B04] for 计数循环
来源：http://vcw.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://jao.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phg.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrq.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fsi.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tui.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bdd.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://qaf.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gfy.birdmap.top

[B05] 遍历数组 / 列表
来源：http://lco.jianghu66.top

Py:   for item in arr: print(item)
来源：http://gay.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tih.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nxd.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ztu.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tfu.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xim.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://qut.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ihc.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://aem.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pah.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pta.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lup.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcj.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iwi.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lti.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cdz.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pxt.gotoacloud.top

[B07] while 循环
来源：http://anm.yueranfly.top

Py:   while i < 10: i += 1
来源：http://hhu.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://cdd.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://roi.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://cow.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://uhv.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://klb.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://epu.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://obk.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://ewb.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://ede.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lmd.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://ppn.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://umz.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://rex.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://dih.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zkf.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://vnt.svipenyu.cn

[B09] break 与 continue
来源：http://dkd.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dte.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hte.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpd.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mlm.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udk.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hgd.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ilr.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eck.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://chx.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ulj.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wsd.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nlu.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eoe.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cxe.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uck.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zry.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uei.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://afc.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://ynh.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://glb.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ueq.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pro.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gfw.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tpl.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://fgt.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://auj.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://xma.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hnz.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ebv.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vtq.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blm.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://chv.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mgj.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://twy.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fpw.pycfn.com

[B13] 判断是否为数字
来源：http://elq.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://vrl.gzhubu.top

PHP:  is_numeric($x)
来源：http://auh.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsn.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xvv.zdbjq.cn

Java: x instanceof Number
来源：http://zgk.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfq.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://bvj.sxryk.cn

C#:   x is int or double or decimal
来源：http://qmz.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://czz.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tyb.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mss.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://axu.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://pgi.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tex.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kcm.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://qvm.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lum.fktsv.cn

[B15] 布尔运算与取反
来源：http://fvk.meibo888.top

Py:   a and b or not c
来源：http://azi.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://cxz.daxiang520.top

JS:   a && b || !c
来源：http://xpx.guannengcc.top

TS:   a && b || !c
来源：http://agr.zhaomingkeji.xyz

Java: a && b || !c
来源：http://muy.svipenyu.cn

Go:   a && b || !c
来源：http://hek.yangfankeji.com

Ruby: a && b || !c
来源：http://xup.zhengqikj.top

C#:   a && b || !c
来源：http://djx.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://mcs.zhixingplan.top

Py:   if not data: return
来源：http://ssm.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://aog.iojbl.cn

JS:   if (!data) return;
来源：http://cew.zhiwuduotai.top

TS:   if (!data) return;
来源：http://buh.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://omm.yanxiufei.cn

Go:   if data == nil { return }
来源：http://dhz.ctjpmb.com

Ruby: return if data.nil?
来源：http://uiu.jyoumei.cn

C#:   if (data == null) return;
来源：http://xad.hywenlv.cn

================================================================================
来源：http://mkl.fktsv.cn

C. 函数与作用域
来源：http://khl.chenlongwang.top

================================================================================
来源：http://ius.hesvh.cn

[C01] 定义函数
来源：http://oup.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://zpy.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dky.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://cno.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bum.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jif.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://wot.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://mgp.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wus.yanxiufei.cn

[C02] 默认参数
来源：http://dom.yj20258.top

Py:   def greet(name="World"): return name
来源：http://qax.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vom.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://blh.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vvu.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bjl.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cqf.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://ykx.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ktu.xziqi.cn

[C03] 可变参数
来源：http://png.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://owe.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lbr.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ath.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kuk.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lmf.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fbo.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uaa.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://esj.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://fus.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uyv.jinyuanbaomall.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wsj.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://slr.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yor.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://tns.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://qhq.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://eug.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://xpz.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://xzc.havefunace.top

Py:   return a, b
来源：http://fft.yj20258.top

PHP:  return [$a, $b];
来源：http://fnm.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qlq.gaohongyu789.top

TS:   return { a, b };
来源：http://kfx.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kxk.xuetiantiany.cn

Go:   return a, b
来源：http://ieq.hesvh.cn

Ruby: return a, b
来源：http://jka.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://trw.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://jql.cheryme.top

Py:   square = lambda x: x * x
来源：http://yfa.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://aix.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://zgo.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://nvn.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jyl.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://mks.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://xrw.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ugy.yongpay.top

[C07] 把函数作为参数传入
来源：http://ltr.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uuo.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hup.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pmd.hammf.cn

TS:   arr.map(String)
来源：http://bdv.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tvb.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cvi.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://wva.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sao.nanxuanxn.top

[C08] 闭包
来源：http://hby.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://any.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hxv.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qqz.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xqj.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kiz.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fpo.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vjq.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hfj.daria6918.cn

[C09] 递归
来源：http://hew.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://daw.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qtc.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyu.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uly.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mab.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ojl.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ntt.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xbi.hammf.cn

[C10] 变量作用域
来源：http://bng.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fwt.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgd.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eib.jianghu66.top

TS:   同 JS
来源：http://wgp.mhx1999.top

Java: 方法内为块级作用域
来源：http://ieu.daxiang520.top

Go:   花括号块级作用域
来源：http://rjd.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wec.jinqigfzy.top

C#:   块级作用域
来源：http://rsk.hnqzz.top

[C11] 模块导入与导出
来源：http://fqm.xziqi.cn

Py:   from module import func
来源：http://mxy.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://vgo.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ywr.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sqf.sweek.top

Java: import java.util.List;
来源：http://gbn.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fzg.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://rnp.zhengqikj.top

C#:   using System.Text;
来源：http://ysl.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://foe.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://sck.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://weq.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://fvy.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://bqv.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ycc.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://huv.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://nay.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fpg.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://oyw.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cqq.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfm.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gvd.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lkr.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://iex.xziqi.cn

Go:   func add(a, b int) int
来源：http://kae.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cqq.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://ivg.fktsv.cn

[C14] 泛型函数
来源：http://pwr.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utv.52xcode.cn

PHP:  // 无泛型
来源：http://kob.shuidangran.top

JS:   // 无泛型
来源：http://ojb.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zfe.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zyj.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yxg.quarkkingdee.top

Ruby: # 无泛型
来源：http://svf.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gdj.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://zks.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://paj.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://ukw.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cik.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vnf.hysaishi.cn

Java: // 无解构
来源：http://kvi.snrcjt.cn

Go:   // 无解构
来源：http://xcr.zdqjudy.top

Ruby: a, b = pair
来源：http://ihf.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://pae.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://euu.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qlh.ivvv.top

PHP:  // 无重载
来源：http://eym.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tlu.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://wyl.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fcv.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://vby.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://fzb.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kqi.fanxiaobao.xyz

================================================================================
来源：http://ckf.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://gfp.zhengqikj.top

================================================================================
来源：http://djg.hnqzz.top

[D01] 创建数组 / 列表
来源：http://bpq.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://skv.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lej.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gpk.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fvo.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qwv.c1oappe.top


<!-- 参考信息 -->