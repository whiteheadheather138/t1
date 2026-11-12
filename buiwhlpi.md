代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://suz.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pyw.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://iwb.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mgz.zhoulong.xyz

[A26] 类型转换总览
来源：http://xey.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://slb.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cwj.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybh.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://vla.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bmb.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://euh.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://pzd.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bro.tian-w.cn

================================================================================
来源：http://vry.c1oappe.top

B. 流程控制
来源：http://jal.yanxiufei.cn

================================================================================
来源：http://gkv.cashguo.top

[B01] 条件判断 if / else
来源：http://mpb.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sve.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aca.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uew.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ksl.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wxk.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://azk.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ysi.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gkb.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://iiw.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aef.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bel.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kdk.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqn.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://avx.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://msd.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kzl.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmj.bbcook.cn

[B03] switch / match / case
来源：http://dhh.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xwf.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vng.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ysa.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pmp.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xom.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xhr.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iyt.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pdu.yfazqb.com

[B04] for 计数循环
来源：http://saz.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://ste.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dus.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ncq.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxa.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pll.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://raj.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://ljj.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pix.birdmap.top

[B05] 遍历数组 / 列表
来源：http://jsq.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://dvy.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wsp.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gpa.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://dan.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uov.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zbn.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://eik.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hrv.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://bdu.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eqt.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ums.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jin.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zij.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfa.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mfo.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bfp.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qlv.hcnkem.com

[B07] while 循环
来源：http://lnr.hammf.cn

Py:   while i < 10: i += 1
来源：http://joa.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://ssu.sweek.top

JS:   while (i < 10) { i++; }
来源：http://oou.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://mbd.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://fpf.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qhw.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://vhc.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://zen.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://scl.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://gba.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qmx.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://bax.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://xfu.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://tkq.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hxp.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://esg.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://bog.shuidangran.top

[B09] break 与 continue
来源：http://xel.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://knp.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://onv.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vfi.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfv.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mde.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lqc.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://npy.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xiq.fzhhl.top

[B10] 遍历同时拿索引
来源：http://www.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fgw.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tew.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mxt.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shq.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bkt.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iwl.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uts.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://efy.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://qfh.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://giw.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://qoa.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubv.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uvb.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ugx.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fzq.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://giy.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uus.zhengqikj.top

[B12] 跳出多层循环
来源：http://hga.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://olw.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qqm.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mhn.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://shu.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hny.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fay.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mly.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gqv.jinqigfzy.top

[B13] 判断是否为数字
来源：http://cpi.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://xds.fehbvm.com

PHP:  is_numeric($x)
来源：http://iab.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://muq.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ded.hywenlv.cn

Java: x instanceof Number
来源：http://fuw.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sch.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://ajh.aibaodan.cn

C#:   x is int or double or decimal
来源：http://azl.guannengcc.top

[B14] 判断值是否在集合内
来源：http://gsp.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gdm.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kql.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://fde.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://dxb.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pnh.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://phy.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://djb.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twu.gotoacloud.top

[B15] 布尔运算与取反
来源：http://cdr.jiagoushi.top

Py:   a and b or not c
来源：http://unj.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://qzj.ehwqpu.com

JS:   a && b || !c
来源：http://mow.fengsongda.top

TS:   a && b || !c
来源：http://nch.c1oappe.top

Java: a && b || !c
来源：http://adb.guowangkeji.top

Go:   a && b || !c
来源：http://aus.daxiang520.top

Ruby: a && b || !c
来源：http://nrw.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://exh.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://eno.ywan-chungtsiang.top

Py:   if not data: return
来源：http://eyl.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://gsq.andypj.xyz

JS:   if (!data) return;
来源：http://akd.xuetiantiany.cn

TS:   if (!data) return;
来源：http://ywq.yfazqb.com

Java: if (data == null) return;
来源：http://agn.fktsv.cn

Go:   if data == nil { return }
来源：http://zou.hesvh.cn

Ruby: return if data.nil?
来源：http://sny.dianchejie.cn

C#:   if (data == null) return;
来源：http://wwi.vqdsnc.cn

================================================================================
来源：http://ltx.9152youxi.cn

C. 函数与作用域
来源：http://zck.kuanghao11.cn

================================================================================
来源：http://frx.hfpthk.cn

[C01] 定义函数
来源：http://cba.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://anb.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yeh.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://cbp.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urk.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mbh.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://dgk.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://fzg.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ums.smart0.xyz

[C02] 默认参数
来源：http://rll.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://wte.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aff.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ssn.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tux.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lou.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cez.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://dbk.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://hge.vqdsnc.cn

[C03] 可变参数
来源：http://cdg.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://oep.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yhi.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://knc.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ehq.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cqy.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rix.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dgo.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dfd.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://spy.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kcg.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dxd.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yaf.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bit.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://wrq.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://dog.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://hho.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://awz.fengsongda.top

[C05] 返回多个值
来源：http://omd.0kj1m.cn

Py:   return a, b
来源：http://wzh.daxiang520.top

PHP:  return [$a, $b];
来源：http://xvf.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yvs.mhx1999.top

TS:   return { a, b };
来源：http://ivo.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://igt.cheryme.top

Go:   return a, b
来源：http://cyw.jlsjyb.cn

Ruby: return a, b
来源：http://ntu.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://iix.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://rev.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://mfk.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zze.guowangkeji.top

JS:   const square = x => x * x;
来源：http://xvs.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://xxg.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://emb.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ucv.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://nrg.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://qsj.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://zap.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kpw.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://guf.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gaw.sufxvd.cn

TS:   arr.map(String)
来源：http://zou.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://umb.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xak.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://bjb.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ryp.zhoulong.xyz

[C08] 闭包
来源：http://ono.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eqm.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bit.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wct.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tjc.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wtu.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uod.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cab.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qll.zhengqikj.top

[C09] 递归
来源：http://pxs.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dka.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qob.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dki.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khr.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xwq.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fwz.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rdu.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dlt.vqdsnc.cn

[C10] 变量作用域
来源：http://riu.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hzh.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xia.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bdr.shanyushiyangkeji.top

TS:   同 JS
来源：http://hyd.fktsv.cn

Java: 方法内为块级作用域
来源：http://wex.zhijiandao.cn

Go:   花括号块级作用域
来源：http://rek.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ofy.epnwcf.com

C#:   块级作用域
来源：http://tvz.kuanghao11.cn

[C11] 模块导入与导出
来源：http://cpj.hywenlv.cn

Py:   from module import func
来源：http://gez.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xhr.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bme.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sqv.meibo888.top

Java: import java.util.List;
来源：http://rvd.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xal.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://hwi.fanxiaobao.xyz

C#:   using System.Text;
来源：http://gvd.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://mhy.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://lnl.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://tsk.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://ubi.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://moh.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://itw.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://lqy.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://qhf.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zbo.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://tmr.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vrp.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyt.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bly.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yej.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://czb.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://vlz.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://etm.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://elz.yuanzhike.top

[C14] 泛型函数
来源：http://otp.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vit.uphjek.com

PHP:  // 无泛型
来源：http://clj.ivvv.top

JS:   // 无泛型
来源：http://hjs.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sqk.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wrs.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://det.chenjidiqi.icu

Ruby: # 无泛型
来源：http://wrk.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hzz.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://tja.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eon.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://qwp.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mcp.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://brs.yueranfly.top

Java: // 无解构
来源：http://gwc.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://ngt.cucudq.cn

Ruby: a, b = pair
来源：http://lkt.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://rxo.yj20258888.top

[C16] 函数 / 方法重载
来源：http://jgd.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fkq.sjlbkw.cn


<!-- 参考信息 -->