代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://whq.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nby.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vhl.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://hbr.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rat.zdqjudy.top

================================================================================
来源：http://tir.0kj1m.cn

B. 流程控制
来源：http://tro.yj202588.top

================================================================================
来源：http://drh.yvedp.cn

[B01] 条件判断 if / else
来源：http://lrr.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://xdp.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tyg.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ibw.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nja.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://htb.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zms.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zfd.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hia.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://lme.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://txy.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kqp.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wfn.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xow.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vuv.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dvq.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rez.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxn.hfpthk.cn

[B03] switch / match / case
来源：http://kpm.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ily.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rnr.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pjh.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpp.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kmw.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bud.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mtz.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wjh.cucudq.cn

[B04] for 计数循环
来源：http://zpt.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://klf.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lqf.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hrv.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dlc.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jih.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rgj.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://uuc.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nkx.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://vao.hammf.cn

Py:   for item in arr: print(item)
来源：http://ucm.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mfv.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vmy.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://itk.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://fsw.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qwy.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://tsy.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hdk.birdmap.top

[B06] 遍历字典 / 对象
来源：http://bve.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ihy.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zhh.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxs.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://omh.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jmk.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ila.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://org.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://quv.jqgufenzy.top

[B07] while 循环
来源：http://ini.bjfxy.top

Py:   while i < 10: i += 1
来源：http://vug.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://rxp.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://sgq.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://jer.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://mag.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://udv.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://naw.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://mov.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://kng.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://xql.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://foe.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://yvk.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://vto.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://aqk.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jum.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://mtw.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://cfe.shanyushiyangtech.top

[B09] break 与 continue
来源：http://qet.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jng.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xkf.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjv.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgm.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvo.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gje.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gpf.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttn.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://nmr.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://roo.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://duv.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zpd.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pnv.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uub.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tne.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yep.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vnc.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://nfd.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://aeb.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://wjc.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zbt.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nen.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://grs.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aab.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://clj.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hmj.yuxming.cn

[B12] 跳出多层循环
来源：http://nhh.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://njj.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mqu.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uow.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yyp.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uqz.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eth.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jio.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yci.hammf.cn

[B13] 判断是否为数字
来源：http://egc.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://tcs.ydzc1.top

PHP:  is_numeric($x)
来源：http://jjt.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbo.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vuz.jiagoushi.top

Java: x instanceof Number
来源：http://med.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zeu.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://wiy.cdnleiting.top

C#:   x is int or double or decimal
来源：http://qyz.zycfv.cn

[B14] 判断值是否在集合内
来源：http://dmz.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://drl.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dsv.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://gcv.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://ckk.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qoo.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jsi.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://voi.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zhy.redwolf501.top

[B15] 布尔运算与取反
来源：http://fdp.ivvv.top

Py:   a and b or not c
来源：http://xbo.bjfxy.top

PHP:  $a && $b || !$c
来源：http://ujj.xylfe.cn

JS:   a && b || !c
来源：http://gyu.iojbl.cn

TS:   a && b || !c
来源：http://qii.hammf.cn

Java: a && b || !c
来源：http://osa.zdbjq.cn

Go:   a && b || !c
来源：http://jgv.yangfankeji.com

Ruby: a && b || !c
来源：http://rzn.cqqwz.cn

C#:   a && b || !c
来源：http://jbl.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dvw.yanxiufei.cn

Py:   if not data: return
来源：http://lst.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://yae.0kj1m.cn

JS:   if (!data) return;
来源：http://pyc.zdqjudy.top

TS:   if (!data) return;
来源：http://wnb.cqqwz.cn

Java: if (data == null) return;
来源：http://qwp.svipenyu.cn

Go:   if data == nil { return }
来源：http://bqe.svipenyu.cn

Ruby: return if data.nil?
来源：http://ncq.iojbl.cn

C#:   if (data == null) return;
来源：http://nom.zdqjudy.top

================================================================================
来源：http://opu.yuxming.cn

C. 函数与作用域
来源：http://xrd.kuanghao11.cn

================================================================================
来源：http://cda.haohaochexian.top

[C01] 定义函数
来源：http://unl.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://mic.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofx.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://vae.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tln.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cnd.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://dam.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://roi.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gbf.sxryk.cn

[C02] 默认参数
来源：http://lgu.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://woi.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://opm.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://xtf.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zbm.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qdb.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rpj.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://dwz.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://qjv.jqgufenzy.top

[C03] 可变参数
来源：http://zhb.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://hwy.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hik.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://edq.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wcu.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bjm.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zto.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://myc.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://asj.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://fdr.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://osi.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yax.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zou.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fuj.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://qno.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://rwy.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://bjq.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://cvh.yuxming.cn

[C05] 返回多个值
来源：http://rtk.zhiwuduotai.top

Py:   return a, b
来源：http://nve.sufxvd.cn

PHP:  return [$a, $b];
来源：http://zcy.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wxq.fktsv.cn

TS:   return { a, b };
来源：http://bqn.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://reg.xziqi.cn

Go:   return a, b
来源：http://uhz.cdnleiting.top

Ruby: return a, b
来源：http://haj.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://hec.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://ucj.xinyue.icu

Py:   square = lambda x: x * x
来源：http://mxt.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://svv.haohaochexian.top

JS:   const square = x => x * x;
来源：http://qkx.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://kae.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bfc.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://agf.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://csq.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zch.redwolf501.top

[C07] 把函数作为参数传入
来源：http://bpj.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hus.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://qtr.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qxv.sweek.top

TS:   arr.map(String)
来源：http://yvy.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lnb.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gkq.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://uhk.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cie.vqdsnc.cn

[C08] 闭包
来源：http://plk.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ubk.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://unq.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rgc.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://avp.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://goq.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqk.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fvb.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vzn.shanyushiyangtech.top

[C09] 递归
来源：http://rjh.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gkc.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gkz.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nmw.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbf.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fep.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lnj.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nnm.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eoj.c1oappe.top

[C10] 变量作用域
来源：http://xiw.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jjf.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hgj.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmj.hammf.cn

TS:   同 JS
来源：http://skd.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://phy.yuanzhike.top

Go:   花括号块级作用域
来源：http://xtw.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://slb.sufxvd.cn

C#:   块级作用域
来源：http://ptn.gogol.net.cn

[C11] 模块导入与导出
来源：http://pcv.vqdsnc.cn

Py:   from module import func
来源：http://txf.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://xzv.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jvj.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pmb.ydjk.org.cn

Java: import java.util.List;
来源：http://jev.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cel.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://ucf.yj20258888.top

C#:   using System.Text;
来源：http://lvk.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://dyh.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://rea.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://fpf.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://llh.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://yuy.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gbj.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://nid.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://gfz.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hww.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://tex.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://usk.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qge.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lug.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qyv.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://sha.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://pxu.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mht.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ogv.yvedp.cn

[C14] 泛型函数
来源：http://qvy.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbb.52xcode.cn

PHP:  // 无泛型
来源：http://kpw.sxryk.cn

JS:   // 无泛型
来源：http://pwn.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rkh.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qst.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rfd.yj202588.top

Ruby: # 无泛型
来源：http://okf.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://reu.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://trc.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://glc.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://kto.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://noa.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kbz.fengsongda.top

Java: // 无解构
来源：http://saw.guowangkeji.top

Go:   // 无解构
来源：http://isv.pengpengdd.cyou

Ruby: a, b = pair
来源：http://nln.nwbrower.top

C#:   var (a, b) = pair;
来源：http://huu.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://tnu.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfr.fengsongda.top

PHP:  // 无重载
来源：http://bcg.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qnk.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://yde.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://psg.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://dgz.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://gup.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nft.fengsongda.top

================================================================================
来源：http://enc.jinghuilouyu.cn


<!-- 参考信息 -->