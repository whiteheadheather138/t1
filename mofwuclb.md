代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zkq.tian-w.cn

================================================================================
来源：http://zmy.hongshengwenyu.top

B. 流程控制
来源：http://jnd.xingfuxueyuan.xyz

================================================================================
来源：http://hth.zhengqikj.top

[B01] 条件判断 if / else
来源：http://ygb.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://atf.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sta.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rek.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yxe.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jqt.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kqv.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wqi.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lqj.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://eeu.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iia.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wxo.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://heq.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipc.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnw.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://twh.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://thd.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvi.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://ksz.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uen.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nhn.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xat.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lkb.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gzl.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sjf.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zvd.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sbe.zycfv.cn

[B04] for 计数循环
来源：http://qlz.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://ykf.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://urf.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qug.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kni.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uca.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lnh.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://oah.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://msg.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://fda.sysykeji.top

Py:   for item in arr: print(item)
来源：http://zso.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yiu.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://opz.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xpw.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mvi.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qcs.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://aqq.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bcc.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://jix.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vnz.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iok.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hfq.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dek.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bhm.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xbl.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qkn.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ohr.hesvh.cn

[B07] while 循环
来源：http://zfx.xinyue.icu

Py:   while i < 10: i += 1
来源：http://guw.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://crc.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://doe.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://hpj.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://yxb.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://avp.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://aih.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://zeq.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://wnc.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://prh.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://pur.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://gwt.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://ngt.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://khl.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wae.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://yts.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://rwg.yvedp.cn

[B09] break 与 continue
来源：http://nnl.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lkr.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rho.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffv.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://onq.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovx.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ljs.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uns.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocl.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://dtu.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qod.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udu.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cdu.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eej.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rva.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ytc.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xmj.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jnt.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://hgn.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://ksr.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://eur.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lkw.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjt.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pgt.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hwq.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://oje.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oqm.tarul.cn

[B12] 跳出多层循环
来源：http://ujm.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hzd.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jom.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kib.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nsn.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lgw.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ndo.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cld.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jti.havefunace.top

[B13] 判断是否为数字
来源：http://fsu.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://kvv.jianghu66.top

PHP:  is_numeric($x)
来源：http://kyg.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gxp.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://akz.sysykeji.top

Java: x instanceof Number
来源：http://lox.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cxn.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://klf.iojbl.cn

C#:   x is int or double or decimal
来源：http://dqj.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://nqd.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pij.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dyu.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://jmo.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://uch.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sec.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jyj.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://lsk.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pxq.havefunace.top

[B15] 布尔运算与取反
来源：http://lpj.cqqwz.cn

Py:   a and b or not c
来源：http://rjs.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://pqq.bbcook.cn

JS:   a && b || !c
来源：http://ytg.zdbjq.cn

TS:   a && b || !c
来源：http://qas.ppjwa.cn

Java: a && b || !c
来源：http://vxy.yueranfly.top

Go:   a && b || !c
来源：http://axd.shangyingyoupin.top

Ruby: a && b || !c
来源：http://bdk.fanxiaobao.xyz

C#:   a && b || !c
来源：http://rxk.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://ads.fehbvm.com

Py:   if not data: return
来源：http://grh.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://rde.sxryk.cn

JS:   if (!data) return;
来源：http://pen.nwbrower.top

TS:   if (!data) return;
来源：http://htm.yuanzhike.top

Java: if (data == null) return;
来源：http://bxo.pycfn.com

Go:   if data == nil { return }
来源：http://oln.yanxiufei.cn

Ruby: return if data.nil?
来源：http://svb.shuidangran.top

C#:   if (data == null) return;
来源：http://dem.hywenlv.cn

================================================================================
来源：http://xur.jqgfzy.top

C. 函数与作用域
来源：http://ezw.sjlbkw.cn

================================================================================
来源：http://hfj.ydjk.org.cn

[C01] 定义函数
来源：http://mjd.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://nrm.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bwm.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://mel.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmd.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rai.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://rvv.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://svl.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jon.havefunace.top

[C02] 默认参数
来源：http://ywx.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://zud.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ftp.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://nve.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://tar.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cuu.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kiy.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://wmj.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ouf.yuxming.cn

[C03] 可变参数
来源：http://psx.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://ukk.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lio.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pmr.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yei.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jyl.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ouv.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cdo.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://joj.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://fts.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gvi.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wmo.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tbp.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jeb.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://xds.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://rjj.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://mmr.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://yya.ehwqpu.com

[C05] 返回多个值
来源：http://zui.iojbl.cn

Py:   return a, b
来源：http://qim.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://zro.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zbb.gogol.net.cn

TS:   return { a, b };
来源：http://ydv.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgb.uphjek.com

Go:   return a, b
来源：http://azq.xuetiantiany.cn

Ruby: return a, b
来源：http://jwf.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://vwr.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://kqz.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://ibp.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bnw.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://ydf.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://man.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nwi.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://nzv.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://fus.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://ejv.hammf.cn

[C07] 把函数作为参数传入
来源：http://juq.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kgt.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://lei.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://als.jlsjyb.cn

TS:   arr.map(String)
来源：http://pya.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nzt.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yuo.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://zml.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xwj.cheryme.top

[C08] 闭包
来源：http://wfr.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bfv.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://osg.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gpr.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgq.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mak.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mce.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dab.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ofx.jinqigfzy.top

[C09] 递归
来源：http://hww.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vlq.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epb.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yve.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://awe.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://amn.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://guz.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fsj.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zka.9152youxi.cn

[C10] 变量作用域
来源：http://khr.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qwh.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qdo.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://laa.316326.xyz

TS:   同 JS
来源：http://hlz.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://qnd.dashuyun.cn

Go:   花括号块级作用域
来源：http://wbw.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://snb.pengpengdd.cyou

C#:   块级作用域
来源：http://srp.aizwys.cn

[C11] 模块导入与导出
来源：http://oqc.hesvh.cn

Py:   from module import func
来源：http://eky.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phl.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://efd.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdz.redwolf501.top

Java: import java.util.List;
来源：http://zlf.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wwo.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://foc.gaohongyu789.top

C#:   using System.Text;
来源：http://thl.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://div.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://jiu.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://aoo.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://gkl.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://kvc.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qxf.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://ohm.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://xsd.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ubm.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://dll.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fvu.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rwe.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hje.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfb.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://iqh.yj20258888.top

Go:   func add(a, b int) int
来源：http://csz.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://snk.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://him.meibo888.top

[C14] 泛型函数
来源：http://xkq.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mgc.hywenlv.cn

PHP:  // 无泛型
来源：http://hwm.zhijiandao.cn

JS:   // 无泛型
来源：http://qkf.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ykf.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://may.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rpb.gogol.net.cn

Ruby: # 无泛型
来源：http://tgf.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bok.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://hnj.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lmz.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://gqu.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fbd.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pfo.zdqjudy.top

Java: // 无解构
来源：http://kbv.9152youxi.cn

Go:   // 无解构
来源：http://gqu.jqgufenzy.top

Ruby: a, b = pair
来源：http://iav.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://inj.bbcook.cn

[C16] 函数 / 方法重载
来源：http://ghq.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mvi.zhixingplan.top

PHP:  // 无重载
来源：http://zrh.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rpy.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://cbl.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wqt.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://kdj.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://ueu.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://emy.pycfn.com

================================================================================
来源：http://kkj.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://sep.yj20258888.top

================================================================================
来源：http://urx.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://yat.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tfg.ydjk.org.cn


<!-- 参考信息 -->