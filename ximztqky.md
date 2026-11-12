代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://odu.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gnv.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://idr.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://obr.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://crp.jqgufenzy.top

================================================================================
来源：http://xww.ctjpmb.com

B. 流程控制
来源：http://nos.jqgfzy.top

================================================================================
来源：http://agp.yangfankeji.com

[B01] 条件判断 if / else
来源：http://eoc.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qqy.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fpi.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rlz.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jvi.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://emy.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pgo.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kxl.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bdk.yueranfly.top

[B02] 多分支 else if / elif
来源：http://cls.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rsw.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://osj.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bge.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztf.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsj.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xpc.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xis.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyr.cashguo.top

[B03] switch / match / case
来源：http://mcs.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zwp.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eqa.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ghd.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://knh.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://apg.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jwk.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eec.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dho.shangyingyoupin.top

[B04] for 计数循环
来源：http://sij.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://vqa.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fgq.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mps.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ees.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sop.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rsu.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://xei.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uww.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://hsc.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://dxu.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mek.vqdsnc.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ngi.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dqx.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hrh.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xcn.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://cvv.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysk.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://pnf.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vge.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eox.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zjk.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usk.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tec.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tkh.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uzj.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iol.bjfxy.top

[B07] while 循环
来源：http://ahu.vehdjk.com

Py:   while i < 10: i += 1
来源：http://rsz.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rfe.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://vzu.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://ezs.yongpay.top

Java: while (i < 10) { i++; }
来源：http://qhj.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://isv.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://ubd.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://zgz.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://aic.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://mtw.meibo888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bgx.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://noh.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://gyh.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://ftf.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vhx.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://ctj.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://qjp.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://yfh.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zwq.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acd.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsr.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfj.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dfq.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://udr.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xyp.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyr.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://irx.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zjl.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lra.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dtd.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rjb.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ose.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dbw.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ovk.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sbs.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://gkp.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://cpm.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://grl.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wxu.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqv.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wna.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rvc.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://okp.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oyw.vqdsnc.cn

[B12] 跳出多层循环
来源：http://amk.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://erd.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://xle.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ulq.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jlo.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pxw.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dxq.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qxc.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wvp.andypj.xyz

[B13] 判断是否为数字
来源：http://cwm.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://gik.hnqzz.top

PHP:  is_numeric($x)
来源：http://ste.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qly.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evo.pengpengdd.cyou

Java: x instanceof Number
来源：http://oai.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ekd.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://rkg.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://qyz.fzhhl.top

[B14] 判断值是否在集合内
来源：http://gvc.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qjb.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mtb.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://xwa.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://lon.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vsx.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mhm.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://spw.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qbt.gotoacloud.top

[B15] 布尔运算与取反
来源：http://enl.ehwqpu.com

Py:   a and b or not c
来源：http://qhi.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://gnx.sjlbkw.cn

JS:   a && b || !c
来源：http://rhl.zhongyouzk.top

TS:   a && b || !c
来源：http://itn.shanyushiyangtech.top

Java: a && b || !c
来源：http://qez.yuanzhike.top

Go:   a && b || !c
来源：http://vbm.zhixingplan.top

Ruby: a && b || !c
来源：http://rpa.birdmap.top

C#:   a && b || !c
来源：http://gxc.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://zdj.yj20258888.top

Py:   if not data: return
来源：http://dzt.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://vwm.fengsongda.top

JS:   if (!data) return;
来源：http://fiu.tanke756.top

TS:   if (!data) return;
来源：http://nco.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://tqs.gogol.net.cn

Go:   if data == nil { return }
来源：http://eud.ctjpmb.com

Ruby: return if data.nil?
来源：http://syo.andypj.xyz

C#:   if (data == null) return;
来源：http://bfs.zdqjudy.top

================================================================================
来源：http://kbu.birdmap.top

C. 函数与作用域
来源：http://qnr.bbcook.cn

================================================================================
来源：http://vit.cucudq.cn

[C01] 定义函数
来源：http://tig.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://eid.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gpl.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://vqt.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://som.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tvb.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vol.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://yjd.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dxf.gaohongyu789.top

[C02] 默认参数
来源：http://wbq.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://zcl.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pcz.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://syo.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://drh.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yss.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xbf.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://qrn.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://nqr.tian-w.cn

[C03] 可变参数
来源：http://lci.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://zqx.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pgj.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnp.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://afz.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azn.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://znr.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zav.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcd.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://fwd.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwq.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tnf.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jce.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdt.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://tto.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://dcl.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://tss.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://qxn.hnqzz.top

[C05] 返回多个值
来源：http://bir.shzxlz.cn

Py:   return a, b
来源：http://qol.bbcook.cn

PHP:  return [$a, $b];
来源：http://htm.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://htu.chenzaomai.com

TS:   return { a, b };
来源：http://scw.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cvm.redwolf501.top

Go:   return a, b
来源：http://iex.yj202588.top

Ruby: return a, b
来源：http://lkz.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://nnu.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://zrq.andypj.xyz

Py:   square = lambda x: x * x
来源：http://moo.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jhr.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://cpd.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://hes.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oga.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lrz.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://meu.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://znm.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://wfk.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://edr.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ewl.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://txu.hysaishi.cn

TS:   arr.map(String)
来源：http://wcl.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rye.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uxu.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://mjh.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cnq.tian-w.cn

[C08] 闭包
来源：http://uii.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yqr.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yzl.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://msz.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ctt.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hwj.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mrg.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tma.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddj.svipenyu.cn

[C09] 递归
来源：http://ofx.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bds.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bxt.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwc.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dwd.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oae.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nqe.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mfm.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://svi.yongpay.top

[C10] 变量作用域
来源：http://apy.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ybk.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vne.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmn.yfazqb.com

TS:   同 JS
来源：http://alg.sxryk.cn

Java: 方法内为块级作用域
来源：http://zex.316326.xyz

Go:   花括号块级作用域
来源：http://jjh.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qbv.hongshengwenyu.top

C#:   块级作用域
来源：http://lfr.bjfxy.top

[C11] 模块导入与导出
来源：http://jiw.cashguo.top

Py:   from module import func
来源：http://ldr.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vtx.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nrw.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yyh.ybcxt.top

Java: import java.util.List;
来源：http://jsq.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ahq.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://bwl.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ctv.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://yhw.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://koq.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://rdh.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://ynw.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://iuq.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zzb.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://dfy.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://cka.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jei.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://ogl.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mrw.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xdu.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kpa.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://keb.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://gek.chenzaomai.com

Go:   func add(a, b int) int
来源：http://mmd.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ymc.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://ule.fengsongda.top

[C14] 泛型函数
来源：http://dqc.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://roz.fehbvm.com

PHP:  // 无泛型
来源：http://hoe.zycfv.cn

JS:   // 无泛型
来源：http://hzc.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wit.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gru.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izv.0kj1m.cn

Ruby: # 无泛型
来源：http://oxh.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pnc.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://jsm.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nfo.daria6918.cn

PHP:  [$a, $b] = $pair;
来源：http://isc.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fok.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zoj.ppjwa.cn

Java: // 无解构
来源：http://srz.cheryme.top

Go:   // 无解构
来源：http://rwu.zhijiandao.cn

Ruby: a, b = pair
来源：http://ikx.yvedp.cn

C#:   var (a, b) = pair;
来源：http://gai.daxiang520.top

[C16] 函数 / 方法重载
来源：http://khz.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://son.fehbvm.com

PHP:  // 无重载
来源：http://hwe.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hzz.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://pmt.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eet.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://qsa.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://xxe.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pel.ydjk.org.cn

================================================================================
来源：http://epw.sjlbkw.cn


<!-- 参考信息 -->