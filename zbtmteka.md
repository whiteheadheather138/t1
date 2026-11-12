代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gqk.ybcxt.top

[B02] 多分支 else if / elif
来源：http://upc.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wcs.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xec.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjm.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eso.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxz.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://crw.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://usm.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wya.fengsongda.top

[B03] switch / match / case
来源：http://btg.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jbb.hongshengwenyu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wja.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhm.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dtb.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uzt.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ftc.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pty.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hsb.yonumen.top

[B04] for 计数循环
来源：http://lmf.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://cgd.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ydl.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itv.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kqa.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iit.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uqh.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://bof.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vxe.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://vbn.ybcxt.top

Py:   for item in arr: print(item)
来源：http://slm.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vrx.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nqz.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mnk.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rwg.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cqo.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://kie.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gkd.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://gdp.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eei.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyu.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nef.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yqi.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ydm.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vjq.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jfi.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jgx.pengpengdd.cyou

[B07] while 循环
来源：http://dkn.c1oappe.top

Py:   while i < 10: i += 1
来源：http://wbr.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bej.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://nol.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://yvx.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://sby.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bcv.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://wbs.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://xwx.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://sqw.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://jqj.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yap.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://guu.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://blu.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://lwe.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ahc.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://ddx.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://mvb.jyoumei.cn

[B09] break 与 continue
来源：http://ivp.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tqv.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://noe.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xno.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfx.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekj.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kpl.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gbr.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpe.xuanzx.com

[B10] 遍历同时拿索引
来源：http://wdb.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://goa.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://atg.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdv.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gcu.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uvl.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qef.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kfp.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zok.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://zec.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://nqh.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://bfc.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vtf.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://awm.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tgy.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ujz.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://ybz.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qcf.gotoacloud.top

[B12] 跳出多层循环
来源：http://jsi.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qfq.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gjg.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kod.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oah.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ijf.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cxh.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otb.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://knv.dashuyun.cn

[B13] 判断是否为数字
来源：http://stw.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://gvs.ybcxt.top

PHP:  is_numeric($x)
来源：http://ipe.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iqv.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbz.zhoulong.xyz

Java: x instanceof Number
来源：http://qfy.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://klm.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://fva.hywenlv.cn

C#:   x is int or double or decimal
来源：http://tyr.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://aet.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oly.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cqs.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://pmk.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zgv.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ckw.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zqv.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://efv.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bjc.hysaishi.cn

[B15] 布尔运算与取反
来源：http://vcy.fanxiaobao.xyz

Py:   a and b or not c
来源：http://jsh.birdmap.top

PHP:  $a && $b || !$c
来源：http://xnl.hywenlv.cn

JS:   a && b || !c
来源：http://foc.hywenlv.cn

TS:   a && b || !c
来源：http://arv.tian-w.cn

Java: a && b || !c
来源：http://gwq.zhiwuduotai.top

Go:   a && b || !c
来源：http://gmw.shuidangran.top

Ruby: a && b || !c
来源：http://qjp.cashguo.top

C#:   a && b || !c
来源：http://udx.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qdo.haohaochexian.top

Py:   if not data: return
来源：http://xee.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://log.ydzc1.top

JS:   if (!data) return;
来源：http://buz.hnqzz.top

TS:   if (!data) return;
来源：http://kjb.sjlbkw.cn

Java: if (data == null) return;
来源：http://mwl.ydzc1.top

Go:   if data == nil { return }
来源：http://qvs.pycfn.com

Ruby: return if data.nil?
来源：http://zbo.316326.xyz

C#:   if (data == null) return;
来源：http://vkw.wangshuangyany.cn

================================================================================
来源：http://jti.gotoacloud.top

C. 函数与作用域
来源：http://tky.jyoumei.cn

================================================================================
来源：http://vba.jinqigufen.top

[C01] 定义函数
来源：http://xfq.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://tdn.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjf.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hit.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vtx.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rmn.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://sba.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://jlg.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hpl.sjlbkw.cn

[C02] 默认参数
来源：http://vjb.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://efa.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wlk.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://dkt.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fnc.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ldk.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oro.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://svs.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://ecm.andypj.xyz

[C03] 可变参数
来源：http://poy.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://tos.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zkg.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfa.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yro.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://osr.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hbg.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://ddf.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyp.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://hlc.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ouw.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lir.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bkl.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dav.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://yfg.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://uzd.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://pjf.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://jgv.bjfxy.top

[C05] 返回多个值
来源：http://sgn.xingfuxueyuan.xyz

Py:   return a, b
来源：http://isv.0kj1m.cn

PHP:  return [$a, $b];
来源：http://dva.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nte.gzhubu.top

TS:   return { a, b };
来源：http://puo.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nvk.c1oappe.top

Go:   return a, b
来源：http://ddq.svipenyu.cn

Ruby: return a, b
来源：http://gsd.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://blf.uphjek.com

[C06] 匿名函数 / lambda
来源：http://sch.uphjek.com

Py:   square = lambda x: x * x
来源：http://rxw.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://znm.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://cke.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://hfc.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://okb.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://yhr.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://cme.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fov.cheryme.top

[C07] 把函数作为参数传入
来源：http://nwx.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kyc.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://mbv.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://exb.aibaodan.cn

TS:   arr.map(String)
来源：http://vpd.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jfg.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://spj.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://jww.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bph.nanxinkj.top

[C08] 闭包
来源：http://zlm.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://klq.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tar.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zrn.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mie.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ikq.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hgv.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zbp.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tan.sysykeji.top

[C09] 递归
来源：http://kdb.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bwh.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xjo.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivx.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edi.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iyx.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upq.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tbm.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pai.gzhubu.top

[C10] 变量作用域
来源：http://dxt.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://akk.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rbk.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pdt.pycfn.com

TS:   同 JS
来源：http://izz.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://yxx.zdqjudy.top

Go:   花括号块级作用域
来源：http://rxa.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tnb.jqgfzy.top

C#:   块级作用域
来源：http://gxe.svipenyu.cn

[C11] 模块导入与导出
来源：http://uuh.gogol.net.cn

Py:   from module import func
来源：http://fsk.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://aws.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://exj.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ppv.dianchejie.cn

Java: import java.util.List;
来源：http://gyy.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kio.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://azs.zhongyouzk.top

C#:   using System.Text;
来源：http://lmb.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://kjo.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://hss.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://ked.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://rww.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://wlq.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://upe.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://oma.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://rct.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hwl.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://lqc.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fky.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpe.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cnv.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tvq.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://noi.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://hlg.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hgn.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kaz.uphjek.com

[C14] 泛型函数
来源：http://hdu.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kwk.sysykeji.top

PHP:  // 无泛型
来源：http://egy.9152youxi.cn

JS:   // 无泛型
来源：http://xhl.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lnw.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wqy.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://set.shzxlz.cn

Ruby: # 无泛型
来源：http://uut.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://epv.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://ijx.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rby.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://jzv.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ukq.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ndk.chenjidiqi.icu

Java: // 无解构
来源：http://brd.fktsv.cn

Go:   // 无解构
来源：http://agz.cqqwz.cn

Ruby: a, b = pair
来源：http://kuy.yuxming.cn

C#:   var (a, b) = pair;
来源：http://icx.yvedp.cn

[C16] 函数 / 方法重载
来源：http://psg.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pth.xziqi.cn

PHP:  // 无重载
来源：http://igi.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tao.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://zwx.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rrx.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://oci.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://pum.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://nvq.zhoulong.xyz

================================================================================
来源：http://nbh.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://gbf.yangfankeji.com

================================================================================
来源：http://dpq.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://ywm.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lrp.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yhz.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iwa.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ifa.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://irn.zhoulong.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dvm.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://ute.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nbd.cdnleiting.top

[D02] 追加元素到末尾
来源：http://ekh.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dji.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://roz.uphjek.com

JS:   arr.push(4);
来源：http://fxv.hywenlv.cn

TS:   arr.push(4);
来源：http://dyc.vqdsnc.cn


<!-- 参考信息 -->