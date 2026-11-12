代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tbz.fktsv.cn

================================================================================
来源：http://kax.xylfe.cn

B. 流程控制
来源：http://xrw.birdmap.top

================================================================================
来源：http://jhh.sxryk.cn

[B01] 条件判断 if / else
来源：http://kxi.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zfz.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dzt.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jei.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sve.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vfs.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sqh.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xmk.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bhn.bbcook.cn

[B02] 多分支 else if / elif
来源：http://use.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vaw.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ruh.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mij.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pym.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cer.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vyn.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nxj.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyd.sjlbkw.cn

[B03] switch / match / case
来源：http://lgz.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sjk.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aam.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ork.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://agy.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qwg.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rnr.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://deu.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rmg.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://ywx.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://ihk.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wxo.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtw.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://twe.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eof.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yvg.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://egx.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cas.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://mqp.tanke756.top

Py:   for item in arr: print(item)
来源：http://svk.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hor.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gyr.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://prw.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wyj.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kol.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://fsk.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eop.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://jps.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ysi.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kkb.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ynt.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhs.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ynj.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jvf.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vyv.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oio.ctjpmb.com

[B07] while 循环
来源：http://jjp.yj20258.top

Py:   while i < 10: i += 1
来源：http://qio.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://egh.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ybc.quarkkingdee.top

TS:   while (i < 10) { i++; }
来源：http://srz.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://uwi.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eyb.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://mvx.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://oei.meibo888.top

[B08] do-while（至少执行一次）
来源：http://ajh.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://lbo.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yuv.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://cmc.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://heg.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://ztj.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ben.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://cff.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://iyw.gzhubu.top

[B09] break 与 continue
来源：http://krt.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ntd.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mru.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qth.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lig.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjd.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uyt.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vzu.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llk.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://niv.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://znj.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fno.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qpl.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dkv.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sfh.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dpj.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qjy.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lzb.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://kfy.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://ijy.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://ioo.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uwy.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwq.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ngq.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zsi.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://gnk.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vnp.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://pny.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ddi.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpm.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ttd.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aus.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oyk.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://odw.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://upy.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uqm.ydjk.org.cn

[B13] 判断是否为数字
来源：http://unl.hfpthk.cn

Py:   isinstance(x, (int, float))
来源：http://fgy.gotoacloud.top

PHP:  is_numeric($x)
来源：http://nvt.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bku.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mce.yueranfly.top

Java: x instanceof Number
来源：http://gig.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqs.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://clu.sxryk.cn

C#:   x is int or double or decimal
来源：http://zat.sysykeji.top

[B14] 判断值是否在集合内
来源：http://efx.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vof.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yrz.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://jyn.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://lvb.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qtl.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mai.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://bhv.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jtc.meibo888.top

[B15] 布尔运算与取反
来源：http://map.fzhhl.top

Py:   a and b or not c
来源：http://mxf.birdmap.top

PHP:  $a && $b || !$c
来源：http://uvc.hesvh.cn

JS:   a && b || !c
来源：http://wup.andypj.xyz

TS:   a && b || !c
来源：http://tmp.ehwqpu.com

Java: a && b || !c
来源：http://jtu.yanxiufei.cn

Go:   a && b || !c
来源：http://wls.cucudq.cn

Ruby: a && b || !c
来源：http://hry.hysaishi.cn

C#:   a && b || !c
来源：http://bvv.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://rva.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://yhc.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://eud.hfpthk.cn

JS:   if (!data) return;
来源：http://teo.316326.xyz

TS:   if (!data) return;
来源：http://roi.c1oappe.top

Java: if (data == null) return;
来源：http://pqu.xziqi.cn

Go:   if data == nil { return }
来源：http://bgi.zhixingplan.top

Ruby: return if data.nil?
来源：http://cmu.gotoacloud.top

C#:   if (data == null) return;
来源：http://jto.cashguo.top

================================================================================
来源：http://ehj.daria6918.cn

C. 函数与作用域
来源：http://lvm.dashuyun.cn

================================================================================
来源：http://bci.shanyushiyangkeji.top

[C01] 定义函数
来源：http://wpu.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://pzl.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zpy.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://yen.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vop.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kbr.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://rbd.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://dae.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nlh.havefunace.top

[C02] 默认参数
来源：http://ppa.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://idy.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hgx.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://gzu.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fsi.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zgf.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ric.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://qdl.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://wko.birdmap.top

[C03] 可变参数
来源：http://tcg.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://tzh.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jma.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pku.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cbh.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vqq.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szr.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://crm.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bpi.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://lic.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kdb.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cyq.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mlo.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kfj.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://ltw.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://qwt.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://rjk.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://gik.vqdsnc.cn

[C05] 返回多个值
来源：http://mdw.tarul.cn

Py:   return a, b
来源：http://jrc.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://lfs.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uvr.tianlin.xyz

TS:   return { a, b };
来源：http://zsy.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://svr.hongshengwenyu.top

Go:   return a, b
来源：http://vzf.iojbl.cn

Ruby: return a, b
来源：http://foe.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://zmi.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://cwx.smart0.xyz

Py:   square = lambda x: x * x
来源：http://ehk.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://idd.yuanzhike.top

JS:   const square = x => x * x;
来源：http://vom.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://yvv.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zdj.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rze.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://ctb.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hak.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://gdl.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ijw.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rew.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wer.jqgfzy.top

TS:   arr.map(String)
来源：http://dfh.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vov.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bup.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://xhh.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qcn.zhongyouzk.top

[C08] 闭包
来源：http://rjh.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfw.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wgp.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ggb.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dlx.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mdi.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iad.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://idr.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pff.wangdashe.top

[C09] 递归
来源：http://xkk.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pan.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ofy.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qqr.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lia.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iap.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qcq.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xvk.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://obz.wangshuangyany.cn

[C10] 变量作用域
来源：http://ecq.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pcg.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://moo.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jxm.redwolf501.top

TS:   同 JS
来源：http://ons.jianghu66.top

Java: 方法内为块级作用域
来源：http://rzh.yonumen.top

Go:   花括号块级作用域
来源：http://gpj.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yok.gaohongyu789.top

C#:   块级作用域
来源：http://moa.quarkkingdee.top

[C11] 模块导入与导出
来源：http://yqz.hnqzz.top

Py:   from module import func
来源：http://twu.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://lpr.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdn.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hcl.zhengqikj.top

Java: import java.util.List;
来源：http://oqn.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcx.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://nyy.yonumen.top

C#:   using System.Text;
来源：http://kzq.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://irb.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://yqf.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://dbk.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://pcx.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://thx.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://abf.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://xee.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://whl.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ucp.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://hjg.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dxm.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yme.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rwb.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://utr.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://caj.smart0.xyz

Go:   func add(a, b int) int
来源：http://cbd.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yfr.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://mbp.gotoacloud.top

[C14] 泛型函数
来源：http://uwb.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vlq.shuidangran.top

PHP:  // 无泛型
来源：http://syu.yueranfly.top

JS:   // 无泛型
来源：http://yld.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sai.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uuj.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cvb.chenlongwang.top

Ruby: # 无泛型
来源：http://eln.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fun.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://iap.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pcm.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://wda.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hvc.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dsl.tian-w.cn

Java: // 无解构
来源：http://xhq.hfpthk.cn

Go:   // 无解构
来源：http://wxm.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://yyr.birdmap.top

C#:   var (a, b) = pair;
来源：http://kxv.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://ozw.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yej.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://lug.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://rye.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://ejt.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://glq.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://fod.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://fsx.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ttv.fanxiaobao.xyz

================================================================================
来源：http://iva.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://lxo.xuanzx.com

================================================================================
来源：http://day.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://ifg.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ile.aibaodan.cn


<!-- 参考信息 -->