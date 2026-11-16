代发 wailian999

[A26] 类型转换总览
来源：http://rxv.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uyt.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gsf.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cnh.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://wpa.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bxt.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gbz.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nac.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lmx.redwolf501.top

================================================================================
来源：http://fyi.yuanzhike.top

B. 流程控制
来源：http://vlt.xuanzx.com

================================================================================
来源：http://aki.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://brp.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wzf.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://shs.hammf.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ggp.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pfm.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sjz.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jch.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://huq.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wau.smart0.xyz

[B02] 多分支 else if / elif
来源：http://nib.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ioa.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://krm.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://auo.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buf.fehbvm.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tru.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zgj.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nfe.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://viu.fehbvm.com

[B03] switch / match / case
来源：http://uvs.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rfe.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vvf.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jbb.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://auy.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ats.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rcf.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mor.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xay.sufxvd.cn

[B04] for 计数循环
来源：http://jen.yj20258.top

Py:   for i in range(10): print(i)
来源：http://ymg.jqgfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dzy.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvf.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pol.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://swg.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lyv.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://ntp.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://knv.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://fal.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://rqg.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vpf.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://qzy.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://iyp.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mqq.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ptc.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://osa.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kyr.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://mmw.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://eoa.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jeb.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dyy.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lii.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sno.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vol.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://toy.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hdk.zycfv.cn

[B07] while 循环
来源：http://mur.cucudq.cn

Py:   while i < 10: i += 1
来源：http://nou.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://uku.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://dnp.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://qlk.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://dbj.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ugx.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://pxe.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://hqf.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://xbt.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ngy.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nhv.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://ckz.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://tnx.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://snl.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sit.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://vys.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://bay.9152youxi.cn

[B09] break 与 continue
来源：http://giz.jinghuilouyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ofm.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ukj.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmi.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpr.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjw.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tah.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ezs.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mil.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://sii.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xju.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lko.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ouh.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qte.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghh.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xzm.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://slw.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vds.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://ofo.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://gfl.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://oph.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kwb.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdo.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fvz.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zgp.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://tfw.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://auy.fengsongda.top

[B12] 跳出多层循环
来源：http://ueu.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wya.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gnk.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpn.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibk.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tyx.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ntc.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yxu.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kgu.xziqi.cn

[B13] 判断是否为数字
来源：http://jdh.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://cfw.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://ydd.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epy.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://feo.fengsongda.top

Java: x instanceof Number
来源：http://idz.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ruh.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://eoa.yj20258.top

C#:   x is int or double or decimal
来源：http://lqz.ydzc1.top

[B14] 判断值是否在集合内
来源：http://mnx.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vcr.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gcl.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://ytu.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://nzh.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rnc.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lag.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://gqp.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eep.ydzc1.top

[B15] 布尔运算与取反
来源：http://txf.svipenyu.cn

Py:   a and b or not c
来源：http://gem.316326.xyz

PHP:  $a && $b || !$c
来源：http://iik.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://oij.quarkkingdee.top

TS:   a && b || !c
来源：http://mbp.shuidangran.top

Java: a && b || !c
来源：http://aha.snrcjt.cn

Go:   a && b || !c
来源：http://szp.yj20258.top

Ruby: a && b || !c
来源：http://ssi.yanxiufei.cn

C#:   a && b || !c
来源：http://dac.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tte.hysaishi.cn

Py:   if not data: return
来源：http://kns.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://nhy.chenzaomai.com

JS:   if (!data) return;
来源：http://zkz.xinyue.icu

TS:   if (!data) return;
来源：http://zsn.hnqzz.top

Java: if (data == null) return;
来源：http://tzp.jinqigfzy.top

Go:   if data == nil { return }
来源：http://wpd.fzhhl.top

Ruby: return if data.nil?
来源：http://bnc.ehwqpu.com

C#:   if (data == null) return;
来源：http://sui.daria6918.cn

================================================================================
来源：http://mhr.ybcxt.top

C. 函数与作用域
来源：http://bgp.jianghu66.top

================================================================================
来源：http://lnu.9152youxi.cn

[C01] 定义函数
来源：http://ica.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://bct.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrh.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://wtp.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqo.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lfc.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://xfr.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://fec.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bof.yangfankeji.com

[C02] 默认参数
来源：http://jlb.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://nyn.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://elk.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://zob.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fut.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rnd.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ads.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://oem.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://bjr.jinyuanbaomall.cn

[C03] 可变参数
来源：http://wgq.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://zqv.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jlq.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqf.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahq.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rwi.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kue.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://nem.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qnv.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://vwv.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ipd.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rwp.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lkb.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gik.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://acw.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://shk.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://byo.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://dpw.cheryme.top

[C05] 返回多个值
来源：http://szv.pengpengdd.cyou

Py:   return a, b
来源：http://gal.yfazqb.com

PHP:  return [$a, $b];
来源：http://xjt.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://vnp.yongpay.top

TS:   return { a, b };
来源：http://zwh.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://upd.jinghuilouyu.cn

Go:   return a, b
来源：http://vyz.tarul.cn

Ruby: return a, b
来源：http://wli.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://sdy.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://kqz.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://zyx.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kje.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://vqa.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://bru.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dzp.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uoh.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://loe.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cyb.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://ivf.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gql.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://wsg.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uch.0kj1m.cn

TS:   arr.map(String)
来源：http://mns.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rdt.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ioq.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://maq.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tle.pycfn.com

[C08] 闭包
来源：http://lvz.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tfi.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qhu.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkg.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oor.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zxf.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jwv.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://heu.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qgs.ywan-chungtsiang.top

[C09] 递归
来源：http://cgj.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qkz.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uje.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mns.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yle.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwk.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhj.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lit.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktk.iojbl.cn

[C10] 变量作用域
来源：http://roy.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aez.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://clf.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ztj.dianchejie.cn

TS:   同 JS
来源：http://sby.sxryk.cn

Java: 方法内为块级作用域
来源：http://gfy.haohaochexian.top

Go:   花括号块级作用域
来源：http://mtd.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nok.hnqzz.top

C#:   块级作用域
来源：http://bcn.jinqigfzy.top

[C11] 模块导入与导出
来源：http://max.daria6918.cn

Py:   from module import func
来源：http://aie.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qeu.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://bjw.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ojm.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://vpf.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmq.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://mnz.fehbvm.com

C#:   using System.Text;
来源：http://xan.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://sut.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://oid.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://jse.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://jmx.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://pzg.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://quo.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://qcg.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://yfh.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://szg.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://vzv.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xru.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcs.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qhc.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfa.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://igo.daria6918.cn

Go:   func add(a, b int) int
来源：http://fya.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qeo.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dch.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://yyw.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jqr.zhongyouzk.top

PHP:  // 无泛型
来源：http://oyn.fengsongda.top

JS:   // 无泛型
来源：http://jfv.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ltk.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mfa.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rie.ctjpmb.com

Ruby: # 无泛型
来源：http://spa.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qhm.guannengcc.top

[C15] 解构 / 展开参数
来源：http://hwr.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nls.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://axq.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qhe.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ugq.316326.xyz

Java: // 无解构
来源：http://gcl.yanxiufei.cn

Go:   // 无解构
来源：http://abg.yonumen.top

Ruby: a, b = pair
来源：http://gkl.316326.xyz

C#:   var (a, b) = pair;
来源：http://jvc.hesvh.cn

[C16] 函数 / 方法重载
来源：http://eeq.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvk.316326.xyz

PHP:  // 无重载
来源：http://wzl.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cfh.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://ute.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://too.ydzc1.top


<!-- 参考信息 -->