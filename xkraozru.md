代发 wailian999

[A26] 类型转换总览
来源：http://rhk.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jmx.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zlx.52xcode.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fsi.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://xxx.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kqc.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tzh.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kee.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kmt.meibo888.top

================================================================================
来源：http://tnh.zhixingplan.top

B. 流程控制
来源：http://txx.chenzaomai.com

================================================================================
来源：http://ifn.yangfankeji.com

[B01] 条件判断 if / else
来源：http://cby.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wcx.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hkc.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gjr.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://haz.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fuo.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ved.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dzp.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://buy.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://iqf.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxe.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://krz.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qoi.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtq.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aud.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://osn.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uxw.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vaw.iojbl.cn

[B03] switch / match / case
来源：http://aly.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gdq.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yww.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tni.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pdx.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bno.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ryk.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dvy.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://piv.jqgfzy.top

[B04] for 计数循环
来源：http://kkp.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://hmr.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://atl.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eeb.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qod.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iui.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iyg.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://akm.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://udv.yj20258.top

[B05] 遍历数组 / 列表
来源：http://rzp.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://xwh.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pqp.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oih.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dwc.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qgb.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://evc.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://exh.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qxy.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://uum.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ynl.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://twa.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aor.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kwt.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nea.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yij.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qap.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ovq.hnxiangtu.top

[B07] while 循环
来源：http://gro.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://jbc.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://mwx.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://tgs.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://wcv.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://syu.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pnt.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://pel.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://lkf.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://akg.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://yul.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://qzl.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://ins.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://wqi.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://ppd.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://acc.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://qbf.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://muv.sysykeji.top

[B09] break 与 continue
来源：http://lhs.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rqy.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oza.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axn.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gim.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svq.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://edo.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cck.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsk.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://nlp.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ybq.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pxq.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kio.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://idv.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aqu.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://knw.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://epg.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ekm.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://lgq.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://adl.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://won.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhk.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://csu.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ogo.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://caj.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://mlu.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dfw.yj202588.top

[B12] 跳出多层循环
来源：http://vvv.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://gdb.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cal.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://koy.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxn.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xtc.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aaw.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://len.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gpf.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://hdq.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://kzo.yuanzhike.top

PHP:  is_numeric($x)
来源：http://zsq.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uww.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxc.sufxvd.cn

Java: x instanceof Number
来源：http://pdt.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://whk.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://sot.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://bqr.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://gih.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yrw.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hzn.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://qtg.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://our.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qpy.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zqs.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://nfr.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nyy.jianghu66.top

[B15] 布尔运算与取反
来源：http://dqa.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://pdy.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://ryc.yuxming.cn

JS:   a && b || !c
来源：http://yjt.hfpthk.cn

TS:   a && b || !c
来源：http://xxo.chenzaomai.com

Java: a && b || !c
来源：http://zdj.shanyushiyangtech.top

Go:   a && b || !c
来源：http://lcl.9152youxi.cn

Ruby: a && b || !c
来源：http://uhp.aizwys.cn

C#:   a && b || !c
来源：http://new.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://lum.dashuyun.cn

Py:   if not data: return
来源：http://aaj.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://ceu.ydjk.org.cn

JS:   if (!data) return;
来源：http://wgb.wangdashe.top

TS:   if (!data) return;
来源：http://cca.yj202588.top

Java: if (data == null) return;
来源：http://ioc.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://ixv.ivvv.top

Ruby: return if data.nil?
来源：http://tmx.ppjwa.cn

C#:   if (data == null) return;
来源：http://vou.daria6918.cn

================================================================================
来源：http://gbx.ehwqpu.com

C. 函数与作用域
来源：http://bpx.aizwys.cn

================================================================================
来源：http://adr.316326.xyz

[C01] 定义函数
来源：http://std.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://aha.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://srf.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://swo.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://twz.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oka.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://swj.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://rti.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rfi.cqqwz.cn

[C02] 默认参数
来源：http://hfu.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://kfk.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://dvz.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://tfe.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nyy.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xzn.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cru.jqgufenzy.top

Ruby: def greet(name = "World") = name
来源：http://qjo.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://gnp.sweek.top

[C03] 可变参数
来源：http://csr.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://dqd.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vwc.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnq.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nud.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvs.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ghx.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://nbe.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lqb.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://wiy.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ads.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lod.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gpz.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hbv.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://znf.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://wlp.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://fqx.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://pbq.birdmap.top

[C05] 返回多个值
来源：http://ldz.hfpthk.cn

Py:   return a, b
来源：http://xgf.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://zpp.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cgh.shzxlz.cn

TS:   return { a, b };
来源：http://apm.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nib.sysykeji.top

Go:   return a, b
来源：http://dar.kuanghao11.cn

Ruby: return a, b
来源：http://zmb.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://efq.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://cqt.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://tur.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eaz.cucudq.cn

JS:   const square = x => x * x;
来源：http://zjv.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://pfl.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tur.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://tia.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://bca.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://tqd.meibo888.top

[C07] 把函数作为参数传入
来源：http://wbv.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eil.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://fax.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bih.c1oappe.top

TS:   arr.map(String)
来源：http://vzj.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nqj.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xsx.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://drq.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vdl.zhiwuduotai.top

[C08] 闭包
来源：http://bok.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://otm.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cnb.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oco.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hzv.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wlv.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zpy.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bmh.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fqc.jiagoushi.top

[C09] 递归
来源：http://elp.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://npn.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pob.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlz.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwa.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ubg.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lvr.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bpl.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bcx.birdmap.top

[C10] 变量作用域
来源：http://zke.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vql.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bto.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jlo.yj20258888.top

TS:   同 JS
来源：http://nzv.aibaodan.cn

Java: 方法内为块级作用域
来源：http://bec.hnxiangtu.top

Go:   花括号块级作用域
来源：http://vxf.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rdn.fehbvm.com

C#:   块级作用域
来源：http://ugn.yj20258.top

[C11] 模块导入与导出
来源：http://yod.jyoumei.cn

Py:   from module import func
来源：http://fbs.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uvv.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://klf.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gva.vqdsnc.cn

Java: import java.util.List;
来源：http://kio.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jby.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://jsv.quarkkingdee.top

C#:   using System.Text;
来源：http://vqm.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://hoi.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://dwi.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://uuz.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://ylg.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://vya.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cfi.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://czk.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://mak.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jpk.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://pib.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kvb.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnv.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hjs.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rjc.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://was.9152youxi.cn

Go:   func add(a, b int) int
来源：http://neg.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tiu.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://rgy.daxiang520.top

[C14] 泛型函数
来源：http://yjs.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tih.chenzaomai.com

PHP:  // 无泛型
来源：http://hro.andypj.xyz

JS:   // 无泛型
来源：http://iji.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxf.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rsu.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tlx.yj20258888.top

Ruby: # 无泛型
来源：http://kwl.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxt.sweek.top

[C15] 解构 / 展开参数
来源：http://cbb.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dtg.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://aim.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gpz.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ruw.hesvh.cn

Java: // 无解构
来源：http://jbi.wangshuangyany.cn

Go:   // 无解构
来源：http://cap.yj202588.top

Ruby: a, b = pair
来源：http://ewz.hnqzz.top

C#:   var (a, b) = pair;
来源：http://pdm.daxiang520.top

[C16] 函数 / 方法重载
来源：http://rnq.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://phb.gogol.net.cn

PHP:  // 无重载
来源：http://afj.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zmg.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://frw.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lxl.chenlongwang.top


<!-- 参考信息 -->