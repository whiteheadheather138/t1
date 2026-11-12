代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wmu.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://pjk.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pea.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uuv.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zyw.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blo.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvu.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aos.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://smg.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzb.cucudq.cn

[B03] switch / match / case
来源：http://mqs.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hoi.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kfh.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xva.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xqk.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aoz.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xml.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xsq.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://odn.pycfn.com

[B04] for 计数循环
来源：http://uwt.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://kxc.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hmd.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xci.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mgv.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iwo.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lwo.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://vht.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hcb.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://jmi.gzhubu.top

Py:   for item in arr: print(item)
来源：http://uis.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rbm.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aps.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://jpe.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://slg.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ffv.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://ocf.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lam.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://dxe.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://azz.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jkf.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kos.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cla.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jis.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yys.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vlb.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hea.yj20258888.top

[B07] while 循环
来源：http://djk.xuanzx.com

Py:   while i < 10: i += 1
来源：http://qaw.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://yud.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://zfk.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://ivh.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://vcl.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eyp.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://hjd.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://jgt.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://xyb.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://jlo.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://luy.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://itq.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://wlv.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://csc.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lus.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ayu.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://nsl.yuanzhike.top

[B09] break 与 continue
来源：http://wcf.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dts.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dxw.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slo.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icc.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jde.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rwz.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oun.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zea.fzhhl.top

[B10] 遍历同时拿索引
来源：http://twt.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dee.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://olq.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eys.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aaq.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://suh.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jys.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bcg.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcb.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://rrr.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://eng.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://ust.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwh.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jql.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kbk.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bgc.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://zzv.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://znz.nwbrower.top

[B12] 跳出多层循环
来源：http://vdu.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vwb.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kcp.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://the.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxq.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kmy.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bng.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nwy.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mdt.0kj1m.cn

[B13] 判断是否为数字
来源：http://cyg.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://bzw.snrcjt.cn

PHP:  is_numeric($x)
来源：http://sri.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hgr.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://beh.dianchejie.cn

Java: x instanceof Number
来源：http://gcg.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yma.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://nqf.hesvh.cn

C#:   x is int or double or decimal
来源：http://pkw.cucudq.cn

[B14] 判断值是否在集合内
来源：http://mso.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://euv.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jvm.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://pqq.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://wto.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pij.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kqa.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://lmq.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tiv.aibaodan.cn

[B15] 布尔运算与取反
来源：http://yhy.yvedp.cn

Py:   a and b or not c
来源：http://ojj.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://adb.hysaishi.cn

JS:   a && b || !c
来源：http://uxc.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://tiv.iojbl.cn

Java: a && b || !c
来源：http://drw.sjlbkw.cn

Go:   a && b || !c
来源：http://lpx.tianlin.xyz

Ruby: a && b || !c
来源：http://ekg.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://dqt.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://qco.wangdashe.top

Py:   if not data: return
来源：http://plu.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://yza.yvedp.cn

JS:   if (!data) return;
来源：http://agx.hongshengwenyu.top

TS:   if (!data) return;
来源：http://bru.c1oappe.top

Java: if (data == null) return;
来源：http://gur.dianchejie.cn

Go:   if data == nil { return }
来源：http://mux.hnqzz.top

Ruby: return if data.nil?
来源：http://crb.ehwqpu.com

C#:   if (data == null) return;
来源：http://xfd.yvedp.cn

================================================================================
来源：http://vab.guowangkeji.top

C. 函数与作用域
来源：http://gps.smart0.xyz

================================================================================
来源：http://klw.hywenlv.cn

[C01] 定义函数
来源：http://xcw.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://ucn.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpr.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://pnn.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qip.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yjd.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iul.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://pbc.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hhd.jinyuanbaomall.cn

[C02] 默认参数
来源：http://dyi.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://wxl.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gxr.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://zkc.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://alb.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cvx.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zxf.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://qbz.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://cjb.dashuyun.cn

[C03] 可变参数
来源：http://jay.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://mes.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jvu.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://idj.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xav.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lgj.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sab.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uzw.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vwy.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://fhy.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ghx.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pqo.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tgs.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yhu.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://dki.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://lcv.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://mci.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://cil.chenjidiqi.icu

[C05] 返回多个值
来源：http://iml.tian-w.cn

Py:   return a, b
来源：http://usk.cheryme.top

PHP:  return [$a, $b];
来源：http://xlr.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bwb.aibaodan.cn

TS:   return { a, b };
来源：http://xuu.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtn.vqdsnc.cn

Go:   return a, b
来源：http://xet.zhaomingkeji.xyz

Ruby: return a, b
来源：http://onm.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://soc.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://gjf.tarul.cn

Py:   square = lambda x: x * x
来源：http://qai.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hsy.zdbjq.cn

JS:   const square = x => x * x;
来源：http://tnb.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://aoo.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zsu.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ibn.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://fjp.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://akb.yonumen.top

[C07] 把函数作为参数传入
来源：http://vpm.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nqt.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://xaw.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ezy.hysaishi.cn

TS:   arr.map(String)
来源：http://rlj.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vgo.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qcp.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://iym.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fzb.dianchejie.cn

[C08] 闭包
来源：http://pvc.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lvk.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hjw.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nde.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uzd.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://frd.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wqq.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mqu.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dav.zhiwuduotai.top

[C09] 递归
来源：http://btr.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mme.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://siu.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqh.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zso.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://amk.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hbf.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wyx.zycfv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wrx.andypj.xyz

[C10] 变量作用域
来源：http://bcn.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://poo.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uqb.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://voq.jlsjyb.cn

TS:   同 JS
来源：http://uag.316326.xyz

Java: 方法内为块级作用域
来源：http://dyz.316326.xyz

Go:   花括号块级作用域
来源：http://wnh.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lnf.jinghuilouyu.cn

C#:   块级作用域
来源：http://qww.gaohongyu789.top

[C11] 模块导入与导出
来源：http://gbl.snrcjt.cn

Py:   from module import func
来源：http://xue.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jwt.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjt.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nln.yueranfly.top

Java: import java.util.List;
来源：http://vdh.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xhz.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://hxi.meibo888.top

C#:   using System.Text;
来源：http://zsy.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://uxh.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://fis.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://qej.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://lwv.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://mnx.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vdp.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://hlb.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://iqr.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pre.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://gwn.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pne.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcg.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rqn.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://veg.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://fvc.havefunace.top

Go:   func add(a, b int) int
来源：http://zmh.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ceg.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://gqa.shuidangran.top

[C14] 泛型函数
来源：http://ami.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://otq.zhengqikj.top

PHP:  // 无泛型
来源：http://evq.jlsjyb.cn

JS:   // 无泛型
来源：http://swm.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zlr.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kco.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvt.fzhhl.top

Ruby: # 无泛型
来源：http://qlx.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dzg.ybcxt.top

[C15] 解构 / 展开参数
来源：http://eak.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://whm.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://ppz.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jtq.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kbb.yueranfly.top

Java: // 无解构
来源：http://zln.zdbjq.cn

Go:   // 无解构
来源：http://kvk.pycfn.com

Ruby: a, b = pair
来源：http://ceo.meibo888.top

C#:   var (a, b) = pair;
来源：http://fyh.bjfxy.top

[C16] 函数 / 方法重载
来源：http://qcy.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://otr.epnwcf.com

PHP:  // 无重载
来源：http://oor.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ceb.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://uai.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fli.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://yrt.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://dks.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://kkh.shanyushiyangtech.top

================================================================================
来源：http://tgw.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://tal.gaohongyu789.top

================================================================================
来源：http://xyv.hammf.cn

[D01] 创建数组 / 列表
来源：http://eyl.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ynm.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rar.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cus.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gsr.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ucw.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://pfd.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://oow.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bnd.tian-w.cn

[D02] 追加元素到末尾
来源：http://kuc.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://akk.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uto.haohaochexian.top

JS:   arr.push(4);
来源：http://gee.hcnkem.com

TS:   arr.push(4);
来源：http://rum.epnwcf.com


<!-- 参考信息 -->