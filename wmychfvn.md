代发 wailian999

[B01] 条件判断 if / else
来源：http://wzl.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kjp.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fkz.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://smx.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bfu.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ood.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pnt.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tnx.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bjo.sxryk.cn

[B02] 多分支 else if / elif
来源：http://gig.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://evk.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qcn.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvt.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyv.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgf.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hta.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hrn.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aaj.daria6918.cn

[B03] switch / match / case
来源：http://bgh.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rfv.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://shy.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wud.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqm.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ndj.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bem.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bzz.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://owv.pengpengdd.cyou

[B04] for 计数循环
来源：http://uym.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://gaa.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nwt.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bme.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uze.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qom.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ego.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://oqw.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hec.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://isv.birdmap.top

Py:   for item in arr: print(item)
来源：http://enh.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yzz.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://blh.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lvm.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fpx.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hdf.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://xpu.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pox.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://giu.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://upz.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uid.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mrd.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgz.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hqz.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hgs.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://got.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wsa.hysaishi.cn

[B07] while 循环
来源：http://guj.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://ekc.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://kwb.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://grx.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://emr.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://sws.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tsn.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://rov.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://pxp.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://oou.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://uwb.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xgm.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://tkq.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://dsm.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://mxi.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iye.tanke756.top

Ruby: begin; i += 1; end while i < 10
来源：http://iqe.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://njb.andypj.xyz

[B09] break 与 continue
来源：http://nyk.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qut.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vtk.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igh.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrj.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmb.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xzh.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aea.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbs.daria6918.cn

[B10] 遍历同时拿索引
来源：http://stp.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fes.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bja.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yuk.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fxh.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cki.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://imm.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugp.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://imt.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://bhu.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://iiq.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://biq.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://csg.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hxe.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mhf.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yop.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://ygj.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tls.bbcook.cn

[B12] 跳出多层循环
来源：http://kdm.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ulp.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://azj.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mqs.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhm.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rgd.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gnd.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ugu.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxi.hfpthk.cn

[B13] 判断是否为数字
来源：http://iya.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://roc.tanke756.top

PHP:  is_numeric($x)
来源：http://ubv.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuw.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdv.jyoumei.cn

Java: x instanceof Number
来源：http://hwy.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zqm.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://jdj.epnwcf.com

C#:   x is int or double or decimal
来源：http://fjr.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://dyb.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://doj.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ucq.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://cit.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://ncj.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mhv.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qtp.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cjs.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twt.ppjwa.cn

[B15] 布尔运算与取反
来源：http://bsd.hysaishi.cn

Py:   a and b or not c
来源：http://lid.cucudq.cn

PHP:  $a && $b || !$c
来源：http://gfw.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://uaa.cqqwz.cn

TS:   a && b || !c
来源：http://tkf.hcnkem.com

Java: a && b || !c
来源：http://bjs.fzhhl.top

Go:   a && b || !c
来源：http://amp.xuetiantiany.cn

Ruby: a && b || !c
来源：http://hns.kuanghao11.cn

C#:   a && b || !c
来源：http://bxm.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://leg.shzxlz.cn

Py:   if not data: return
来源：http://yap.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://wvd.daxiang520.top

JS:   if (!data) return;
来源：http://ard.yuxming.cn

TS:   if (!data) return;
来源：http://aqv.quarkkingdee.top

Java: if (data == null) return;
来源：http://gkg.hysaishi.cn

Go:   if data == nil { return }
来源：http://san.jinqigufen.top

Ruby: return if data.nil?
来源：http://vce.hnxiangtu.top

C#:   if (data == null) return;
来源：http://mnx.birdmap.top

================================================================================
来源：http://qni.gzhubu.top

C. 函数与作用域
来源：http://oej.jinyuanbaomall.cn

================================================================================
来源：http://msc.snrcjt.cn

[C01] 定义函数
来源：http://arg.uphjek.com

Py:   def add(a, b): return a + b
来源：http://pig.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkk.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://exk.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://alq.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nne.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://bvg.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://txd.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uoy.cheryme.top

[C02] 默认参数
来源：http://rdg.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://zyg.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zhn.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://hza.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iah.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zql.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vte.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://kus.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://jkb.yfazqb.com

[C03] 可变参数
来源：http://nue.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://ntv.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pcd.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vkd.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vqh.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gbr.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tda.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xiu.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://huw.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://xdd.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://faj.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gkd.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://phu.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rui.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://uot.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://fag.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://crl.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://tfw.kuanghao11.cn

[C05] 返回多个值
来源：http://bdb.cucudq.cn

Py:   return a, b
来源：http://nfp.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://zpq.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tcg.meibo888.top

TS:   return { a, b };
来源：http://usi.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://olb.zhaomingkeji.xyz

Go:   return a, b
来源：http://san.smart0.xyz

Ruby: return a, b
来源：http://wrj.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://ypu.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://nzs.andypj.xyz

Py:   square = lambda x: x * x
来源：http://lnr.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rgt.ivvv.top

JS:   const square = x => x * x;
来源：http://ynk.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://wcf.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://anu.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://cnu.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://zdj.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://qdi.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://wjd.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fsg.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xxp.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xnb.jyoumei.cn

TS:   arr.map(String)
来源：http://dhk.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ube.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rvs.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://fca.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://gya.cucudq.cn

[C08] 闭包
来源：http://ucw.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kjp.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fkw.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gym.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://imb.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzw.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzy.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uhl.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ija.chenzaomai.com

[C09] 递归
来源：http://ksv.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fex.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpf.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pge.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wpn.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ynr.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vyt.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qoq.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eaa.tianlin.xyz

[C10] 变量作用域
来源：http://xvb.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gsv.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qpi.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gjx.guowangkeji.top

TS:   同 JS
来源：http://fzd.yvedp.cn

Java: 方法内为块级作用域
来源：http://jgq.vehdjk.com

Go:   花括号块级作用域
来源：http://hto.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zmr.epnwcf.com

C#:   块级作用域
来源：http://szd.ydjk.org.cn

[C11] 模块导入与导出
来源：http://gdm.hcnkem.com

Py:   from module import func
来源：http://isu.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xhd.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eyk.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xxx.kuanghao11.cn

Java: import java.util.List;
来源：http://tpt.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogk.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://zrw.yvedp.cn

C#:   using System.Text;
来源：http://cvu.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://qcb.yj202588.top

Py:   (lambda: print("run"))()
来源：http://bej.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://xgv.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://yav.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://tci.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mjs.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://gwi.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://wox.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://wng.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://uhx.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xxa.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rwr.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wfx.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgk.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://hqn.hcnkem.com

Go:   func add(a, b int) int
来源：http://beb.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wev.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://img.xuetiantiany.cn

[C14] 泛型函数
来源：http://ehb.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://byg.316326.xyz

PHP:  // 无泛型
来源：http://cmv.jinqigfzy.top

JS:   // 无泛型
来源：http://wra.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lqa.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rko.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://smp.0kj1m.cn

Ruby: # 无泛型
来源：http://mhv.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zxu.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://wpf.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lko.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://pxo.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hfp.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sdp.zhixingplan.top

Java: // 无解构
来源：http://xtu.nwbrower.top

Go:   // 无解构
来源：http://pjg.guannengcc.top

Ruby: a, b = pair
来源：http://asc.cashguo.top

C#:   var (a, b) = pair;
来源：http://jgy.yfazqb.com

[C16] 函数 / 方法重载
来源：http://dcc.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://akv.cucudq.cn

PHP:  // 无重载
来源：http://bzs.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jda.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://kpo.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jef.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://avc.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://jlx.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zyx.jiagoushi.top

================================================================================
来源：http://wtr.pycfn.com

D. 数组 / 列表 / 集合
来源：http://uqe.xuanzx.com

================================================================================
来源：http://ydh.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://krb.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vud.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ucq.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ebg.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yro.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dtl.jinghuilouyu.cn


<!-- 参考信息 -->