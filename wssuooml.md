代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xyw.xylfe.cn

================================================================================
来源：http://xof.kuanghao11.cn

B. 流程控制
来源：http://ozy.316326.xyz

================================================================================
来源：http://bqu.dianchejie.cn

[B01] 条件判断 if / else
来源：http://klz.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qih.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://llu.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://djb.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vxx.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://paz.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mip.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyr.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mat.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://ypu.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hvx.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qag.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npq.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://suu.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svq.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mie.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fub.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aro.zhengqikj.top

[B03] switch / match / case
来源：http://rev.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mdo.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mqo.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xtu.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bsp.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://siq.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bvx.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zpl.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://thg.zycfv.cn

[B04] for 计数循环
来源：http://hzk.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://whu.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jlh.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ats.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klr.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://egm.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ybc.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://dep.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rsa.hammf.cn

[B05] 遍历数组 / 列表
来源：http://add.uphjek.com

Py:   for item in arr: print(item)
来源：http://lhi.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qyh.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pye.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lfk.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://aeh.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qfu.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://qvr.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pqx.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://dtw.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nfp.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xax.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://roc.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ids.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ncl.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dch.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jsm.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fyw.hnxiangtu.top

[B07] while 循环
来源：http://fsu.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://jyt.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://yxe.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://frd.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://iuh.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://dgm.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://upu.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://rjc.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://upe.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://jbp.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://mzr.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vux.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://vha.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://nnh.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://bgk.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yco.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://nsu.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://rch.zhongyouzk.top

[B09] break 与 continue
来源：http://dbr.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cuy.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qkq.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fii.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsq.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afp.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://otr.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cqk.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azs.ybcxt.top

[B10] 遍历同时拿索引
来源：http://qbh.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ohb.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eow.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmw.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dhx.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ehl.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tts.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hld.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vhp.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://kms.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://rgc.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://bqd.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lwp.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqz.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aec.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gfd.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://hmu.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rgd.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://vyl.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ria.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ufl.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bnp.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://buz.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hgz.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pzz.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zjq.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bnt.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://ftv.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://xkf.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://nxr.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlo.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgz.nwbrower.top

Java: x instanceof Number
来源：http://ght.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://era.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://eis.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://sss.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://wbk.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjl.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axo.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://trf.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ivt.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mfm.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbs.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vwa.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ilv.52xcode.cn

[B15] 布尔运算与取反
来源：http://ckv.feifeiyinyue.top

Py:   a and b or not c
来源：http://spy.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://cjb.sxryk.cn

JS:   a && b || !c
来源：http://xyq.sxryk.cn

TS:   a && b || !c
来源：http://efa.zhiwuduotai.top

Java: a && b || !c
来源：http://yua.shangyingyoupin.top

Go:   a && b || !c
来源：http://kdo.chenjidiqi.icu

Ruby: a && b || !c
来源：http://yqj.havefunace.top

C#:   a && b || !c
来源：http://vce.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://iqr.hfpthk.cn

Py:   if not data: return
来源：http://axc.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://hyb.sxryk.cn

JS:   if (!data) return;
来源：http://kvb.ydzc1.top

TS:   if (!data) return;
来源：http://skf.gzhubu.top

Java: if (data == null) return;
来源：http://smr.daria6918.cn

Go:   if data == nil { return }
来源：http://yyg.yanxiufei.cn

Ruby: return if data.nil?
来源：http://xdo.cucudq.cn

C#:   if (data == null) return;
来源：http://dix.epnwcf.com

================================================================================
来源：http://tfq.haohaochexian.top

C. 函数与作用域
来源：http://rei.pycfn.com

================================================================================
来源：http://rda.hnxiangtu.top

[C01] 定义函数
来源：http://cdi.hammf.cn

Py:   def add(a, b): return a + b
来源：http://qfu.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hrp.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://exi.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sdm.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ifz.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iwo.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://wdn.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jtr.birdmap.top

[C02] 默认参数
来源：http://vlm.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://ktb.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://csq.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://snl.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mva.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ftd.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://auh.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://oaj.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://rzp.aibaodan.cn

[C03] 可变参数
来源：http://hks.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://aqx.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wdn.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pqp.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypk.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://crb.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xoo.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://xsy.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cwt.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://pgt.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pfn.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cmd.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://soq.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jtp.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://cfx.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://iih.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://sff.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://gxz.dianchejie.cn

[C05] 返回多个值
来源：http://soi.sweek.top

Py:   return a, b
来源：http://dlj.xinyue.icu

PHP:  return [$a, $b];
来源：http://man.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hfj.smart0.xyz

TS:   return { a, b };
来源：http://hsk.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbf.zhixingplan.top

Go:   return a, b
来源：http://tki.bjfxy.top

Ruby: return a, b
来源：http://nti.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://kpv.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://nwb.yfazqb.com

Py:   square = lambda x: x * x
来源：http://wsc.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ivu.hnqzz.top

JS:   const square = x => x * x;
来源：http://irn.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://ovs.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rqq.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://egz.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://dlz.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://ptw.guannengcc.top

[C07] 把函数作为参数传入
来源：http://zkp.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vto.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://drr.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sjw.yuxming.cn

TS:   arr.map(String)
来源：http://euu.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hjs.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://umu.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://tub.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ydc.ybcxt.top

[C08] 闭包
来源：http://rcm.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tiw.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://crc.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zsy.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dgh.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://irn.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gym.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sjs.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ppi.bbcook.cn

[C09] 递归
来源：http://dxd.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zod.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yht.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kni.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yii.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mui.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hfl.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qct.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txx.sjlbkw.cn

[C10] 变量作用域
来源：http://gfp.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://asu.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://osh.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://myu.ctjpmb.com

TS:   同 JS
来源：http://xhz.9152youxi.cn

Java: 方法内为块级作用域
来源：http://fxh.yanxiufei.cn

Go:   花括号块级作用域
来源：http://lkq.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jqj.xuetiantiany.cn

C#:   块级作用域
来源：http://tfw.cqqwz.cn

[C11] 模块导入与导出
来源：http://vqh.jinghuilouyu.cn

Py:   from module import func
来源：http://zld.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uee.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://fjb.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://siz.hywenlv.cn

Java: import java.util.List;
来源：http://hnm.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uze.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://lho.fktsv.cn

C#:   using System.Text;
来源：http://pcd.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://gvv.316326.xyz

Py:   (lambda: print("run"))()
来源：http://yru.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://glx.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://jtx.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://xrf.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ube.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://lim.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://alt.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://cmp.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://yio.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qhr.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dab.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zkw.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gkd.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://elf.sxryk.cn

Go:   func add(a, b int) int
来源：http://sie.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jfk.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://xws.hywenlv.cn

[C14] 泛型函数
来源：http://ahc.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nca.shangyingyoupin.top

PHP:  // 无泛型
来源：http://pfn.yangfankeji.com

JS:   // 无泛型
来源：http://fxw.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fdk.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gsr.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tma.jianghu66.top

Ruby: # 无泛型
来源：http://rtn.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://flz.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://xiq.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cjm.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://nes.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ija.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://byz.wangshuangyany.cn

Java: // 无解构
来源：http://off.jinqigfzy.top

Go:   // 无解构
来源：http://olk.xylfe.cn

Ruby: a, b = pair
来源：http://giw.bjfxy.top

C#:   var (a, b) = pair;
来源：http://cen.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://esx.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jpq.tanke756.top

PHP:  // 无重载
来源：http://taq.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dis.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://bgi.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sud.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://vdk.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://gfw.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gsh.xinyue.icu

================================================================================
来源：http://wgq.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://wli.ydjk.org.cn

================================================================================
来源：http://bad.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://hjh.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://roo.yanxiufei.cn


<!-- 参考信息 -->