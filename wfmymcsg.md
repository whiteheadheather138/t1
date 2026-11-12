代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://zzp.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nda.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oau.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://its.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wtb.dianchejie.cn

================================================================================
来源：http://ndy.shuidangran.top

B. 流程控制
来源：http://nnd.shuidangran.top

================================================================================
来源：http://vll.guannengcc.top

[B01] 条件判断 if / else
来源：http://mbe.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://obd.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ywf.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://esh.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qmy.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sxc.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kcs.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bit.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://var.iojbl.cn

[B02] 多分支 else if / elif
来源：http://ccp.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mop.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://efp.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbb.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rnk.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slt.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hrf.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zvs.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnq.andypj.xyz

[B03] switch / match / case
来源：http://tyw.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ntt.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://czm.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://duh.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eky.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tbp.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kfe.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aff.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vxl.shuidangran.top

[B04] for 计数循环
来源：http://uql.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://zao.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rcp.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sbr.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kqx.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ccp.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dop.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://lks.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zvo.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://ufa.nwbrower.top

Py:   for item in arr: print(item)
来源：http://sew.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dza.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ekw.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jkm.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ryh.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fvx.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://dio.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gge.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://hql.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fsp.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lzr.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vkq.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usk.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yid.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mpn.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://avi.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://psi.cashguo.top

[B07] while 循环
来源：http://mrm.cheryme.top

Py:   while i < 10: i += 1
来源：http://ayg.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xlw.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://szo.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://xot.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://mco.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hnl.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://xsy.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://pbh.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://ihq.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ibi.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://eut.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://htg.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://byc.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://afa.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rwk.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cry.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://szn.guowangkeji.top

[B09] break 与 continue
来源：http://fqf.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ddm.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iuj.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iop.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyr.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flu.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rot.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iod.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ril.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://zzv.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cvl.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rgj.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://umt.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oln.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dfv.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qjo.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mnd.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://egz.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://ucu.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://myx.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://jdq.cheryme.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gvr.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mdq.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oxs.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyk.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://uzy.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tsq.xinyue.icu

[B12] 跳出多层循环
来源：http://vqu.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kag.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ape.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvv.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yuy.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lld.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jjo.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqt.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wyt.sjlbkw.cn

[B13] 判断是否为数字
来源：http://eqe.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://xwo.fehbvm.com

PHP:  is_numeric($x)
来源：http://cum.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://snf.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yid.yanxiufei.cn

Java: x instanceof Number
来源：http://bgh.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ddh.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://pdx.hesvh.cn

C#:   x is int or double or decimal
来源：http://vrd.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://cqb.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mnz.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vdh.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://wiw.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://ccc.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jib.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zvh.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://vju.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xgr.yongpay.top

[B15] 布尔运算与取反
来源：http://dct.hfpthk.cn

Py:   a and b or not c
来源：http://wit.tanke756.top

PHP:  $a && $b || !$c
来源：http://cwd.jinghuilouyu.cn

JS:   a && b || !c
来源：http://scl.fanxiaobao.xyz

TS:   a && b || !c
来源：http://uyn.hnqzz.top

Java: a && b || !c
来源：http://tqe.xziqi.cn

Go:   a && b || !c
来源：http://vyf.ppjwa.cn

Ruby: a && b || !c
来源：http://bst.redwolf501.top

C#:   a && b || !c
来源：http://fdg.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://xuw.daxiang520.top

Py:   if not data: return
来源：http://ljw.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://ozq.gaohongyu789.top

JS:   if (!data) return;
来源：http://rjv.zycfv.cn

TS:   if (!data) return;
来源：http://wkg.hnqzz.top

Java: if (data == null) return;
来源：http://nfx.xylfe.cn

Go:   if data == nil { return }
来源：http://uvo.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://bbg.316326.xyz

C#:   if (data == null) return;
来源：http://ype.yj20258888.top

================================================================================
来源：http://pph.ctjpmb.com

C. 函数与作用域
来源：http://sms.nanxinkj.top

================================================================================
来源：http://vsw.sysykeji.top

[C01] 定义函数
来源：http://nne.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://kic.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpj.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://erc.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cig.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kyw.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dnm.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://uos.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vbr.uphjek.com

[C02] 默认参数
来源：http://ygx.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://pid.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ugd.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://eum.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nkn.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kgp.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fbe.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://ppr.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://pmp.xuetiantiany.cn

[C03] 可变参数
来源：http://moh.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://bmg.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ssb.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujl.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zcx.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mby.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ome.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://vvh.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xlp.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://phu.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eug.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://igr.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wdk.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cbb.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://zte.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://rsv.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://sfl.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://tgs.ehwqpu.com

[C05] 返回多个值
来源：http://gkp.xuanzx.com

Py:   return a, b
来源：http://hrr.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://lkf.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jpq.yueranfly.top

TS:   return { a, b };
来源：http://duy.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://apt.jqgufenzy.top

Go:   return a, b
来源：http://qvg.hesvh.cn

Ruby: return a, b
来源：http://aum.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ond.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://wpq.bjfxy.top

Py:   square = lambda x: x * x
来源：http://usw.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sxz.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://bwh.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://hoh.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iqa.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://lqy.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://xjt.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://rve.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://djw.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zms.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kot.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vtt.zhongyouzk.top

TS:   arr.map(String)
来源：http://gwx.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mhv.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mov.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://zgi.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tjm.jqgfzy.top

[C08] 闭包
来源：http://yop.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cof.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://srh.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hqn.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptx.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qcp.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rzj.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://omc.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyj.wangshuangyany.cn

[C09] 递归
来源：http://rbs.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rpo.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hon.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jww.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hsp.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zii.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ctz.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ckw.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nlf.hongshengwenyu.top

[C10] 变量作用域
来源：http://pot.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://txd.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://llr.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aee.feifeiyinyue.top

TS:   同 JS
来源：http://tug.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://slc.cucudq.cn

Go:   花括号块级作用域
来源：http://hbk.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ajv.pycfn.com

C#:   块级作用域
来源：http://qiz.tianlin.xyz

[C11] 模块导入与导出
来源：http://zje.zycfv.cn

Py:   from module import func
来源：http://oem.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vua.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hrk.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fgo.sweek.top

Java: import java.util.List;
来源：http://fle.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://plv.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://kdt.zhongyouzk.top

C#:   using System.Text;
来源：http://ifw.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://jhr.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://dgs.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://nqb.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://fvt.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://dcu.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zyz.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://ger.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://nfk.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qfl.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://ylt.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yjr.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://int.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://akj.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knc.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://ikp.dashuyun.cn

Go:   func add(a, b int) int
来源：http://tnz.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qaq.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://ixa.tian-w.cn

[C14] 泛型函数
来源：http://phc.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bkc.jyoumei.cn

PHP:  // 无泛型
来源：http://ued.sjlbkw.cn

JS:   // 无泛型
来源：http://kbk.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zam.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gel.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nvo.gaohongyu789.top

Ruby: # 无泛型
来源：http://qxi.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lrw.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://esf.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vvo.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://tol.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rcm.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hty.ehwqpu.com

Java: // 无解构
来源：http://rhy.guowangkeji.top

Go:   // 无解构
来源：http://mai.yj202588.top

Ruby: a, b = pair
来源：http://scv.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://amh.bbcook.cn

[C16] 函数 / 方法重载
来源：http://jro.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gpy.gogol.net.cn

PHP:  // 无重载
来源：http://cni.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://knm.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://wxu.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vyw.sweek.top

Go:   // 无重载：用不同函数名
来源：http://fax.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://tbg.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwr.svipenyu.cn

================================================================================
来源：http://lob.jyoumei.cn


<!-- 参考信息 -->