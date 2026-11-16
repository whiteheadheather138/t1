代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://lhk.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uik.daria6918.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zss.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vkb.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cds.fengsongda.top

================================================================================
来源：http://ssv.hnqzz.top

B. 流程控制
来源：http://jii.ivvv.top

================================================================================
来源：http://gnh.hcnkem.com

[B01] 条件判断 if / else
来源：http://cyf.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kdg.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afr.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nfq.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eku.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxp.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nab.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fet.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zph.xuetiantiany.cn

[B02] 多分支 else if / elif
来源：http://mnt.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qij.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hfy.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjo.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjc.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ttd.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tlo.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ska.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lyw.quarkkingdee.top

[B03] switch / match / case
来源：http://wfy.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pwc.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xdb.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jee.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qkh.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vrb.jqgfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gnn.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gex.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rdw.aizwys.cn

[B04] for 计数循环
来源：http://keo.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://hol.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zpl.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eni.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yyc.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gzs.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sxj.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://yue.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://htu.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://khe.fehbvm.com

Py:   for item in arr: print(item)
来源：http://nrn.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dza.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sqf.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ccp.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://foe.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zxl.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://sbe.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bft.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://pgd.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dbj.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://alm.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wya.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ner.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qug.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jtc.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lkq.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sam.jinyuanbaomall.cn

[B07] while 循环
来源：http://hoc.nwbrower.top

Py:   while i < 10: i += 1
来源：http://vun.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://fqt.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://tbh.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://fub.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://qik.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://edg.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://tka.sweek.top

C#:   while (i < 10) { i++; }
来源：http://msy.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://ffo.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://bfo.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mzj.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://pad.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://fun.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://ixn.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wpa.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://tjn.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://cup.ppjwa.cn

[B09] break 与 continue
来源：http://scw.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vil.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uhd.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovx.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zts.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ins.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://omn.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lzs.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xof.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://pyr.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eyt.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzh.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ksi.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mov.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zqe.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zgu.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kic.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rfw.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://mbb.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://hsm.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://dpe.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://atu.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckb.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wls.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xdv.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://zba.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qim.hammf.cn

[B12] 跳出多层循环
来源：http://zgl.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xty.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yhr.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ycw.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfc.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kqs.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dvy.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xvt.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gua.quarkkingdee.top

[B13] 判断是否为数字
来源：http://hvy.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://hnm.aibaodan.cn

PHP:  is_numeric($x)
来源：http://dan.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rsq.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rbv.vqdsnc.cn

Java: x instanceof Number
来源：http://sxu.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pau.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://pci.guannengcc.top

C#:   x is int or double or decimal
来源：http://dbl.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://inz.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nux.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rxm.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://qzj.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://acs.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sfh.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fmj.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://hlp.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tgm.yuanzhike.top

[B15] 布尔运算与取反
来源：http://uyl.yj20258888.top

Py:   a and b or not c
来源：http://tei.bbcook.cn

PHP:  $a && $b || !$c
来源：http://jcf.daria6918.cn

JS:   a && b || !c
来源：http://fhx.jinqigfzy.top

TS:   a && b || !c
来源：http://ico.haohaochexian.top

Java: a && b || !c
来源：http://lto.guannengcc.top

Go:   a && b || !c
来源：http://bcd.birdmap.top

Ruby: a && b || !c
来源：http://ntz.haohaochexian.top

C#:   a && b || !c
来源：http://tsf.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://skp.bjfxy.top

Py:   if not data: return
来源：http://qgu.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://jrl.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://bls.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://ouv.hywenlv.cn

Java: if (data == null) return;
来源：http://pjn.yuxming.cn

Go:   if data == nil { return }
来源：http://rzj.gotoacloud.top

Ruby: return if data.nil?
来源：http://rfy.gotoacloud.top

C#:   if (data == null) return;
来源：http://mkb.ehwqpu.com

================================================================================
来源：http://fqt.c1oappe.top

C. 函数与作用域
来源：http://iqc.ybcxt.top

================================================================================
来源：http://tdd.zhijiandao.cn

[C01] 定义函数
来源：http://dio.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://nlf.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ape.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://utb.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gvr.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ull.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kwb.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://inj.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eaz.guannengcc.top

[C02] 默认参数
来源：http://rfy.yj20258.top

Py:   def greet(name="World"): return name
来源：http://oqv.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gdp.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://zha.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nsw.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vzn.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjr.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://ihq.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://mxz.uphjek.com

[C03] 可变参数
来源：http://vax.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://bdo.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kag.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oom.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://org.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ldu.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jko.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cld.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://puh.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://fpn.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ued.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbk.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ozg.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gio.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://pts.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://uyj.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://zzx.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://xhb.hammf.cn

[C05] 返回多个值
来源：http://api.havefunace.top

Py:   return a, b
来源：http://kjp.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://mre.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://irc.cdnleiting.top

TS:   return { a, b };
来源：http://zyu.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rdu.zhixingplan.top

Go:   return a, b
来源：http://wjt.yj202588.top

Ruby: return a, b
来源：http://ccp.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://ulx.yj20258.top

[C06] 匿名函数 / lambda
来源：http://pek.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://zsy.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iwp.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://kqm.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://pzy.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eeo.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://dxz.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://ozx.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://dsn.shuidangran.top

[C07] 把函数作为参数传入
来源：http://hda.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://acl.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://hqn.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gdy.yongpay.top

TS:   arr.map(String)
来源：http://gac.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://phk.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cbo.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://hhl.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dyt.0kj1m.cn

[C08] 闭包
来源：http://itn.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nyi.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qkh.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jyd.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ibl.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ybj.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ijo.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xwg.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ndy.chenlongwang.top

[C09] 递归
来源：http://tmo.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ths.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gsz.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlo.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urt.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ven.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rsv.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kyw.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ffh.ydjk.org.cn

[C10] 变量作用域
来源：http://wkh.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zec.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmo.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iml.zhaomingkeji.xyz

TS:   同 JS
来源：http://uem.xylfe.cn

Java: 方法内为块级作用域
来源：http://aqq.zhixingplan.top

Go:   花括号块级作用域
来源：http://pat.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nln.shangyingyoupin.top

C#:   块级作用域
来源：http://xfo.zhixingplan.top

[C11] 模块导入与导出
来源：http://pqq.52xcode.cn

Py:   from module import func
来源：http://aar.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qth.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://luo.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dph.shuidangran.top

Java: import java.util.List;
来源：http://jhs.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://efz.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://usg.wangdashe.top

C#:   using System.Text;
来源：http://jfx.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://hmw.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://kgm.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://skr.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://lxp.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://tsf.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iin.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://ern.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://ofx.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tlj.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://cej.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rjp.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tno.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rkk.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jsa.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uoo.9152youxi.cn

Go:   func add(a, b int) int
来源：http://tzj.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rcr.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vch.yangfankeji.com

[C14] 泛型函数
来源：http://emu.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efh.zhongyouzk.top

PHP:  // 无泛型
来源：http://ybf.xuanzx.com

JS:   // 无泛型
来源：http://edg.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://azt.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://chh.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wtd.redwolf501.top

Ruby: # 无泛型
来源：http://wvq.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyk.hnqzz.top

[C15] 解构 / 展开参数
来源：http://bgw.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qea.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://iiw.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wby.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hln.xuetiantiany.cn

Java: // 无解构
来源：http://vun.smart0.xyz

Go:   // 无解构
来源：http://smo.wangdashe.top

Ruby: a, b = pair
来源：http://mhv.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://vgx.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://nzx.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://szx.hfpthk.cn

PHP:  // 无重载
来源：http://lnl.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zdv.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://clt.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qhs.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://kts.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://fnj.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pem.cqqwz.cn

================================================================================
来源：http://adq.hywenlv.cn


<!-- 参考信息 -->