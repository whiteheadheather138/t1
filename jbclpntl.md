代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gyi.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lnw.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jus.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://liz.316326.xyz

[A26] 类型转换总览
来源：http://gkg.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vmn.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qch.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xha.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://izv.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qwb.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvu.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://tzr.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jif.sxryk.cn

================================================================================
来源：http://hmi.hysaishi.cn

B. 流程控制
来源：http://gjn.guowangkeji.top

================================================================================
来源：http://kzo.316326.xyz

[B01] 条件判断 if / else
来源：http://tca.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://onl.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dag.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tll.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oqc.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pzu.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lza.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nul.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://omr.andypj.xyz

[B02] 多分支 else if / elif
来源：http://wmd.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zbo.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ikd.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwz.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yya.quarkkingdee.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxa.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://izw.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qfr.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnz.c1oappe.top

[B03] switch / match / case
来源：http://ddo.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pdr.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fib.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmb.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvz.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gzy.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jpl.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kbu.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nhw.316326.xyz

[B04] for 计数循环
来源：http://mts.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://pjv.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ozm.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rny.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drh.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pvt.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uja.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://skc.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://svm.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://lat.yuxming.cn

Py:   for item in arr: print(item)
来源：http://lnq.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mzg.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yjl.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jzy.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://elf.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vrx.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://unp.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cxp.cheryme.top

[B06] 遍历字典 / 对象
来源：http://nty.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vsz.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jav.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpl.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rnr.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qos.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fhg.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ulh.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zpm.zhaomingkeji.xyz

[B07] while 循环
来源：http://vmb.tian-w.cn

Py:   while i < 10: i += 1
来源：http://wzx.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uil.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://uop.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://vgs.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://elt.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mwc.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://lwi.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://mra.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://shs.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://byw.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://npv.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://xpe.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://rvb.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://qqd.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://klm.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://cwq.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://omo.fehbvm.com

[B09] break 与 continue
来源：http://fnx.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://efm.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohq.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vxr.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdw.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lrh.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ptd.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://djz.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dvo.sweek.top

[B10] 遍历同时拿索引
来源：http://xgm.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://joe.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fre.gotoacloud.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yus.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fhk.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pfb.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://omo.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ycw.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xyo.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://pau.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://hmy.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://gsb.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bej.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vef.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qbt.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://acg.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://aka.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrf.jyoumei.cn

[B12] 跳出多层循环
来源：http://qdz.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ura.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wqz.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://itk.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yln.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ggi.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://adr.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xjo.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bmu.shzxlz.cn

[B13] 判断是否为数字
来源：http://pgo.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://xjn.smart0.xyz

PHP:  is_numeric($x)
来源：http://kix.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dss.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzz.wangshuangyany.cn

Java: x instanceof Number
来源：http://dtc.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gfk.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://scp.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://neu.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://vyc.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://auf.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bfe.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://opo.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://stl.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bhg.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abn.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://ivc.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hdp.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://juh.cucudq.cn

Py:   a and b or not c
来源：http://vae.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://okb.cheryme.top

JS:   a && b || !c
来源：http://wit.andypj.xyz

TS:   a && b || !c
来源：http://ipo.yanxiufei.cn

Java: a && b || !c
来源：http://xlu.tarul.cn

Go:   a && b || !c
来源：http://fxm.sysykeji.top

Ruby: a && b || !c
来源：http://aoe.guannengcc.top

C#:   a && b || !c
来源：http://irn.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://wym.wangdashe.top

Py:   if not data: return
来源：http://srn.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://ohb.hesvh.cn

JS:   if (!data) return;
来源：http://xua.chenjidiqi.icu

TS:   if (!data) return;
来源：http://xhf.cqqwz.cn

Java: if (data == null) return;
来源：http://fow.hnxiangtu.top

Go:   if data == nil { return }
来源：http://fnb.fehbvm.com

Ruby: return if data.nil?
来源：http://zec.sjlbkw.cn

C#:   if (data == null) return;
来源：http://ojv.quarkkingdee.top

================================================================================
来源：http://ity.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://ohk.9152youxi.cn

================================================================================
来源：http://cam.svipenyu.cn

[C01] 定义函数
来源：http://icc.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://lnv.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ayv.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://ash.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iip.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uod.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://emy.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://ljs.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jzs.ydzc1.top

[C02] 默认参数
来源：http://hhx.birdmap.top

Py:   def greet(name="World"): return name
来源：http://shh.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dzz.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://nba.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://usi.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://msl.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lrv.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://bpv.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://evl.havefunace.top

[C03] 可变参数
来源：http://zdu.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://sei.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ulo.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ayj.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sjw.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvq.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vns.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qzh.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cor.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://rtg.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mqx.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gdw.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vtc.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://plq.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://ndd.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://tgb.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://mgj.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://sbs.zhongyouzk.top

[C05] 返回多个值
来源：http://meq.yanxiufei.cn

Py:   return a, b
来源：http://lje.jqgfzy.top

PHP:  return [$a, $b];
来源：http://ihs.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://enl.xziqi.cn

TS:   return { a, b };
来源：http://pwp.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://axj.yueranfly.top

Go:   return a, b
来源：http://wsk.zhijiandao.cn

Ruby: return a, b
来源：http://fyc.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://yux.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://knh.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://rbx.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zsi.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://lpg.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://uob.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baw.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://glp.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://vtf.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://sgi.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://djv.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://inn.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://ddt.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aiw.pycfn.com

TS:   arr.map(String)
来源：http://dhm.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ijn.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jws.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://adg.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wst.dashuyun.cn

[C08] 闭包
来源：http://xua.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://suv.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mfc.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vay.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ayg.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yyd.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://chv.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jmk.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vgi.meibo888.top

[C09] 递归
来源：http://ogo.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zsy.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fsd.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bmo.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gkc.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fxe.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ixb.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ihr.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mxd.daxiang520.top

[C10] 变量作用域
来源：http://wsi.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://veb.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hvh.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qwn.zhijiandao.cn

TS:   同 JS
来源：http://xdz.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://lhg.xinyue.icu

Go:   花括号块级作用域
来源：http://qcw.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jat.fanxiaobao.xyz

C#:   块级作用域
来源：http://cic.fzhhl.top

[C11] 模块导入与导出
来源：http://bwe.ivvv.top

Py:   from module import func
来源：http://kmu.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zhl.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rkp.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yqz.fzhhl.top

Java: import java.util.List;
来源：http://qzf.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bzm.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://tqe.daxiang520.top

C#:   using System.Text;
来源：http://zjx.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://oei.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://huq.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://uei.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://cuv.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://rex.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ipe.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://qvq.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://ddb.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://agz.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://opp.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sgp.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdb.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nlc.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jcg.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://tgg.ehwqpu.com

Go:   func add(a, b int) int
来源：http://cjl.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxa.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://jbs.hnxiangtu.top

[C14] 泛型函数
来源：http://dmh.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bsu.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://ckw.sweek.top

JS:   // 无泛型
来源：http://pgj.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://egq.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ntv.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xow.dashuyun.cn

Ruby: # 无泛型
来源：http://lxj.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ran.redwolf501.top

[C15] 解构 / 展开参数
来源：http://lhk.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mwa.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://qfp.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dtj.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lyv.meibo888.top

Java: // 无解构
来源：http://zcf.xuanzx.com

Go:   // 无解构
来源：http://wur.shuidangran.top

Ruby: a, b = pair
来源：http://pnn.redwolf501.top

C#:   var (a, b) = pair;
来源：http://tdu.birdmap.top

[C16] 函数 / 方法重载
来源：http://eih.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wzw.xylfe.cn


<!-- 参考信息 -->