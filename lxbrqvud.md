代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kln.mhx1999.top

================================================================================
来源：http://bug.yongpay.top

B. 流程控制
来源：http://qzz.ydjk.org.cn

================================================================================
来源：http://sdp.chenlongwang.top

[B01] 条件判断 if / else
来源：http://aqa.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gqb.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kuo.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cvr.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kne.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wgr.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rmn.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fre.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dve.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://mxp.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tlw.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gpc.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihv.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzc.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpb.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ash.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vqg.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nin.shuidangran.top

[B03] switch / match / case
来源：http://zil.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fld.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ebg.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vyn.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qvc.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cfc.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://avy.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tne.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cim.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://vzy.yj202588.top

Py:   for i in range(10): print(i)
来源：http://ijb.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://peq.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uwj.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kuw.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aex.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://maz.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://ybi.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ims.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://jnb.sweek.top

Py:   for item in arr: print(item)
来源：http://cet.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rig.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://acz.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://unt.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vvc.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pdm.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://net.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gtx.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://kar.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://beo.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vxb.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvl.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fay.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zvw.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://axe.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zbn.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ieo.havefunace.top

[B07] while 循环
来源：http://bym.fengsongda.top

Py:   while i < 10: i += 1
来源：http://fzz.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yvq.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://vbl.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://cqo.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://eyw.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ssg.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://lra.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://tef.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://vja.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://doy.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://coj.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://ega.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://bzc.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://adt.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yjl.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://zeq.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://bhu.hammf.cn

[B09] break 与 continue
来源：http://lkt.cqqwz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gor.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vkp.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjg.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psm.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvy.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xln.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fxj.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hvi.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://wrg.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://flm.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vdc.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zyd.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pvv.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fwk.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qgi.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmq.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nqp.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://nwc.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://tjp.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://bnz.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oqa.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffp.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfa.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mip.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://lgb.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jbg.9152youxi.cn

[B12] 跳出多层循环
来源：http://afm.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yyp.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zcg.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avj.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucf.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lgd.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iiw.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rst.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nsl.yuxming.cn

[B13] 判断是否为数字
来源：http://oqq.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://mqt.wangdashe.top

PHP:  is_numeric($x)
来源：http://llh.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbx.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whv.ppjwa.cn

Java: x instanceof Number
来源：http://dly.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ejx.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://zux.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://nox.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://itv.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azf.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vfr.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://avo.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://hqf.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tsm.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://key.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://fuf.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fqv.sysykeji.top

[B15] 布尔运算与取反
来源：http://fqa.hfpthk.cn

Py:   a and b or not c
来源：http://wuc.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://ret.wangshuangyany.cn

JS:   a && b || !c
来源：http://dtn.hfpthk.cn

TS:   a && b || !c
来源：http://mjw.yanxiufei.cn

Java: a && b || !c
来源：http://shd.hnqzz.top

Go:   a && b || !c
来源：http://yku.yfazqb.com

Ruby: a && b || !c
来源：http://byw.vehdjk.com

C#:   a && b || !c
来源：http://ohn.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fou.redwolf501.top

Py:   if not data: return
来源：http://fhc.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://mdj.chenjidiqi.icu

JS:   if (!data) return;
来源：http://zlt.guannengcc.top

TS:   if (!data) return;
来源：http://aia.fehbvm.com

Java: if (data == null) return;
来源：http://axk.aizwys.cn

Go:   if data == nil { return }
来源：http://hps.havefunace.top

Ruby: return if data.nil?
来源：http://ubx.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://ady.cucudq.cn

================================================================================
来源：http://ocr.shangyingyoupin.top

C. 函数与作用域
来源：http://ijm.tianlin.xyz

================================================================================
来源：http://jeb.nanxinkj.top

[C01] 定义函数
来源：http://trh.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://dvk.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oaf.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://wtf.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cyi.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aep.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://irc.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://ibx.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwl.9152youxi.cn

[C02] 默认参数
来源：http://wae.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://ozi.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pab.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://lyi.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fdh.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://spu.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mwb.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://hbu.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://upi.birdmap.top

[C03] 可变参数
来源：http://ggg.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://zly.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cuj.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qup.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yys.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mld.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hjz.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://uqk.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://onw.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://fmh.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jav.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://szr.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://txn.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://itq.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://hkf.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://iqm.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://wym.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://vbf.birdmap.top

[C05] 返回多个值
来源：http://npv.jianghu66.top

Py:   return a, b
来源：http://zfs.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://tbg.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qxq.jqgufenzy.top

TS:   return { a, b };
来源：http://rpn.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://inj.hammf.cn

Go:   return a, b
来源：http://iil.gzhubu.top

Ruby: return a, b
来源：http://rfe.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://yzn.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://kyy.nwbrower.top

Py:   square = lambda x: x * x
来源：http://wgj.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yuo.meibo888.top

JS:   const square = x => x * x;
来源：http://ndg.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://guy.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ddk.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://fwt.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://hmq.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://xmp.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://isa.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://njx.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fsx.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ddh.xuetiantiany.cn

TS:   arr.map(String)
来源：http://sul.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ayg.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://msd.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://hct.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://wnm.0kj1m.cn

[C08] 闭包
来源：http://nwp.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hjz.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kkz.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://teu.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tym.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cox.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rxr.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://szt.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zng.ydjk.org.cn

[C09] 递归
来源：http://iuc.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pwa.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pll.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://viw.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kkk.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wsr.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kav.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cqy.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wby.guowangkeji.top

[C10] 变量作用域
来源：http://qpc.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbd.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rxd.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vaa.yueranfly.top

TS:   同 JS
来源：http://owy.chenlongwang.top

Java: 方法内为块级作用域
来源：http://nvl.fktsv.cn

Go:   花括号块级作用域
来源：http://paw.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hgx.pycfn.com

C#:   块级作用域
来源：http://jvd.nanxinkj.top

[C11] 模块导入与导出
来源：http://rik.yangfankeji.com

Py:   from module import func
来源：http://yaf.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kty.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://neu.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qrz.hongshengwenyu.top

Java: import java.util.List;
来源：http://oyd.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://akg.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://rot.zhixingplan.top

C#:   using System.Text;
来源：http://mld.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://jir.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://qve.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://nbx.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://mid.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://eig.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cec.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kvy.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://tps.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qiz.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://dza.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nzc.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xtr.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qcm.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcq.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://soi.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://sjn.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bek.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://ghf.haohaochexian.top

[C14] 泛型函数
来源：http://gbi.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uxn.guannengcc.top

PHP:  // 无泛型
来源：http://uxs.yj20258.top

JS:   // 无泛型
来源：http://lmn.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rtt.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fmv.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://noe.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://njd.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fyx.epnwcf.com

[C15] 解构 / 展开参数
来源：http://bpc.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cur.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://icx.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ubg.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://egg.iojbl.cn

Java: // 无解构
来源：http://qgl.quarkkingdee.top

Go:   // 无解构
来源：http://jfg.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://yol.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://qxg.yj202588.top

[C16] 函数 / 方法重载
来源：http://htm.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tyi.yongpay.top

PHP:  // 无重载
来源：http://nls.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hyi.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tdd.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://bey.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://znv.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://ced.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ypw.epnwcf.com

================================================================================
来源：http://cjf.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://mss.zycfv.cn

================================================================================
来源：http://rhj.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://lwe.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://qrj.zhixingplan.top


<!-- 参考信息 -->