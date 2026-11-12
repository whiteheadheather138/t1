代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sav.shzxlz.cn

================================================================================
来源：http://tys.guannengcc.top

B. 流程控制
来源：http://zsn.fengsongda.top

================================================================================
来源：http://kwe.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://oxm.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://itd.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mbp.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://urj.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dey.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://mnz.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://itg.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bav.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wod.yj202588.top

[B02] 多分支 else if / elif
来源：http://edj.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cse.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vfh.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uti.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vov.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uss.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://siy.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iyz.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shb.andypj.xyz

[B03] switch / match / case
来源：http://wwp.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tos.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xnv.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kaf.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gfv.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gxt.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ohb.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eko.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dih.ivvv.top

[B04] for 计数循环
来源：http://hsn.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://cux.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://psd.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pgf.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipn.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysi.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rbe.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://xrf.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ssg.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://mym.tarul.cn

Py:   for item in arr: print(item)
来源：http://sbt.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uim.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cpk.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kdr.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wdz.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmz.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://qid.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ujg.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://zdh.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qfe.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gds.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cbz.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uoo.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xrk.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://crl.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mwv.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://agz.sjlbkw.cn

[B07] while 循环
来源：http://tki.ydzc1.top

Py:   while i < 10: i += 1
来源：http://qen.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://cxe.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://iom.sweek.top

TS:   while (i < 10) { i++; }
来源：http://rcc.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://qxs.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xns.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://yjp.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://ohb.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://uhs.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://yhz.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pjs.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://sdy.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://msr.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://zvk.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wwd.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://fqx.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://wvn.xziqi.cn

[B09] break 与 continue
来源：http://nsx.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ile.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rwz.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://khm.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixq.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltp.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xus.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ikk.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pps.jianghu66.top

[B10] 遍历同时拿索引
来源：http://aji.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qcd.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cec.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jnj.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qiv.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uzx.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://coc.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bdi.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://asn.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://knh.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://cet.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://gsn.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjm.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mcw.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kzo.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wkm.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://uth.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bbm.gaohongyu789.top

[B12] 跳出多层循环
来源：http://mmc.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ern.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://qwr.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hmd.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbn.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://owd.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yvr.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zul.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tbd.zdqjudy.top

[B13] 判断是否为数字
来源：http://wpe.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://byz.havefunace.top

PHP:  is_numeric($x)
来源：http://ruy.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mdk.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hsa.0kj1m.cn

Java: x instanceof Number
来源：http://psi.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://axd.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://apz.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://sro.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://buy.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ksq.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://auj.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://ypw.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://zsm.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xmc.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wzk.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://awr.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfl.guowangkeji.top

[B15] 布尔运算与取反
来源：http://yoe.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://msj.wangdashe.top

PHP:  $a && $b || !$c
来源：http://imy.andypj.xyz

JS:   a && b || !c
来源：http://shx.mhx1999.top

TS:   a && b || !c
来源：http://roe.hnxiangtu.top

Java: a && b || !c
来源：http://maj.feifeiyinyue.top

Go:   a && b || !c
来源：http://enu.gzhubu.top

Ruby: a && b || !c
来源：http://zbp.9152youxi.cn

C#:   a && b || !c
来源：http://oth.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://urg.andypj.xyz

Py:   if not data: return
来源：http://rzq.hammf.cn

PHP:  if (!$data) { return; }
来源：http://nxa.sjlbkw.cn

JS:   if (!data) return;
来源：http://why.vehdjk.com

TS:   if (!data) return;
来源：http://dyd.cashguo.top

Java: if (data == null) return;
来源：http://tpd.bbcook.cn

Go:   if data == nil { return }
来源：http://nxy.yueranfly.top

Ruby: return if data.nil?
来源：http://mwy.hcnkem.com

C#:   if (data == null) return;
来源：http://teh.sufxvd.cn

================================================================================
来源：http://sul.ctjpmb.com

C. 函数与作用域
来源：http://kfk.jinyuanbaomall.cn

================================================================================
来源：http://wly.hesvh.cn

[C01] 定义函数
来源：http://bhk.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://zpy.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ult.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://lsd.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vzb.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lnu.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://epz.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://tml.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aeu.vehdjk.com

[C02] 默认参数
来源：http://jxx.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://dod.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://uuf.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://ktp.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lvp.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yim.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hcr.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://fvr.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://uoj.hesvh.cn

[C03] 可变参数
来源：http://zxa.sweek.top

Py:   def total(*args): return sum(args)
来源：http://fyn.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xds.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkd.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxi.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wba.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jjk.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jgb.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dtn.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://gco.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zkh.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://awy.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qll.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zlp.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://glw.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://yul.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://yvo.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://xql.snrcjt.cn

[C05] 返回多个值
来源：http://mrk.wangshuangyany.cn

Py:   return a, b
来源：http://kci.yangfankeji.com

PHP:  return [$a, $b];
来源：http://ssu.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bwd.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://msq.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bnu.jianghu66.top

Go:   return a, b
来源：http://qca.meibo888.top

Ruby: return a, b
来源：http://gsc.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://bqd.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://nqv.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://ujn.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wxb.fktsv.cn

JS:   const square = x => x * x;
来源：http://ogq.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://qre.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fik.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://mpq.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://gbx.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://lyd.ydzc1.top

[C07] 把函数作为参数传入
来源：http://yyy.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyn.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ggx.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://klr.fktsv.cn

TS:   arr.map(String)
来源：http://xmp.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://url.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sqn.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://jfy.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wsa.gotoacloud.top

[C08] 闭包
来源：http://goh.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://elu.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://awa.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cyv.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ikc.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dfj.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cca.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wqv.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zek.jinghuilouyu.cn

[C09] 递归
来源：http://thm.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://obi.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fjs.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://adr.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cqs.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vzg.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jwq.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tga.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vms.nanxuanxn.top

[C10] 变量作用域
来源：http://ylw.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://voh.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kxr.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmf.jiagoushi.top

TS:   同 JS
来源：http://jxm.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://lxx.chenzaomai.com

Go:   花括号块级作用域
来源：http://oll.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uuz.zdbjq.cn

C#:   块级作用域
来源：http://ynb.hammf.cn

[C11] 模块导入与导出
来源：http://hlf.fehbvm.com

Py:   from module import func
来源：http://pwg.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mzk.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zxb.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qwa.ppjwa.cn

Java: import java.util.List;
来源：http://cjx.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wlw.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://dmg.zycfv.cn

C#:   using System.Text;
来源：http://jkj.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://grr.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://cgq.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://wia.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://eor.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://vjn.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xol.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://ich.sweek.top

Ruby: -> { puts "run" }.call
来源：http://hij.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://kgn.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://vxu.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kpx.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxo.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ndx.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lfy.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cyy.cucudq.cn

Go:   func add(a, b int) int
来源：http://qah.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qpe.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mni.52xcode.cn

[C14] 泛型函数
来源：http://nrt.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fok.tanke756.top

PHP:  // 无泛型
来源：http://oax.redwolf501.top

JS:   // 无泛型
来源：http://ise.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vqo.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vwy.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hrg.jlsjyb.cn

Ruby: # 无泛型
来源：http://vnr.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hyc.redwolf501.top

[C15] 解构 / 展开参数
来源：http://ihv.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mbe.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://yfi.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ejk.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kuq.ybcxt.top

Java: // 无解构
来源：http://fgr.ivvv.top

Go:   // 无解构
来源：http://qkb.gogol.net.cn

Ruby: a, b = pair
来源：http://mbg.guannengcc.top

C#:   var (a, b) = pair;
来源：http://lnr.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://vco.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yvt.jqgufenzy.top

PHP:  // 无重载
来源：http://tyh.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fgx.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://cls.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://idm.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://brb.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://oep.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://rmx.snrcjt.cn

================================================================================
来源：http://icm.cheryme.top

D. 数组 / 列表 / 集合
来源：http://gxq.gotoacloud.top

================================================================================
来源：http://jgr.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://ehl.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xcr.zhoulong.xyz


<!-- 参考信息 -->