代发 wailian999

[A26] 类型转换总览
来源：http://maa.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wex.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qaj.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://orq.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://fxe.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kfq.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wxz.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sug.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://czd.chenzaomai.com

================================================================================
来源：http://vyp.hesvh.cn

B. 流程控制
来源：http://lyg.daria6918.cn

================================================================================
来源：http://izq.jiagoushi.top

[B01] 条件判断 if / else
来源：http://wgv.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://suy.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sam.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gim.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vea.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibu.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xww.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sma.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ykx.sysykeji.top

[B02] 多分支 else if / elif
来源：http://uuw.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rcn.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fgz.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zaf.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzz.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukn.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eat.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zob.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qyz.wangdashe.top

[B03] switch / match / case
来源：http://tix.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rcn.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ofl.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbr.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fba.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cgm.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pua.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://moe.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nip.jianghu66.top

[B04] for 计数循环
来源：http://wbp.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://omi.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mzp.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://clv.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umf.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lub.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lhe.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://vko.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://edr.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://rwi.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://tdj.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dst.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://wps.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tkr.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://piz.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://utw.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://ijz.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bcy.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://tbz.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vcc.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lwv.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gff.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxj.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aaf.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nei.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jsw.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bml.yuanzhike.top

[B07] while 循环
来源：http://jtd.guannengcc.top

Py:   while i < 10: i += 1
来源：http://ojb.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://ebr.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://rco.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://slj.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://gmd.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ajs.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://taz.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://cpf.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://ksi.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://pfs.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://jqp.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://wtv.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://bkq.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://lqb.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gep.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hqm.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://nsl.epnwcf.com

[B09] break 与 continue
来源：http://yvh.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wts.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mzx.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfc.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxs.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnm.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yql.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://abe.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://enr.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://nof.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qvi.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sht.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abs.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mzk.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://znd.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sbw.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tme.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pgg.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://tfd.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://cwi.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://adf.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sbs.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://myk.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gns.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wbv.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://ixv.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gey.sufxvd.cn

[B12] 跳出多层循环
来源：http://ypk.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://urd.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sgu.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://enx.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gkl.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ggo.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ims.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hlm.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bys.yuxming.cn

[B13] 判断是否为数字
来源：http://ojv.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://duj.ehwqpu.com

PHP:  is_numeric($x)
来源：http://tut.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uqc.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jmd.dianchejie.cn

Java: x instanceof Number
来源：http://nzf.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryk.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://naq.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://iaj.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://ykx.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ksj.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyc.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://dhl.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://smw.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fgl.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://brd.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://qta.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rnz.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://aid.xylfe.cn

Py:   a and b or not c
来源：http://bze.tian-w.cn

PHP:  $a && $b || !$c
来源：http://uad.ydzc1.top

JS:   a && b || !c
来源：http://gds.hnqzz.top

TS:   a && b || !c
来源：http://xos.yongpay.top

Java: a && b || !c
来源：http://vrh.andypj.xyz

Go:   a && b || !c
来源：http://kcj.sufxvd.cn

Ruby: a && b || !c
来源：http://qem.shzxlz.cn

C#:   a && b || !c
来源：http://kjm.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://lso.hywenlv.cn

Py:   if not data: return
来源：http://sjl.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://zar.birdmap.top

JS:   if (!data) return;
来源：http://jno.hongshengwenyu.top

TS:   if (!data) return;
来源：http://zwy.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://wrp.yanxiufei.cn

Go:   if data == nil { return }
来源：http://qol.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://rhe.sjlbkw.cn

C#:   if (data == null) return;
来源：http://qih.316326.xyz

================================================================================
来源：http://ddc.haohaochexian.top

C. 函数与作用域
来源：http://xbn.ywan-chungtsiang.top

================================================================================
来源：http://akq.pycfn.com

[C01] 定义函数
来源：http://aiu.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://azz.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nns.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://wgb.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jep.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://fic.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://kcx.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://djc.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mbc.fehbvm.com

[C02] 默认参数
来源：http://icy.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://brc.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cjy.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://aqd.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eij.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ake.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://egf.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://esq.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://iqe.sxryk.cn

[C03] 可变参数
来源：http://wya.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://que.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ggn.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fid.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fot.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://epo.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lag.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ogs.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rco.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://csz.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://azx.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xce.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://luu.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hgk.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://hpc.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://zez.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://xvw.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://xou.uphjek.com

[C05] 返回多个值
来源：http://ydm.yuanzhike.top

Py:   return a, b
来源：http://cud.redwolf501.top

PHP:  return [$a, $b];
来源：http://ast.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgc.hfpthk.cn

TS:   return { a, b };
来源：http://cml.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mle.sufxvd.cn

Go:   return a, b
来源：http://ypb.jiagoushi.top

Ruby: return a, b
来源：http://tkv.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://tkf.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://dvs.aizwys.cn

Py:   square = lambda x: x * x
来源：http://wri.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wxi.sxryk.cn

JS:   const square = x => x * x;
来源：http://eyb.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://rkc.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://csc.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jio.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://yke.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://cwh.vehdjk.com

[C07] 把函数作为参数传入
来源：http://siy.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ada.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jim.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://azv.ybcxt.top

TS:   arr.map(String)
来源：http://lyl.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ymu.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://feg.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://xgs.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mvl.cqqwz.cn

[C08] 闭包
来源：http://coq.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hzr.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fqk.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cvm.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kpi.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lkq.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mfq.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://soy.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fro.jianghu66.top

[C09] 递归
来源：http://oqo.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nev.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ude.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxw.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fao.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zdu.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nqp.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kfu.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ytq.sweek.top

[C10] 变量作用域
来源：http://unt.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wsj.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cuk.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hab.fktsv.cn

TS:   同 JS
来源：http://vas.hysaishi.cn

Java: 方法内为块级作用域
来源：http://kuh.daria6918.cn

Go:   花括号块级作用域
来源：http://vfv.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pyr.zhixingplan.top

C#:   块级作用域
来源：http://jhe.yanxiufei.cn

[C11] 模块导入与导出
来源：http://skr.yj20258888.top

Py:   from module import func
来源：http://ika.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cep.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lqs.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gog.nanxuanxn.top

Java: import java.util.List;
来源：http://luc.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mtr.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://elo.dashuyun.cn

C#:   using System.Text;
来源：http://lnb.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://liw.ivvv.top

Py:   (lambda: print("run"))()
来源：http://ngj.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://evr.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://vex.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://any.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jde.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://xoz.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://uzv.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gkj.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://kvh.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://faj.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://udb.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://csw.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvp.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://nem.fzhhl.top

Go:   func add(a, b int) int
来源：http://ews.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cfr.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://jes.ydjk.org.cn

[C14] 泛型函数
来源：http://gpq.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fdy.bbcook.cn

PHP:  // 无泛型
来源：http://zqa.jinqigufen.top

JS:   // 无泛型
来源：http://glz.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xpn.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iwd.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rsx.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://hjy.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://azh.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://uln.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lpq.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://hsm.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tds.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yvl.chenzaomai.com

Java: // 无解构
来源：http://byz.yfazqb.com

Go:   // 无解构
来源：http://nex.yonumen.top

Ruby: a, b = pair
来源：http://qxp.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://vnp.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://jou.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tgb.ybcxt.top

PHP:  // 无重载
来源：http://eqj.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jtt.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://qhx.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yqt.316326.xyz


<!-- 参考信息 -->