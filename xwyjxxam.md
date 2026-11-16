代发 wailian999

[A26] 类型转换总览
来源：http://ipp.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://exi.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ogk.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lmt.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://zoh.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zfw.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://prn.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ost.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qam.0kj1m.cn

================================================================================
来源：http://dfn.jqgfzy.top

B. 流程控制
来源：http://gjz.yongpay.top

================================================================================
来源：http://ssd.andypj.xyz

[B01] 条件判断 if / else
来源：http://mbi.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nvo.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nbj.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://heo.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vlr.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dct.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mfm.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dbt.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lhw.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://ork.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kql.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fob.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bas.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxb.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltx.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wru.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qze.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syb.redwolf501.top

[B03] switch / match / case
来源：http://ubo.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fdq.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rzv.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://foh.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ode.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uky.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kck.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xmz.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ilh.pengpengdd.cyou

[B04] for 计数循环
来源：http://wxb.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://dfm.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cnk.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gdf.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bqz.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nlz.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://usp.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://qes.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fhy.pycfn.com

[B05] 遍历数组 / 列表
来源：http://qva.cheryme.top

Py:   for item in arr: print(item)
来源：http://bro.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kgx.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bvo.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://lsm.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uwt.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://isv.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://jjh.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yeb.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://qpj.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://dea.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ald.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqp.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://flv.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vyg.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nsk.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://moq.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lqr.c1oappe.top

[B07] while 循环
来源：http://qiy.fzhhl.top

Py:   while i < 10: i += 1
来源：http://vmk.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjq.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://zwe.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://krc.yongpay.top

Java: while (i < 10) { i++; }
来源：http://mpm.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mcv.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://kcc.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://gts.hammf.cn

[B08] do-while（至少执行一次）
来源：http://juf.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://uif.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pmf.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://yak.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://sme.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://hum.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://lew.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://krb.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://uyb.gotoacloud.top

[B09] break 与 continue
来源：http://fgk.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ibh.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qpw.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vlh.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbr.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvq.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wbw.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qdr.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpb.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://keu.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fto.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xyo.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zse.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oop.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hnj.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://srf.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://csl.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ons.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://lnu.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://wyq.tanke756.top

PHP:  range(0, 10, 2);
来源：http://mci.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oks.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqw.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kzg.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gzc.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://vxj.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sbd.hnqzz.top

[B12] 跳出多层循环
来源：http://diy.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mnp.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://hqw.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mjh.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cxs.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xhy.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zma.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xtc.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aui.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://xll.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://vhy.sxryk.cn

PHP:  is_numeric($x)
来源：http://njy.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xpo.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wnn.shanyushiyangtech.top

Java: x instanceof Number
来源：http://tdh.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yox.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://ign.epnwcf.com

C#:   x is int or double or decimal
来源：http://set.daxiang520.top

[B14] 判断值是否在集合内
来源：http://uaa.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ips.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nkz.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://qxu.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://kdy.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vcj.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fci.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://vuc.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tca.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://why.jlsjyb.cn

Py:   a and b or not c
来源：http://bid.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://grd.sweek.top

JS:   a && b || !c
来源：http://nwp.jyoumei.cn

TS:   a && b || !c
来源：http://zpo.wangdashe.top

Java: a && b || !c
来源：http://unz.52xcode.cn

Go:   a && b || !c
来源：http://lax.yuanzhike.top

Ruby: a && b || !c
来源：http://mea.yuanzhike.top

C#:   a && b || !c
来源：http://fqg.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://qtt.jyoumei.cn

Py:   if not data: return
来源：http://jca.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://apy.chenjidiqi.icu

JS:   if (!data) return;
来源：http://jve.chenzaomai.com

TS:   if (!data) return;
来源：http://cpw.daria6918.cn

Java: if (data == null) return;
来源：http://ikp.gogol.net.cn

Go:   if data == nil { return }
来源：http://lcv.epnwcf.com

Ruby: return if data.nil?
来源：http://iyw.jlsjyb.cn

C#:   if (data == null) return;
来源：http://fyt.chenjidiqi.icu

================================================================================
来源：http://njy.havefunace.top

C. 函数与作用域
来源：http://cxw.yuanzhike.top

================================================================================
来源：http://gyb.xylfe.cn

[C01] 定义函数
来源：http://oyc.cashguo.top

Py:   def add(a, b): return a + b
来源：http://unl.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlr.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://cqm.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pug.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gru.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://bqf.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://foa.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zec.pycfn.com

[C02] 默认参数
来源：http://wio.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://bpl.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iwh.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://qlh.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rke.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://typ.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jzs.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://kcw.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://xxa.xuanzx.com

[C03] 可变参数
来源：http://dpe.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://ewj.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fst.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udg.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqq.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tdx.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iza.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://hoa.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://spu.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://fym.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://igt.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wks.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://arl.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lrk.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://jhx.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://ldu.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://pdf.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://qsz.yanxiufei.cn

[C05] 返回多个值
来源：http://tgu.ydzc1.top

Py:   return a, b
来源：http://voe.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://ntt.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qdp.hcnkem.com

TS:   return { a, b };
来源：http://vwi.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pqk.jinghuilouyu.cn

Go:   return a, b
来源：http://ltk.sufxvd.cn

Ruby: return a, b
来源：http://ota.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://hct.tarul.cn

[C06] 匿名函数 / lambda
来源：http://ukp.52xcode.cn

Py:   square = lambda x: x * x
来源：http://cyn.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ksh.andypj.xyz

JS:   const square = x => x * x;
来源：http://hzk.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://dyh.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nfw.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mio.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://iqg.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://pcw.bbcook.cn

[C07] 把函数作为参数传入
来源：http://pex.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wcq.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xqh.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hdu.gaohongyu789.top

TS:   arr.map(String)
来源：http://wlh.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fyp.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ppg.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://kyc.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vkb.tanke756.top

[C08] 闭包
来源：http://ggd.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ntg.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xuq.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gzm.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://plf.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tpb.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mxx.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://odt.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rer.9152youxi.cn

[C09] 递归
来源：http://zfw.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ces.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nyf.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wol.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lrb.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://chn.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://olh.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kwz.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://onl.jiagoushi.top

[C10] 变量作用域
来源：http://jqj.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nmi.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jdx.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ndo.havefunace.top

TS:   同 JS
来源：http://owu.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://ryk.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://epn.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kms.fengsongda.top

C#:   块级作用域
来源：http://tvm.ivvv.top

[C11] 模块导入与导出
来源：http://ctx.sjlbkw.cn

Py:   from module import func
来源：http://gqx.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pih.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://juy.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hnf.tian-w.cn

Java: import java.util.List;
来源：http://wek.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ooq.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://xsa.cdnleiting.top

C#:   using System.Text;
来源：http://net.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://oan.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://elx.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://snn.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://deh.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://jxe.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cou.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://vfd.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://dfa.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xtl.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://ypi.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ooa.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://paq.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lbz.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nyr.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://fts.iojbl.cn

Go:   func add(a, b int) int
来源：http://mtq.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nqe.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://xvb.yvedp.cn

[C14] 泛型函数
来源：http://ilq.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lpi.52xcode.cn

PHP:  // 无泛型
来源：http://lqr.dashuyun.cn

JS:   // 无泛型
来源：http://rky.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qzo.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bnl.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oue.sjlbkw.cn

Ruby: # 无泛型
来源：http://kih.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ate.uphjek.com

[C15] 解构 / 展开参数
来源：http://pfp.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bci.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://mtu.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxq.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://szv.guannengcc.top

Java: // 无解构
来源：http://vtz.hammf.cn

Go:   // 无解构
来源：http://aly.yuxming.cn

Ruby: a, b = pair
来源：http://yzc.yongpay.top

C#:   var (a, b) = pair;
来源：http://clz.yj202588.top

[C16] 函数 / 方法重载
来源：http://ufg.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gge.chenzaomai.com

PHP:  // 无重载
来源：http://eiz.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://okm.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://aru.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kuy.zhoulong.xyz


<!-- 参考信息 -->