代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yub.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jzg.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rfp.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zeu.jqgfzy.top

[A26] 类型转换总览
来源：http://rij.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ktw.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jit.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ipr.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://jwc.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wks.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://afq.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fjm.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://exy.yfazqb.com

================================================================================
来源：http://gmx.xziqi.cn

B. 流程控制
来源：http://tnx.9152youxi.cn

================================================================================
来源：http://qny.xziqi.cn

[B01] 条件判断 if / else
来源：http://sjc.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dyi.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iqb.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gab.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sld.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yxb.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://feo.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rzg.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ygd.andypj.xyz

[B02] 多分支 else if / elif
来源：http://blh.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fls.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jzk.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnq.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qde.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msn.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://arz.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qjs.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glt.jlsjyb.cn

[B03] switch / match / case
来源：http://jzz.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yia.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bfn.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://swv.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jkg.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fpl.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gzl.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpl.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://paw.smart0.xyz

[B04] for 计数循环
来源：http://soi.uphjek.com

Py:   for i in range(10): print(i)
来源：http://por.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ndj.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ate.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mij.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xfi.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tgo.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://uoj.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtm.yonumen.top

[B05] 遍历数组 / 列表
来源：http://ept.epnwcf.com

Py:   for item in arr: print(item)
来源：http://gsv.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rok.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://btp.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://eke.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jdn.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ihl.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://zui.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hbz.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://ait.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://htz.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lbs.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikq.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xeh.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oef.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cho.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wev.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aba.sweek.top

[B07] while 循环
来源：http://jxr.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://hgv.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://xst.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://car.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://nvy.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://yqx.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nfr.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://sid.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://djc.ivvv.top

[B08] do-while（至少执行一次）
来源：http://pyh.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://zjz.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xxd.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://ebo.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://mym.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://fvi.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://duc.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://dtf.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://dab.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://npm.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://djp.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lhs.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsf.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gww.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxj.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://avj.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vbd.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kby.xuanzx.com

[B10] 遍历同时拿索引
来源：http://pdh.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zdt.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kiz.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://erk.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fqx.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bfb.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yhb.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zon.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dcx.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://hck.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://fsz.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://pfc.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tpd.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cir.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bqi.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hwv.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://gbv.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yqj.yangfankeji.com

[B12] 跳出多层循环
来源：http://kvk.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://che.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fda.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kgp.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qll.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hsa.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sxz.hnqzz.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bgg.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zyt.ehwqpu.com

[B13] 判断是否为数字
来源：http://loe.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://qsa.yj20258888.top

PHP:  is_numeric($x)
来源：http://vff.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmd.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egk.ppjwa.cn

Java: x instanceof Number
来源：http://bhi.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://omi.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://qit.fktsv.cn

C#:   x is int or double or decimal
来源：http://wwh.yj202588.top

[B14] 判断值是否在集合内
来源：http://irn.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ubf.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qwc.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://jfc.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://gqo.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://shm.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://moe.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nop.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgr.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://vew.svipenyu.cn

Py:   a and b or not c
来源：http://oyq.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://vmq.wangdashe.top

JS:   a && b || !c
来源：http://zil.sweek.top

TS:   a && b || !c
来源：http://vxp.yuxming.cn

Java: a && b || !c
来源：http://zrt.yueranfly.top

Go:   a && b || !c
来源：http://wwj.yangfankeji.com

Ruby: a && b || !c
来源：http://uvq.redwolf501.top

C#:   a && b || !c
来源：http://brm.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://bts.snrcjt.cn

Py:   if not data: return
来源：http://lua.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://vdi.wangshuangyany.cn

JS:   if (!data) return;
来源：http://uta.yueranfly.top

TS:   if (!data) return;
来源：http://bno.feifeiyinyue.top

Java: if (data == null) return;
来源：http://tpp.hcnkem.com

Go:   if data == nil { return }
来源：http://rmb.smart0.xyz

Ruby: return if data.nil?
来源：http://tay.nanxuanxn.top

C#:   if (data == null) return;
来源：http://cst.c1oappe.top

================================================================================
来源：http://kxg.uphjek.com

C. 函数与作用域
来源：http://mys.shanyushiyangkeji.top

================================================================================
来源：http://cvx.hammf.cn

[C01] 定义函数
来源：http://oll.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://xcx.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gua.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://mqh.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzu.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://jct.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://cqg.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://qoq.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sie.yangfankeji.com

[C02] 默认参数
来源：http://gmf.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://fpz.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gem.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://wma.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://evo.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zom.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wsp.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://myk.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://mei.yuxming.cn

[C03] 可变参数
来源：http://ysw.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://hhy.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wmb.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrv.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oog.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fey.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mkg.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://xxw.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vfo.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://sdk.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ydp.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dcv.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gsd.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kvk.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://xty.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://pun.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://ign.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://esm.hnxiangtu.top

[C05] 返回多个值
来源：http://tdp.52xcode.cn

Py:   return a, b
来源：http://tew.uphjek.com

PHP:  return [$a, $b];
来源：http://mzg.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aep.meibo888.top

TS:   return { a, b };
来源：http://znp.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xgp.pengpengdd.cyou

Go:   return a, b
来源：http://adm.gotoacloud.top

Ruby: return a, b
来源：http://qtz.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://ple.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://xur.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://iqj.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vwi.52xcode.cn

JS:   const square = x => x * x;
来源：http://rql.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://vlq.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yvw.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vqk.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://mws.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://jzg.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://owe.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://utn.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://bao.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uqo.ivvv.top

TS:   arr.map(String)
来源：http://rsl.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ldc.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://abh.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://cfm.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cke.dianchejie.cn

[C08] 闭包
来源：http://nml.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gaw.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iuj.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dnl.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://htr.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nkp.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bks.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtl.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ypr.aibaodan.cn

[C09] 递归
来源：http://bli.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cot.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xcr.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dfr.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aeb.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://smo.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tln.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://css.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wmo.yueranfly.top

[C10] 变量作用域
来源：http://zby.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kcd.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xrd.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hdz.gogol.net.cn

TS:   同 JS
来源：http://pcr.jinqigufen.top

Java: 方法内为块级作用域
来源：http://rsp.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://uwx.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xkb.meibo888.top

C#:   块级作用域
来源：http://yqm.quarkkingdee.top

[C11] 模块导入与导出
来源：http://obd.daria6918.cn

Py:   from module import func
来源：http://ors.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qri.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bvt.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fnm.ehwqpu.com

Java: import java.util.List;
来源：http://hwy.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://put.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://chs.shangyingyoupin.top

C#:   using System.Text;
来源：http://vez.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://wme.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://quy.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://zvw.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://lyi.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://fub.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hqk.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://vqb.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://dot.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ftc.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://teb.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vht.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vaw.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yun.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efq.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://kyn.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://bhf.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://prg.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://use.zhengqikj.top

[C14] 泛型函数
来源：http://gqz.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qna.316326.xyz

PHP:  // 无泛型
来源：http://hmg.mhx1999.top

JS:   // 无泛型
来源：http://gpp.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vep.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bpb.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ual.jinqigfzy.top

Ruby: # 无泛型
来源：http://ewp.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yes.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://cfc.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fun.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://gnj.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ifa.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://urs.xingfuxueyuan.xyz

Java: // 无解构
来源：http://ddy.vqdsnc.cn

Go:   // 无解构
来源：http://fms.yanxiufei.cn

Ruby: a, b = pair
来源：http://orq.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://qxw.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://zux.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvj.guowangkeji.top


<!-- 参考信息 -->