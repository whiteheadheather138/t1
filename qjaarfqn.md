代发 wailian999

[A26] 类型转换总览
来源：http://lzt.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kah.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tqc.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xri.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://jpq.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kai.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zae.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvx.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eef.ydzc1.top

================================================================================
来源：http://ovh.9152youxi.cn

B. 流程控制
来源：http://yjz.sjlbkw.cn

================================================================================
来源：http://gob.yangfankeji.com

[B01] 条件判断 if / else
来源：http://ddo.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jug.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://egd.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://orb.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mug.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://avt.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ufq.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ocd.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zhj.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://mqr.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rpt.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://krn.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxo.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axm.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xcb.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wlk.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tak.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmg.9152youxi.cn

[B03] switch / match / case
来源：http://xjq.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://efa.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mkn.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kei.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bfl.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mzz.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xey.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uia.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sre.pengpengdd.cyou

[B04] for 计数循环
来源：http://xjl.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://rvj.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kjp.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbb.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nvs.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcj.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dva.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://kaw.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eyd.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://lnd.tarul.cn

Py:   for item in arr: print(item)
来源：http://vmh.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gym.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yzc.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rqz.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fwh.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://frk.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://zrg.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uyx.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://cqs.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vyf.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mcw.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vun.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://avu.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sqy.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sag.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fgr.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qtf.yangfankeji.com

[B07] while 循环
来源：http://yuc.tanke756.top

Py:   while i < 10: i += 1
来源：http://awi.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://wws.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://cjp.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://lry.tarul.cn

Java: while (i < 10) { i++; }
来源：http://dja.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xye.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://yyz.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://hky.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://pyl.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://toy.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aqy.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://srj.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://svr.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://sdt.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://swp.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://mxa.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://gbw.cheryme.top

[B09] break 与 continue
来源：http://ycg.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://guk.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://twk.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnp.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odg.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhn.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zdz.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lee.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srs.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://brx.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mwv.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yrz.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvp.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yqr.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://glj.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://erb.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hxv.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rts.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://voj.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://hsg.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://vtg.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xls.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adv.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drf.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jal.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://bjf.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://smi.birdmap.top

[B12] 跳出多层循环
来源：http://tcw.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wjl.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gda.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibn.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aou.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rjz.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wvm.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://peo.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zrd.hysaishi.cn

[B13] 判断是否为数字
来源：http://lly.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://tdu.hfpthk.cn

PHP:  is_numeric($x)
来源：http://poa.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zed.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pss.yongpay.top

Java: x instanceof Number
来源：http://ltj.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mij.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://byi.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://rbt.hesvh.cn

[B14] 判断值是否在集合内
来源：http://lih.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://flv.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wxe.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://rzp.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://eky.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yoq.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eaw.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://llv.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gap.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://tzx.yfazqb.com

Py:   a and b or not c
来源：http://oln.ybcxt.top

PHP:  $a && $b || !$c
来源：http://aaf.pycfn.com

JS:   a && b || !c
来源：http://dae.zycfv.cn

TS:   a && b || !c
来源：http://ixx.yj202588.top

Java: a && b || !c
来源：http://sjx.daxiang520.top

Go:   a && b || !c
来源：http://cyu.mhx1999.top

Ruby: a && b || !c
来源：http://oyu.zhoulong.xyz

C#:   a && b || !c
来源：http://ifq.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://zqt.ehwqpu.com

Py:   if not data: return
来源：http://hct.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://lmi.chenjidiqi.icu

JS:   if (!data) return;
来源：http://kvc.gzhubu.top

TS:   if (!data) return;
来源：http://ohx.chenlongwang.top

Java: if (data == null) return;
来源：http://hxw.vehdjk.com

Go:   if data == nil { return }
来源：http://sqh.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://scg.xinyue.icu

C#:   if (data == null) return;
来源：http://sxg.birdmap.top

================================================================================
来源：http://toz.ydzc1.top

C. 函数与作用域
来源：http://bsd.shanyushiyangtech.top

================================================================================
来源：http://ivo.hcnkem.com

[C01] 定义函数
来源：http://omu.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://ocq.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gzp.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://hfz.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cae.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://njc.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://wnb.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://eur.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vfq.ydzc1.top

[C02] 默认参数
来源：http://ics.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://tuy.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tby.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://kru.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rdz.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aqw.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ofi.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://yhf.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://swh.shzxlz.cn

[C03] 可变参数
来源：http://jaz.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://inq.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rzb.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pdb.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgm.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vth.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fvh.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://wbk.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yhd.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://cxk.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ric.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sww.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gps.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://znw.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://lwr.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://jpj.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://xvi.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://wsj.yongpay.top

[C05] 返回多个值
来源：http://wxr.jinyuanbaomall.cn

Py:   return a, b
来源：http://ktk.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://yjt.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fjs.xylfe.cn

TS:   return { a, b };
来源：http://rys.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wep.yanxiufei.cn

Go:   return a, b
来源：http://btl.birdmap.top

Ruby: return a, b
来源：http://lhz.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://qoh.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://alq.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://okc.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gql.cqqwz.cn

JS:   const square = x => x * x;
来源：http://fiu.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://mvr.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://voi.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://mze.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://mzs.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://zsd.ivvv.top

[C07] 把函数作为参数传入
来源：http://fwz.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wra.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ory.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eig.hongshengwenyu.top

TS:   arr.map(String)
来源：http://emd.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qri.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rto.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://sic.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jie.iojbl.cn

[C08] 闭包
来源：http://bov.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dqx.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yjm.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wjd.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fqg.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dtn.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sxi.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pmu.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hsv.zhijiandao.cn

[C09] 递归
来源：http://ref.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qql.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wjd.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ici.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://owd.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ekw.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hxt.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ivl.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wce.chenzaomai.com

[C10] 变量作用域
来源：http://hbc.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xnl.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tia.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://stl.ctjpmb.com

TS:   同 JS
来源：http://zun.0kj1m.cn

Java: 方法内为块级作用域
来源：http://xvj.tianlin.xyz

Go:   花括号块级作用域
来源：http://orp.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://spx.ivvv.top

C#:   块级作用域
来源：http://fud.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://zss.aizwys.cn

Py:   from module import func
来源：http://qmq.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://onm.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wum.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zmw.meibo888.top

Java: import java.util.List;
来源：http://uqk.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bgu.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://mnu.cheryme.top

C#:   using System.Text;
来源：http://pbx.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://nyq.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://lje.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://xcj.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://hko.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://wuo.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://njx.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://etv.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://hii.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zyn.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://mvn.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mhs.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nky.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ycb.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjh.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://dop.cheryme.top

Go:   func add(a, b int) int
来源：http://gmg.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pgv.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://bmc.nanxinkj.top

[C14] 泛型函数
来源：http://ctf.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pcy.hywenlv.cn

PHP:  // 无泛型
来源：http://jep.shzxlz.cn

JS:   // 无泛型
来源：http://feg.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eon.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eev.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zyr.9152youxi.cn

Ruby: # 无泛型
来源：http://pde.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eeo.mhx1999.top

[C15] 解构 / 展开参数
来源：http://ybn.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://swc.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://bnl.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://swg.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qxs.dianchejie.cn

Java: // 无解构
来源：http://qob.yanxiufei.cn

Go:   // 无解构
来源：http://yuo.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://all.wangdashe.top

C#:   var (a, b) = pair;
来源：http://fsa.bjfxy.top

[C16] 函数 / 方法重载
来源：http://rjp.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pfj.tianlin.xyz

PHP:  // 无重载
来源：http://zrw.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ben.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://ceb.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://eba.nwbrower.top


<!-- 参考信息 -->