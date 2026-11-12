代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhj.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://msa.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mdz.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vbx.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rew.ybcxt.top

[B02] 多分支 else if / elif
来源：http://bod.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mbs.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dro.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjh.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khz.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gso.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpd.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iks.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dct.andypj.xyz

[B03] switch / match / case
来源：http://vpk.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcq.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbq.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wjc.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrr.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pfm.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ehj.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vlo.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://unh.haohaochexian.top

[B04] for 计数循环
来源：http://tbf.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://nje.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://odh.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ltm.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ybl.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwj.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://szu.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://qmm.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ncn.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://lkq.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://wln.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pzq.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nhy.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://osq.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oal.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://obf.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://ftq.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lje.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://uto.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xie.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xal.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnc.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qzw.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://syf.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ljc.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wtc.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pem.shangyingyoupin.top

[B07] while 循环
来源：http://tjq.zycfv.cn

Py:   while i < 10: i += 1
来源：http://oox.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zoy.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://azs.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://fjp.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://vhe.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kat.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://ddg.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://zcv.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://xzn.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://tki.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gjq.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://tpi.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://yib.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://xuv.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://whj.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pxv.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://szb.hfpthk.cn

[B09] break 与 continue
来源：http://bpv.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vxw.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ppv.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmn.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoi.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lay.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kmo.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ehe.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbd.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://sxw.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uhr.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ksc.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://byi.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ywg.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wdg.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fwx.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eue.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uif.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://kka.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://zoc.hammf.cn

PHP:  range(0, 10, 2);
来源：http://rip.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cks.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayc.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lal.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pjz.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://wnb.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lhi.cqqwz.cn

[B12] 跳出多层循环
来源：http://tue.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mtc.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ahr.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzi.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwx.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bbe.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ylz.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cve.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ira.jinqigfzy.top

[B13] 判断是否为数字
来源：http://tsz.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://kdi.cdnleiting.top

PHP:  is_numeric($x)
来源：http://yip.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://upw.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ejg.jiagoushi.top

Java: x instanceof Number
来源：http://osq.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mkx.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://ens.daria6918.cn

C#:   x is int or double or decimal
来源：http://kbu.hcnkem.com

[B14] 判断值是否在集合内
来源：http://cxz.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pbt.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rvk.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://sys.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://bvx.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hwt.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abr.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://qaf.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swt.ctjpmb.com

[B15] 布尔运算与取反
来源：http://jjr.ctjpmb.com

Py:   a and b or not c
来源：http://pwd.xinyue.icu

PHP:  $a && $b || !$c
来源：http://vtq.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://nqa.jqgufenzy.top

TS:   a && b || !c
来源：http://xmt.havefunace.top

Java: a && b || !c
来源：http://wak.andypj.xyz

Go:   a && b || !c
来源：http://yoa.yanxiufei.cn

Ruby: a && b || !c
来源：http://nxz.tarul.cn

C#:   a && b || !c
来源：http://fhq.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://omi.ydzc1.top

Py:   if not data: return
来源：http://nvv.cashguo.top

PHP:  if (!$data) { return; }
来源：http://njw.hnxiangtu.top

JS:   if (!data) return;
来源：http://spa.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://vam.iojbl.cn

Java: if (data == null) return;
来源：http://azn.fktsv.cn

Go:   if data == nil { return }
来源：http://dxg.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://ozz.redwolf501.top

C#:   if (data == null) return;
来源：http://viy.c1oappe.top

================================================================================
来源：http://hsy.smart0.xyz

C. 函数与作用域
来源：http://tzq.yonumen.top

================================================================================
来源：http://vol.jyoumei.cn

[C01] 定义函数
来源：http://apb.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://eqj.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ott.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://rvo.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqh.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lkf.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mss.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://bmt.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zjs.aizwys.cn

[C02] 默认参数
来源：http://qgk.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://myd.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nfj.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://fvt.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dqb.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vib.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ibv.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://mmq.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://kxy.epnwcf.com

[C03] 可变参数
来源：http://bdj.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://ttn.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iyj.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rzh.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rnv.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iig.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lzj.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xav.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yve.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://xmr.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bgd.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://akv.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zeb.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uln.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://dyj.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://kjx.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://rmy.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://atv.haohaochexian.top

[C05] 返回多个值
来源：http://szj.zhijiandao.cn

Py:   return a, b
来源：http://xpw.yvedp.cn

PHP:  return [$a, $b];
来源：http://qhj.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zkw.bbcook.cn

TS:   return { a, b };
来源：http://ilb.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bma.yvedp.cn

Go:   return a, b
来源：http://gvx.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://pfu.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://hmj.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://gvf.c1oappe.top

Py:   square = lambda x: x * x
来源：http://juz.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://fdm.hfpthk.cn

JS:   const square = x => x * x;
来源：http://rpp.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://lqm.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gwb.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://ebd.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://qvw.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://xor.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://ftv.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cms.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://ccv.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xgo.sysykeji.top

TS:   arr.map(String)
来源：http://tcm.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rxj.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cnp.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://igh.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lhm.uphjek.com

[C08] 闭包
来源：http://upf.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://azf.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fcf.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eli.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mhv.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vri.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://neg.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://syx.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zdd.mhx1999.top

[C09] 递归
来源：http://ert.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fcb.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://myw.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vbg.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tps.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vrn.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xsc.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbw.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qtj.316326.xyz

[C10] 变量作用域
来源：http://dze.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qmj.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sjj.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nmq.xuetiantiany.cn

TS:   同 JS
来源：http://muj.ydzc1.top

Java: 方法内为块级作用域
来源：http://foc.jyoumei.cn

Go:   花括号块级作用域
来源：http://cxn.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gol.0kj1m.cn

C#:   块级作用域
来源：http://lwj.daxiang520.top

[C11] 模块导入与导出
来源：http://try.shanyushiyangtech.top

Py:   from module import func
来源：http://yls.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bhh.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdo.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pfl.bbcook.cn

Java: import java.util.List;
来源：http://tgo.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uiv.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://pzr.ppjwa.cn

C#:   using System.Text;
来源：http://rww.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://nsx.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://dbe.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://dfi.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://deq.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://jum.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pqa.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ple.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://sro.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://shw.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://ksb.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fnh.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wdw.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mhw.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vho.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://dpw.mhx1999.top

Go:   func add(a, b int) int
来源：http://yvk.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qbh.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://mgx.yj202588.top

[C14] 泛型函数
来源：http://imt.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cuo.9152youxi.cn

PHP:  // 无泛型
来源：http://izd.fanxiaobao.xyz

JS:   // 无泛型
来源：http://zpf.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://udz.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gif.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bmo.zdqjudy.top

Ruby: # 无泛型
来源：http://dvi.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdj.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://asm.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tkr.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://lci.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwc.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mul.fengsongda.top

Java: // 无解构
来源：http://bcc.zhongyouzk.top

Go:   // 无解构
来源：http://oyi.c1oappe.top

Ruby: a, b = pair
来源：http://tmj.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://rup.daxiang520.top

[C16] 函数 / 方法重载
来源：http://pam.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zss.fzhhl.top

PHP:  // 无重载
来源：http://ywd.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wne.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://gum.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gbm.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://fec.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://nyc.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fue.daria6918.cn

================================================================================
来源：http://mja.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://yil.redwolf501.top

================================================================================
来源：http://pqg.iojbl.cn

[D01] 创建数组 / 列表
来源：http://csk.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pqc.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://svq.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pcs.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lst.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://exx.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://ven.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://pmd.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rlf.jianghu66.top

[D02] 追加元素到末尾
来源：http://rwn.yfazqb.com


<!-- 参考信息 -->