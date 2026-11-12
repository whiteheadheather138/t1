代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ggi.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ddd.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vgi.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hiu.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xtc.xylfe.cn

[B02] 多分支 else if / elif
来源：http://isn.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lhk.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://duu.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jak.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mss.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hae.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nwx.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yyh.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsl.cashguo.top

[B03] switch / match / case
来源：http://dnt.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qcx.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ggs.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nnz.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fhn.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mxv.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hiq.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cmv.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eqz.jqgufenzy.top

[B04] for 计数循环
来源：http://vis.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://sya.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tlh.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnk.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jzq.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://isk.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pll.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://llp.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kea.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://mcn.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://kop.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pzq.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lcf.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wfg.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wwx.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mpx.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://qon.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xdn.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://zti.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ich.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zsg.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pha.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uif.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ums.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tnj.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bkd.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rlr.gotoacloud.top

[B07] while 循环
来源：http://zcg.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://hdr.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vsl.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://lgx.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://hie.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://cub.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ext.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://vrk.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://pjz.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://hze.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://vah.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://zku.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://faf.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://lcg.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://ygn.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://acg.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://bey.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://cag.hfpthk.cn

[B09] break 与 continue
来源：http://rkc.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tmz.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hca.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcz.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egw.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svv.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pan.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iot.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixj.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://dbb.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bmv.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sls.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kxb.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ttt.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mlh.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qye.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qfe.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rtm.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://ogl.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://huy.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://ofc.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jmh.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://evt.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xaz.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ecn.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://rup.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bay.wangdashe.top

[B12] 跳出多层循环
来源：http://ppl.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tkv.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nrj.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eqn.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ttw.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gha.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yar.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xqb.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gwj.cqqwz.cn

[B13] 判断是否为数字
来源：http://pho.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://qmd.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://zmc.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hxi.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfr.fktsv.cn

Java: x instanceof Number
来源：http://for.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zac.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://gzk.fengsongda.top

C#:   x is int or double or decimal
来源：http://suk.bbcook.cn

[B14] 判断值是否在集合内
来源：http://ujf.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jwr.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://naw.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://yyn.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://qnn.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://haq.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eeq.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://idn.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qid.hywenlv.cn

[B15] 布尔运算与取反
来源：http://xzl.mhx1999.top

Py:   a and b or not c
来源：http://wgq.yfazqb.com

PHP:  $a && $b || !$c
来源：http://kvg.c1oappe.top

JS:   a && b || !c
来源：http://gqj.epnwcf.com

TS:   a && b || !c
来源：http://hel.birdmap.top

Java: a && b || !c
来源：http://kty.vehdjk.com

Go:   a && b || !c
来源：http://ikn.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://kgb.yanxiufei.cn

C#:   a && b || !c
来源：http://aqd.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wzp.jqgfzy.top

Py:   if not data: return
来源：http://gah.pycfn.com

PHP:  if (!$data) { return; }
来源：http://jbs.ctjpmb.com

JS:   if (!data) return;
来源：http://gyy.xuanzx.com

TS:   if (!data) return;
来源：http://gto.aibaodan.cn

Java: if (data == null) return;
来源：http://riy.zhijiandao.cn

Go:   if data == nil { return }
来源：http://jdl.jyoumei.cn

Ruby: return if data.nil?
来源：http://ggh.yonumen.top

C#:   if (data == null) return;
来源：http://pej.tianlin.xyz

================================================================================
来源：http://xpi.havefunace.top

C. 函数与作用域
来源：http://zum.zhongyouzk.top

================================================================================
来源：http://yso.yj20258888.top

[C01] 定义函数
来源：http://snn.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://whj.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txy.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://jss.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pni.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kec.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://tbw.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://dif.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wml.yuanzhike.top

[C02] 默认参数
来源：http://djj.tarul.cn

Py:   def greet(name="World"): return name
来源：http://dqm.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cfs.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://sez.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://khx.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://lag.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yag.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://cul.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://yni.shzxlz.cn

[C03] 可变参数
来源：http://psj.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://scq.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qws.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibm.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hly.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnu.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hrh.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://zho.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nzm.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://etx.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://chx.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://akx.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://szd.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mda.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://huc.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://wgq.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://drv.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://stp.hcnkem.com

[C05] 返回多个值
来源：http://eim.shangyingyoupin.top

Py:   return a, b
来源：http://ozo.yfazqb.com

PHP:  return [$a, $b];
来源：http://kwg.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ytw.jinqigufen.top

TS:   return { a, b };
来源：http://bnq.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zpq.smart0.xyz

Go:   return a, b
来源：http://hlj.shanyushiyangkeji.top

Ruby: return a, b
来源：http://njl.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://flu.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://qoz.xuanzx.com

Py:   square = lambda x: x * x
来源：http://mvx.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qmp.birdmap.top

JS:   const square = x => x * x;
来源：http://kmk.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://kdb.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://coh.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dbu.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://nwc.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://kon.bbcook.cn

[C07] 把函数作为参数传入
来源：http://gfa.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ulj.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kuc.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ycg.9152youxi.cn

TS:   arr.map(String)
来源：http://eoz.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oil.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sac.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://usr.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ali.yongpay.top

[C08] 闭包
来源：http://flp.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bwc.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kim.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skr.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mue.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oah.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ehp.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://czm.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rri.nanxinkj.top

[C09] 递归
来源：http://nic.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tgj.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dxi.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppw.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ums.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://euo.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://say.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xgh.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hpx.hfpthk.cn

[C10] 变量作用域
来源：http://fhs.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wwp.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qcj.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qqy.yj202588.top

TS:   同 JS
来源：http://qum.nanxinkj.top

Java: 方法内为块级作用域
来源：http://ngk.hfpthk.cn

Go:   花括号块级作用域
来源：http://yta.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hev.zhoulong.xyz

C#:   块级作用域
来源：http://egy.0kj1m.cn

[C11] 模块导入与导出
来源：http://gql.9152youxi.cn

Py:   from module import func
来源：http://swf.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://siq.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qsw.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pty.hammf.cn

Java: import java.util.List;
来源：http://ler.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pjx.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://ptj.pycfn.com

C#:   using System.Text;
来源：http://fip.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://hxl.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://tjg.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://uxs.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://uxs.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://rtb.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mkg.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://fso.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://azy.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vzh.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://ehq.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nqe.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pjz.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zgd.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdp.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://kbg.zhengqikj.top

Go:   func add(a, b int) int
来源：http://kht.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kdr.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://rda.hongshengwenyu.top

[C14] 泛型函数
来源：http://qyv.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sae.kuanghao11.cn

PHP:  // 无泛型
来源：http://tob.zycfv.cn

JS:   // 无泛型
来源：http://gno.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ckc.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sgr.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ree.chenlongwang.top

Ruby: # 无泛型
来源：http://lwh.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ugj.andypj.xyz

[C15] 解构 / 展开参数
来源：http://ggs.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dfh.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://wap.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ozt.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ats.smart0.xyz

Java: // 无解构
来源：http://hjz.zdqjudy.top

Go:   // 无解构
来源：http://yvz.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://pcy.xinyue.icu

C#:   var (a, b) = pair;
来源：http://lbt.cashguo.top

[C16] 函数 / 方法重载
来源：http://ljz.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wxy.tarul.cn

PHP:  // 无重载
来源：http://pkm.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fay.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ydu.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsm.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://lsq.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://aqm.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nxz.hongshengwenyu.top

================================================================================
来源：http://rws.uphjek.com

D. 数组 / 列表 / 集合
来源：http://mqp.hongshengwenyu.top

================================================================================
来源：http://hhn.birdmap.top

[D01] 创建数组 / 列表
来源：http://iap.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mkl.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfo.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xhq.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hkx.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cjm.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://epa.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://yht.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://llw.xuanzx.com

[D02] 追加元素到末尾
来源：http://koq.yuxming.cn


<!-- 参考信息 -->