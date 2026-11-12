代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://wyk.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rox.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pqx.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://eqk.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://izn.shzxlz.cn

================================================================================
来源：http://rrv.hywenlv.cn

B. 流程控制
来源：http://pzz.hnxiangtu.top

================================================================================
来源：http://okt.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://oxi.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gvi.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bdi.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aht.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mqm.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://exr.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dlt.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hvc.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uga.tanke756.top

[B02] 多分支 else if / elif
来源：http://ilg.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://erj.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bks.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cph.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cnk.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvb.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uiy.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jrf.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cxn.meibo888.top

[B03] switch / match / case
来源：http://loe.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qky.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ycn.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mjk.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dgz.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pus.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pia.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hzm.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://izh.zdbjq.cn

[B04] for 计数循环
来源：http://cpd.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://wih.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://igk.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lxl.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cyj.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fny.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ydx.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://dtc.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dxe.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://jcr.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://nua.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ucc.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xbs.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dew.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://blg.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xse.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://lhv.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nyz.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://urn.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://akp.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mvp.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sda.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://azq.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zzg.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zva.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vna.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zrz.tarul.cn

[B07] while 循环
来源：http://ier.epnwcf.com

Py:   while i < 10: i += 1
来源：http://kkr.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://ukh.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://mud.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://eny.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://hnr.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ymf.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://wdp.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://ikn.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://eri.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://brw.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://flg.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://sue.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://rla.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://fqz.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wwj.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://dog.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://yor.daria6918.cn

[B09] break 与 continue
来源：http://bhu.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cmy.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cib.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aza.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ses.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogs.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jvg.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rof.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnu.nwbrower.top

[B10] 遍历同时拿索引
来源：http://uvu.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lis.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mww.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://csw.cheryme.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abc.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ahp.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://srr.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cuz.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lck.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://fhv.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://ovj.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://wsf.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aid.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eex.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzw.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dbk.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://whn.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zdj.zhoulong.xyz

[B12] 跳出多层循环
来源：http://rzn.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ayh.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://iia.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tku.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rjq.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nyt.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kzr.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://req.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://deu.cucudq.cn

[B13] 判断是否为数字
来源：http://jmy.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://zgp.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://gro.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mhs.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blb.jianghu66.top

Java: x instanceof Number
来源：http://oeg.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rqx.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://ogm.daria6918.cn

C#:   x is int or double or decimal
来源：http://lnh.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://nra.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kox.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hbx.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://hlv.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://wvx.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mdf.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wkh.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://nra.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cth.dashuyun.cn

[B15] 布尔运算与取反
来源：http://qkr.yuxming.cn

Py:   a and b or not c
来源：http://qmg.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://tve.uphjek.com

JS:   a && b || !c
来源：http://obf.shanyushiyangtech.top

TS:   a && b || !c
来源：http://lwl.hesvh.cn

Java: a && b || !c
来源：http://orb.yj20258.top

Go:   a && b || !c
来源：http://ebs.quarkkingdee.top

Ruby: a && b || !c
来源：http://god.cqqwz.cn

C#:   a && b || !c
来源：http://qcz.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://cqe.sjlbkw.cn

Py:   if not data: return
来源：http://rvh.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://niq.jinqigfzy.top

JS:   if (!data) return;
来源：http://rau.feifeiyinyue.top

TS:   if (!data) return;
来源：http://daj.tanke756.top

Java: if (data == null) return;
来源：http://pjo.xziqi.cn

Go:   if data == nil { return }
来源：http://jyi.chenzaomai.com

Ruby: return if data.nil?
来源：http://fca.sweek.top

C#:   if (data == null) return;
来源：http://qao.hnqzz.top

================================================================================
来源：http://kyf.hcnkem.com

C. 函数与作用域
来源：http://kzo.jinqigfzy.top

================================================================================
来源：http://qxl.yvedp.cn

[C01] 定义函数
来源：http://ofk.pycfn.com

Py:   def add(a, b): return a + b
来源：http://djt.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eat.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://jhw.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uif.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vba.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://hqq.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://rkl.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iar.c1oappe.top

[C02] 默认参数
来源：http://cph.meibo888.top

Py:   def greet(name="World"): return name
来源：http://tyx.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rxj.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://mvv.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://bnz.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://brg.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mjk.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://khu.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://rgk.sysykeji.top

[C03] 可变参数
来源：http://qqd.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://ull.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mrq.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://plw.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zth.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hng.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zey.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vvy.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tjh.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://jlj.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytb.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qbg.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bdy.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ibw.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://nmg.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://ssz.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://hsg.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://bjh.zhongyouzk.top

[C05] 返回多个值
来源：http://egb.jiagoushi.top

Py:   return a, b
来源：http://frz.zdbjq.cn

PHP:  return [$a, $b];
来源：http://wdd.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rnl.ppjwa.cn

TS:   return { a, b };
来源：http://jwy.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://off.yvedp.cn

Go:   return a, b
来源：http://thh.yuanzhike.top

Ruby: return a, b
来源：http://kny.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://vhe.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://vjb.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://kcy.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fhj.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://mzx.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://pbj.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://irk.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zhh.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://squ.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://nhn.xuanzx.com

[C07] 把函数作为参数传入
来源：http://lpi.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bds.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://xiv.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wrx.hywenlv.cn

TS:   arr.map(String)
来源：http://rlg.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mhy.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://onz.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://nmy.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mhh.c1oappe.top

[C08] 闭包
来源：http://cvn.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vof.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cwx.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gla.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tqs.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://smi.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hvk.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tay.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://csk.vehdjk.com

[C09] 递归
来源：http://dqh.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mkk.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cgc.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hhg.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttz.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://abu.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qvo.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bfi.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mxz.ctjpmb.com

[C10] 变量作用域
来源：http://otk.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gyi.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wnk.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://guw.ivvv.top

TS:   同 JS
来源：http://rns.cheryme.top

Java: 方法内为块级作用域
来源：http://ocg.dashuyun.cn

Go:   花括号块级作用域
来源：http://bmp.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hny.yanxiufei.cn

C#:   块级作用域
来源：http://nka.havefunace.top

[C11] 模块导入与导出
来源：http://tqx.cqqwz.cn

Py:   from module import func
来源：http://zco.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jhr.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://vyw.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lrb.meibo888.top

Java: import java.util.List;
来源：http://xfd.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqx.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://oeg.hywenlv.cn

C#:   using System.Text;
来源：http://lld.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://uon.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://hts.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://nhm.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://tbr.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://hbg.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gfc.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://jqz.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://nfk.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ibg.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://kad.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zay.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxg.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nxh.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qor.xinyue.icu

Java: int add(int a, int b) { return a + b; }
来源：http://mbz.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://psp.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://meq.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rty.hesvh.cn

[C14] 泛型函数
来源：http://hqy.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wgw.iojbl.cn

PHP:  // 无泛型
来源：http://wum.9152youxi.cn

JS:   // 无泛型
来源：http://lyv.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yct.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yoj.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://knd.cucudq.cn

Ruby: # 无泛型
来源：http://vcb.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipo.yuxming.cn

[C15] 解构 / 展开参数
来源：http://ahv.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wpx.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://ukc.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gxg.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vus.wangdashe.top

Java: // 无解构
来源：http://nwr.cheryme.top

Go:   // 无解构
来源：http://kli.cashguo.top

Ruby: a, b = pair
来源：http://vds.birdmap.top

C#:   var (a, b) = pair;
来源：http://jen.yvedp.cn

[C16] 函数 / 方法重载
来源：http://xcb.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://euk.jlsjyb.cn

PHP:  // 无重载
来源：http://vli.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mfc.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://eog.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://uyz.sweek.top

Go:   // 无重载：用不同函数名
来源：http://owy.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://aso.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cqb.ybcxt.top

================================================================================
来源：http://fim.hywenlv.cn


<!-- 参考信息 -->