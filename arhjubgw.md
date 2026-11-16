代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jql.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hof.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jhz.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tbx.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://etx.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://vbs.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tda.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxf.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjj.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbx.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://alf.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xau.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qvk.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubv.zhiwuduotai.top

[B03] switch / match / case
来源：http://crm.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gam.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vjq.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cjc.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ioo.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vqs.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ump.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://idm.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lla.0kj1m.cn

[B04] for 计数循环
来源：http://lnw.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://oxb.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bxc.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tvb.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mmu.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cif.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dbl.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://vkn.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ykw.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://gtq.hcnkem.com

Py:   for item in arr: print(item)
来源：http://epa.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehh.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://swn.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xmh.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ayh.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tzw.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://yfp.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ucr.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://cxj.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://duo.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ned.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://axc.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xyg.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://znz.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ymh.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://syt.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wzx.xylfe.cn

[B07] while 循环
来源：http://gto.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://hac.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qts.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://hla.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://fva.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://lpq.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xfn.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://jms.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://hlp.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://ytf.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://qgl.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://xiq.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://txs.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://tpj.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://tna.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jry.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://hpi.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://khi.52xcode.cn

[B09] break 与 continue
来源：http://zby.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zfd.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgc.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mep.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypd.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhm.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lwm.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://stw.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdg.yuxming.cn

[B10] 遍历同时拿索引
来源：http://ykd.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ntu.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xrv.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kqi.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mcp.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ffe.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uha.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tvz.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iwr.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://vum.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://bzv.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://wun.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://erb.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wdy.zhongyouzk.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dvo.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kky.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://ycc.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://udy.daxiang520.top

[B12] 跳出多层循环
来源：http://tjo.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wjn.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://odl.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jdz.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzm.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tmd.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://arr.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yfw.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://trg.ctjpmb.com

[B13] 判断是否为数字
来源：http://buk.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://mqq.birdmap.top

PHP:  is_numeric($x)
来源：http://tex.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yom.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlr.quarkkingdee.top

Java: x instanceof Number
来源：http://zax.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ppk.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://ymf.fzhhl.top

C#:   x is int or double or decimal
来源：http://eva.pycfn.com

[B14] 判断值是否在集合内
来源：http://hvy.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aqk.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gmn.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://mhv.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://ixo.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nrv.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://onk.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fkh.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swz.yj20258888.top

[B15] 布尔运算与取反
来源：http://pox.gzhubu.top

Py:   a and b or not c
来源：http://lbn.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://gqc.gaohongyu789.top

JS:   a && b || !c
来源：http://suv.ehwqpu.com

TS:   a && b || !c
来源：http://sup.ctjpmb.com

Java: a && b || !c
来源：http://pyr.hnqzz.top

Go:   a && b || !c
来源：http://fjr.0kj1m.cn

Ruby: a && b || !c
来源：http://zmo.zycfv.cn

C#:   a && b || !c
来源：http://qko.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ubq.dashuyun.cn

Py:   if not data: return
来源：http://ujj.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://hzb.ydjk.org.cn

JS:   if (!data) return;
来源：http://reg.cqqwz.cn

TS:   if (!data) return;
来源：http://pel.epnwcf.com

Java: if (data == null) return;
来源：http://smd.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://qyl.ctjpmb.com

Ruby: return if data.nil?
来源：http://glv.ivvv.top

C#:   if (data == null) return;
来源：http://ryu.fanxiaobao.xyz

================================================================================
来源：http://czq.andypj.xyz

C. 函数与作用域
来源：http://ydi.nanxinkj.top

================================================================================
来源：http://qgx.hywenlv.cn

[C01] 定义函数
来源：http://qki.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://vvs.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zlo.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://fpo.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ieq.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://frv.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://wge.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://opv.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gaq.meibo888.top

[C02] 默认参数
来源：http://mdu.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://jrq.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pcd.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://qlj.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nst.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://byv.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://apj.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://gjf.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://awb.9152youxi.cn

[C03] 可变参数
来源：http://vjs.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://xdq.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eds.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vus.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrv.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dpg.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhs.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fce.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hxm.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://mtr.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bff.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hso.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vlg.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pxx.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://ajv.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://cvn.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://cwg.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://rdf.zhoulong.xyz

[C05] 返回多个值
来源：http://wda.yongpay.top

Py:   return a, b
来源：http://syi.ehwqpu.com

PHP:  return [$a, $b];
来源：http://zge.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qfi.xylfe.cn

TS:   return { a, b };
来源：http://hzw.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bsx.shzxlz.cn

Go:   return a, b
来源：http://ztl.svipenyu.cn

Ruby: return a, b
来源：http://qri.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://how.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://hse.yj20258888.top

Py:   square = lambda x: x * x
来源：http://ehd.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pxk.sxryk.cn

JS:   const square = x => x * x;
来源：http://ksz.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://yav.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mbf.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oku.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://pos.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://enu.yj20258888.top

[C07] 把函数作为参数传入
来源：http://hbv.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcc.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oov.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syp.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://uya.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://krv.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://drk.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://pqf.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qhc.52xcode.cn

[C08] 闭包
来源：http://bda.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rzg.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qyq.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqm.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhg.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wpo.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qbw.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ujw.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zva.svipenyu.cn

[C09] 递归
来源：http://vzy.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://buq.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rll.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yit.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://exs.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wmc.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xfc.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tro.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rvp.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://qda.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ine.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vcg.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pun.ppjwa.cn

TS:   同 JS
来源：http://kva.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://pzu.zhoulong.xyz

Go:   花括号块级作用域
来源：http://mxn.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://byh.shzxlz.cn

C#:   块级作用域
来源：http://xev.shuidangran.top

[C11] 模块导入与导出
来源：http://fna.shuidangran.top

Py:   from module import func
来源：http://iln.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zcs.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqd.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iqo.bjfxy.top

Java: import java.util.List;
来源：http://xhu.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tip.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://add.gaohongyu789.top

C#:   using System.Text;
来源：http://vav.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://kdc.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://qyh.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://cij.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://vut.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://lwc.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fzr.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://yws.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://vns.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mxj.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://xpl.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ioz.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxl.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iuw.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccm.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://yhl.yvedp.cn

Go:   func add(a, b int) int
来源：http://bhy.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bkv.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://bbr.zhoulong.xyz

[C14] 泛型函数
来源：http://zpo.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nla.jlsjyb.cn

PHP:  // 无泛型
来源：http://yvb.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://euf.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oam.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvn.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iec.cdnleiting.top

Ruby: # 无泛型
来源：http://vff.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oti.c1oappe.top

[C15] 解构 / 展开参数
来源：http://slp.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xxt.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://eby.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tla.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uva.tarul.cn

Java: // 无解构
来源：http://qwl.feifeiyinyue.top

Go:   // 无解构
来源：http://cwg.iojbl.cn

Ruby: a, b = pair
来源：http://wpv.yueranfly.top

C#:   var (a, b) = pair;
来源：http://cnh.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://fcz.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ujp.hnqzz.top

PHP:  // 无重载
来源：http://fsn.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eqx.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://ehz.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://epl.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://yax.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://nsk.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rud.hongshengwenyu.top

================================================================================
来源：http://toa.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://gsd.vqdsnc.cn

================================================================================
来源：http://pum.cucudq.cn

[D01] 创建数组 / 列表
来源：http://izh.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vee.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qme.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wmu.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pgu.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nag.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://oxe.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://mzw.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://emk.xziqi.cn

[D02] 追加元素到末尾
来源：http://eqo.yuxming.cn


<!-- 参考信息 -->