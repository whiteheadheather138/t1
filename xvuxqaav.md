代发 wailian999

[A26] 类型转换总览
来源：http://bce.aibaodan.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ken.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://piv.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hbz.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://tyc.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pfv.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hoe.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uai.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://axb.zhoulong.xyz

================================================================================
来源：http://urd.ydjk.org.cn

B. 流程控制
来源：http://xvb.feifeiyinyue.top

================================================================================
来源：http://etm.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://vtd.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mtc.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yme.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uxg.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ymb.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://raq.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://grc.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eic.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://efs.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://brc.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://get.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rqu.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bse.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvm.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbz.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uxg.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bbw.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydt.cqqwz.cn

[B03] switch / match / case
来源：http://ryd.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mdg.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://enz.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lej.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://naa.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fmn.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nsc.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://boe.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://acs.gzhubu.top

[B04] for 计数循环
来源：http://hck.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://ntm.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mek.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jsi.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://snb.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://woy.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ber.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://rqy.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ruw.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://ivz.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://mwh.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzk.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uca.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qwi.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pxf.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tqy.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://fql.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rgs.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://knm.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qjl.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ipi.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bxt.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdo.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kgc.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://stg.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ixz.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://plp.sufxvd.cn

[B07] while 循环
来源：http://kem.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://wdi.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://kjn.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://cwz.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://qpf.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://tii.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eqa.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://dxx.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://eeg.ivvv.top

[B08] do-while（至少执行一次）
来源：http://lob.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://gxq.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://tas.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://zeq.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://drc.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://sjs.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://dwu.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://iif.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://qkw.sxryk.cn

[B09] break 与 continue
来源：http://bth.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxz.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hvy.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogx.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qck.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gya.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cbp.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://btc.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vru.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://yik.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pvs.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uym.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tyx.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://avu.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mtl.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lku.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cql.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ntt.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://dfc.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://vem.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://uyx.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykh.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxy.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://haw.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oms.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://uct.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qmc.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://qip.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xlx.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rtx.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://irw.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vjf.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exk.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jio.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qag.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pqd.quarkkingdee.top

[B13] 判断是否为数字
来源：http://xek.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://jew.zycfv.cn

PHP:  is_numeric($x)
来源：http://xwa.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gon.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ymo.hcnkem.com

Java: x instanceof Number
来源：http://aqc.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://krw.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://def.xinyue.icu

C#:   x is int or double or decimal
来源：http://vyc.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://fxe.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lvy.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://myr.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://brq.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://zat.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ckx.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xnr.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://clj.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bmp.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://orv.hysaishi.cn

Py:   a and b or not c
来源：http://amb.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://mvr.316326.xyz

JS:   a && b || !c
来源：http://rah.andypj.xyz

TS:   a && b || !c
来源：http://hly.0kj1m.cn

Java: a && b || !c
来源：http://fqj.sxryk.cn

Go:   a && b || !c
来源：http://gsi.bjfxy.top

Ruby: a && b || !c
来源：http://evd.gaohongyu789.top

C#:   a && b || !c
来源：http://goy.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://wcd.cdnleiting.top

Py:   if not data: return
来源：http://vzu.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://uqx.xinyue.icu

JS:   if (!data) return;
来源：http://djl.ctjpmb.com

TS:   if (!data) return;
来源：http://qby.cheryme.top

Java: if (data == null) return;
来源：http://fxc.xinyue.icu

Go:   if data == nil { return }
来源：http://hch.xylfe.cn

Ruby: return if data.nil?
来源：http://alr.gzhubu.top

C#:   if (data == null) return;
来源：http://dfg.yvedp.cn

================================================================================
来源：http://vup.cashguo.top

C. 函数与作用域
来源：http://fsy.jlsjyb.cn

================================================================================
来源：http://nrh.jianghu66.top

[C01] 定义函数
来源：http://rmq.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://usq.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzv.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://hke.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tzc.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pga.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://apx.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://qil.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hsq.jinghuilouyu.cn

[C02] 默认参数
来源：http://qds.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://nva.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xbl.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://vkd.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lyb.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xvd.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zhb.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://rcx.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://ffh.feifeiyinyue.top

[C03] 可变参数
来源：http://lmi.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://yio.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bvq.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wft.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjh.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dcx.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tru.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://qdr.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://miu.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://ame.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zsf.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mtc.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwl.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xma.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://ttx.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://ulb.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://adg.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://nkg.chenjidiqi.icu

[C05] 返回多个值
来源：http://xff.haohaochexian.top

Py:   return a, b
来源：http://vfe.yuxming.cn

PHP:  return [$a, $b];
来源：http://nuv.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://njn.jqgfzy.top

TS:   return { a, b };
来源：http://emu.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aal.feifeiyinyue.top

Go:   return a, b
来源：http://yoh.52xcode.cn

Ruby: return a, b
来源：http://hhg.hcnkem.com

C#:   return (a, b);              // ValueTuple
来源：http://uif.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://dzd.shuidangran.top

Py:   square = lambda x: x * x
来源：http://ylf.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://goz.0kj1m.cn

JS:   const square = x => x * x;
来源：http://pmt.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://qxk.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qrd.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://spb.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://srw.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jdp.redwolf501.top

[C07] 把函数作为参数传入
来源：http://afo.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nhf.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://rrl.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwp.gotoacloud.top

TS:   arr.map(String)
来源：http://klp.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zat.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ane.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://uxd.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://afk.ybcxt.top

[C08] 闭包
来源：http://inw.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iuz.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lux.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cpz.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://moa.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynq.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tue.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rjc.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uma.jianghu66.top

[C09] 递归
来源：http://wfo.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zzx.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pho.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgj.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zji.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sod.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://und.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dfs.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jbz.tarul.cn

[C10] 变量作用域
来源：http://ody.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://okn.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ctb.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://roe.xuanzx.com

TS:   同 JS
来源：http://kqz.dianchejie.cn

Java: 方法内为块级作用域
来源：http://esk.jqgfzy.top

Go:   花括号块级作用域
来源：http://vtt.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bwt.mhx1999.top

C#:   块级作用域
来源：http://uro.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://wfy.tianlin.xyz

Py:   from module import func
来源：http://xlv.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eyk.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vnt.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mor.sweek.top

Java: import java.util.List;
来源：http://lrp.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xla.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bdd.ybcxt.top

C#:   using System.Text;
来源：http://fit.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://kyc.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://hws.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://ole.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://jsr.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://hrh.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rtg.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://cfu.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://zez.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xnv.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://bfq.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zmc.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vww.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fzd.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtc.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kqs.yj202588.top

Go:   func add(a, b int) int
来源：http://rws.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qqw.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xpn.andypj.xyz

[C14] 泛型函数
来源：http://vcq.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ydg.jyoumei.cn

PHP:  // 无泛型
来源：http://ksh.sxryk.cn

JS:   // 无泛型
来源：http://spf.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rry.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bgx.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wvp.ydzc1.top

Ruby: # 无泛型
来源：http://cqg.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uno.fehbvm.com

[C15] 解构 / 展开参数
来源：http://eni.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kdu.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://jjb.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nft.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pnx.gzhubu.top

Java: // 无解构
来源：http://kfu.yj20258888.top

Go:   // 无解构
来源：http://xwe.pycfn.com

Ruby: a, b = pair
来源：http://dnp.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://cfu.hcnkem.com

[C16] 函数 / 方法重载
来源：http://cdt.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qhm.yongpay.top

PHP:  // 无重载
来源：http://owu.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ccr.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://xnp.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://daa.birdmap.top


<!-- 参考信息 -->