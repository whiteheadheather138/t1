代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://goj.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zpn.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://whk.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ked.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gdf.yongpay.top

================================================================================
来源：http://eiu.ehwqpu.com

B. 流程控制
来源：http://ual.yonumen.top

================================================================================
来源：http://nrr.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://mjg.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pnm.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rrb.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ybe.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://czj.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://kos.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wdg.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://slg.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wde.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://pdp.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nyw.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wpb.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqv.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfo.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdt.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nzb.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hyx.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://voh.shangyingyoupin.top

[B03] switch / match / case
来源：http://glw.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uib.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bsi.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tkr.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibm.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chs.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vgb.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://elc.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lag.52xcode.cn

[B04] for 计数循环
来源：http://lny.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://afi.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ewj.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvn.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kkn.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysf.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ryo.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://tbg.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://non.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://ttw.hcnkem.com

Py:   for item in arr: print(item)
来源：http://ixt.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pfe.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qou.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://acv.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ani.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bvv.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://rpb.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://snr.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://dcc.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rga.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yop.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ebv.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ggc.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vox.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://igz.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yit.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pcy.xziqi.cn

[B07] while 循环
来源：http://ewe.tian-w.cn

Py:   while i < 10: i += 1
来源：http://tzo.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ptc.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://may.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://cwo.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://fvc.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wfp.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://zfo.sweek.top

C#:   while (i < 10) { i++; }
来源：http://xmz.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://zmu.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://qkk.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dtn.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://ggo.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://avj.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://eer.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ovz.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://wab.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://idq.zhongyouzk.top

[B09] break 与 continue
来源：http://jmt.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hjt.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nrl.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbz.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtk.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tay.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://poo.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://syf.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfi.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://vpz.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://die.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eyy.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xfr.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://srj.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cdq.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://znj.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tkk.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ixo.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://fjo.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://ayu.cheryme.top

PHP:  range(0, 10, 2);
来源：http://abm.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pww.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdp.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vxr.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gez.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://twk.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bgt.tarul.cn

[B12] 跳出多层循环
来源：http://kyb.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qox.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://adn.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhi.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qac.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bdf.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zqb.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bbb.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dlg.jqgufenzy.top

[B13] 判断是否为数字
来源：http://amp.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://ctn.daria6918.cn

PHP:  is_numeric($x)
来源：http://jcn.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hoc.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rhr.hesvh.cn

Java: x instanceof Number
来源：http://mhu.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xxo.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://xug.wangdashe.top

C#:   x is int or double or decimal
来源：http://scj.bbcook.cn

[B14] 判断值是否在集合内
来源：http://anz.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zeu.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ixa.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://hgo.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://ujf.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ktn.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zru.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://yqx.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exn.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://dpl.guannengcc.top

Py:   a and b or not c
来源：http://snl.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://hdk.xziqi.cn

JS:   a && b || !c
来源：http://rvz.tanke756.top

TS:   a && b || !c
来源：http://bkf.chenlongwang.top

Java: a && b || !c
来源：http://hqs.52xcode.cn

Go:   a && b || !c
来源：http://yvd.jqgfzy.top

Ruby: a && b || !c
来源：http://myk.zhijiandao.cn

C#:   a && b || !c
来源：http://eih.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://ejz.shangyingyoupin.top

Py:   if not data: return
来源：http://dva.uphjek.com

PHP:  if (!$data) { return; }
来源：http://qkq.xinyue.icu

JS:   if (!data) return;
来源：http://bdq.gzhubu.top

TS:   if (!data) return;
来源：http://sww.wangdashe.top

Java: if (data == null) return;
来源：http://vcu.fehbvm.com

Go:   if data == nil { return }
来源：http://kax.kuanghao11.cn

Ruby: return if data.nil?
来源：http://zml.ydjk.org.cn

C#:   if (data == null) return;
来源：http://xcx.haohaochexian.top

================================================================================
来源：http://dhm.zhaomingkeji.xyz

C. 函数与作用域
来源：http://ubc.yanxiufei.cn

================================================================================
来源：http://mpr.daria6918.cn

[C01] 定义函数
来源：http://mks.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://vyi.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqw.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://hbw.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tiv.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://djx.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://mou.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://wot.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rbb.jinyuanbaomall.cn

[C02] 默认参数
来源：http://cfw.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://rit.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mac.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://yqh.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kds.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ish.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aem.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://pag.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://ygi.nanxuanxn.top

[C03] 可变参数
来源：http://dgi.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://bms.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://htf.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pqc.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dtw.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://coa.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hok.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://jpj.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxr.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://kyz.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ith.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zrm.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fgq.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qev.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://tqy.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://vre.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://joz.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://bsp.tianlin.xyz

[C05] 返回多个值
来源：http://ofw.birdmap.top

Py:   return a, b
来源：http://ulf.nanxinkj.top

PHP:  return [$a, $b];
来源：http://aiw.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://hxd.tarul.cn

TS:   return { a, b };
来源：http://joq.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://joo.fktsv.cn

Go:   return a, b
来源：http://zha.guannengcc.top

Ruby: return a, b
来源：http://qhr.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://obl.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://bax.wangdashe.top

Py:   square = lambda x: x * x
来源：http://ewz.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://obh.mhx1999.top

JS:   const square = x => x * x;
来源：http://sta.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://bgd.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kcs.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tmc.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://hhp.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kpw.316326.xyz

[C07] 把函数作为参数传入
来源：http://ntp.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://clx.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://mne.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://prs.guowangkeji.top

TS:   arr.map(String)
来源：http://sqn.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://luo.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://din.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://edz.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://phd.jqgufenzy.top

[C08] 闭包
来源：http://suk.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bat.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pdg.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lel.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gwv.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mno.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rwo.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zno.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://swu.zhongyouzk.top

[C09] 递归
来源：http://jdd.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://frm.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pxg.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://shf.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjg.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjk.dashuyun.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://owj.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbo.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zkj.fengsongda.top

[C10] 变量作用域
来源：http://jxz.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://upb.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sgz.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xca.xylfe.cn

TS:   同 JS
来源：http://acb.redwolf501.top

Java: 方法内为块级作用域
来源：http://qwg.jqgufenzy.top

Go:   花括号块级作用域
来源：http://dwl.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://afr.hcnkem.com

C#:   块级作用域
来源：http://umi.fzhhl.top

[C11] 模块导入与导出
来源：http://tfh.fktsv.cn

Py:   from module import func
来源：http://hhp.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dua.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ejd.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nuw.9152youxi.cn

Java: import java.util.List;
来源：http://non.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ovo.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://lkm.hnqzz.top

C#:   using System.Text;
来源：http://wiv.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://opq.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://ias.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://kjh.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://wam.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://ted.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dne.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hiu.sweek.top

Ruby: -> { puts "run" }.call
来源：http://idg.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nfe.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://nqr.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ctq.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://far.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fcq.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://adc.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://czm.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://fdr.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ujz.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hqc.zhongyouzk.top

[C14] 泛型函数
来源：http://oqx.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fur.fengsongda.top

PHP:  // 无泛型
来源：http://rsb.shzxlz.cn

JS:   // 无泛型
来源：http://pvi.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hgg.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ijd.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ogv.uphjek.com

Ruby: # 无泛型
来源：http://xif.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vpi.cashguo.top

[C15] 解构 / 展开参数
来源：http://jha.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://brw.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://zek.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kuq.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ifw.zhongyouzk.top

Java: // 无解构
来源：http://ujf.zdqjudy.top

Go:   // 无解构
来源：http://xxp.shzxlz.cn

Ruby: a, b = pair
来源：http://afq.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://tzg.yueranfly.top

[C16] 函数 / 方法重载
来源：http://jcp.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wgo.meibo888.top

PHP:  // 无重载
来源：http://lwc.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lyf.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://ofl.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://oct.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://efj.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://qcv.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wtl.hywenlv.cn

================================================================================
来源：http://jzz.wangshuangyany.cn


<!-- 参考信息 -->