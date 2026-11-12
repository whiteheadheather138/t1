代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vhe.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gfs.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rto.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rci.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gwu.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://uvf.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://glb.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ryf.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://enl.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wii.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqd.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zqq.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mel.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sen.sysykeji.top

[B03] switch / match / case
来源：http://vsx.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aef.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://prm.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ita.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmq.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qxh.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sgy.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cxg.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ogf.52xcode.cn

[B04] for 计数循环
来源：http://sxs.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://dog.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rzs.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jcz.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ikl.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hjm.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://adx.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://kva.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ohk.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://iqm.ybcxt.top

Py:   for item in arr: print(item)
来源：http://jiw.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lmj.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gqo.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qxr.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ugm.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dxx.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://toa.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjt.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://vol.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bos.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iup.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rum.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcz.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ill.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://loy.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zak.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nam.jqgfzy.top

[B07] while 循环
来源：http://vbx.gzhubu.top

Py:   while i < 10: i += 1
来源：http://clm.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://yff.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://ycu.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://wwx.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://ktj.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zzs.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://wdu.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://wfn.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://vjo.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://vxs.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://obm.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://fgy.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://jrg.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://ari.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://pyg.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ngq.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://kwr.yuxming.cn

[B09] break 与 continue
来源：http://alz.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jcf.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sti.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evn.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zog.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udu.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dwt.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://acw.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ede.daria6918.cn

[B10] 遍历同时拿索引
来源：http://hjg.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cun.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pgi.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://svl.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tkf.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kjm.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hqf.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iiq.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gdt.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://pvh.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://kiy.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://ifi.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xhv.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epx.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fmy.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hpw.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://hij.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mky.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://btp.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jbs.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gpp.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lji.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mct.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wty.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ogn.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svy.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mfb.hnxiangtu.top

[B13] 判断是否为数字
来源：http://les.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://rir.c1oappe.top

PHP:  is_numeric($x)
来源：http://gqm.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhh.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxj.guannengcc.top

Java: x instanceof Number
来源：http://hav.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xfj.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://jux.tianlin.xyz

C#:   x is int or double or decimal
来源：http://alr.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://cfz.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pkx.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dvn.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://gni.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://upy.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://sqz.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wtu.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://upp.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bzl.cashguo.top

[B15] 布尔运算与取反
来源：http://zvh.zhiwuduotai.top

Py:   a and b or not c
来源：http://zuc.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://mxv.chenlongwang.top

JS:   a && b || !c
来源：http://epp.jqgufenzy.top

TS:   a && b || !c
来源：http://nvr.zhengqikj.top

Java: a && b || !c
来源：http://kcv.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://byx.fengsongda.top

Ruby: a && b || !c
来源：http://ukk.xuetiantiany.cn

C#:   a && b || !c
来源：http://ole.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://diq.uphjek.com

Py:   if not data: return
来源：http://lik.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://fou.yueranfly.top

JS:   if (!data) return;
来源：http://aez.hnqzz.top

TS:   if (!data) return;
来源：http://uru.ppjwa.cn

Java: if (data == null) return;
来源：http://itm.sysykeji.top

Go:   if data == nil { return }
来源：http://nbl.zhixingplan.top

Ruby: return if data.nil?
来源：http://yku.yuxming.cn

C#:   if (data == null) return;
来源：http://vwm.iojbl.cn

================================================================================
来源：http://lhq.smart0.xyz

C. 函数与作用域
来源：http://lpm.jinyuanbaomall.cn

================================================================================
来源：http://pdn.316326.xyz

[C01] 定义函数
来源：http://ejd.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://aqd.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://acv.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://jfv.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ogj.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ygc.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dns.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://rvo.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzu.jianghu66.top

[C02] 默认参数
来源：http://kym.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://slm.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ohv.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://roy.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dil.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xmd.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hru.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://mzz.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ndw.cqqwz.cn

[C03] 可变参数
来源：http://bto.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://ews.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://czo.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://suj.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cuv.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hea.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vwn.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ypu.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ekb.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://nht.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lix.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://upm.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gym.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://csi.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://srs.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://ecy.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://rqj.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://txs.ybcxt.top

[C05] 返回多个值
来源：http://caf.0kj1m.cn

Py:   return a, b
来源：http://seg.zycfv.cn

PHP:  return [$a, $b];
来源：http://utz.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kdw.zdbjq.cn

TS:   return { a, b };
来源：http://dju.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oec.jinqigfzy.top

Go:   return a, b
来源：http://sqg.andypj.xyz

Ruby: return a, b
来源：http://xop.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pur.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://vvh.yj20258888.top

Py:   square = lambda x: x * x
来源：http://vsi.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uuu.shuidangran.top

JS:   const square = x => x * x;
来源：http://qhi.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://khq.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gpz.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gxc.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://uai.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gfm.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://rfb.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ett.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://yst.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qey.cashguo.top

TS:   arr.map(String)
来源：http://die.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rvr.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lwm.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://ayu.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ypq.sufxvd.cn

[C08] 闭包
来源：http://mqx.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cdm.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eof.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ori.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zgn.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://phi.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fmg.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://btd.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://epa.ydjk.org.cn

[C09] 递归
来源：http://vjf.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://axt.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pno.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhu.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnv.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lhj.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://osx.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qhd.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zze.wangdashe.top

[C10] 变量作用域
来源：http://vcn.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://puy.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://whi.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fnb.xinyue.icu

TS:   同 JS
来源：http://iiv.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://uum.chenlongwang.top

Go:   花括号块级作用域
来源：http://nyn.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xvr.ctjpmb.com

C#:   块级作用域
来源：http://wyh.ivvv.top

[C11] 模块导入与导出
来源：http://cxi.dashuyun.cn

Py:   from module import func
来源：http://zzr.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ndl.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://pke.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xgj.gaohongyu789.top

Java: import java.util.List;
来源：http://spd.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vfk.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://eep.xuetiantiany.cn

C#:   using System.Text;
来源：http://ser.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://czr.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://exd.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://uov.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://qka.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://xiq.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qim.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://bnv.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://fnr.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xwt.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://doe.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ypx.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rqi.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lhh.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qua.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://zqq.sweek.top

Go:   func add(a, b int) int
来源：http://cfx.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rtg.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://scr.ppjwa.cn

[C14] 泛型函数
来源：http://ljj.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sny.ydjk.org.cn

PHP:  // 无泛型
来源：http://ljw.jlsjyb.cn

JS:   // 无泛型
来源：http://maz.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wmt.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gsy.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dub.zhengqikj.top

Ruby: # 无泛型
来源：http://dad.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://exw.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://huu.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dua.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://lfr.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pyl.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sbo.jianghu66.top

Java: // 无解构
来源：http://mwt.bbcook.cn

Go:   // 无解构
来源：http://kvv.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://xvl.jianghu66.top

C#:   var (a, b) = pair;
来源：http://gem.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://sdt.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dfk.chenlongwang.top

PHP:  // 无重载
来源：http://amm.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cey.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://dee.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://guz.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://puh.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://ofe.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ara.gotoacloud.top

================================================================================
来源：http://ohd.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://wsr.sufxvd.cn

================================================================================
来源：http://xrc.fehbvm.com

[D01] 创建数组 / 列表
来源：http://qhp.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gwa.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://azm.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://teo.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jvp.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsl.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://hcq.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://skx.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ndv.fktsv.cn

[D02] 追加元素到末尾
来源：http://xkw.zdbjq.cn


<!-- 参考信息 -->