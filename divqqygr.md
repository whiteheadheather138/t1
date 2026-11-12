代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dme.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tho.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kgt.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://evy.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://are.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://ayt.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fqb.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ziy.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sif.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxy.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fso.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vdz.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fms.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnr.svipenyu.cn

[B03] switch / match / case
来源：http://buj.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcq.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xdq.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqe.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fni.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bye.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mzj.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dlc.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://scv.uphjek.com

[B04] for 计数循环
来源：http://hxt.ivvv.top

Py:   for i in range(10): print(i)
来源：http://hpr.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kph.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fyr.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pko.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bdu.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fzy.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://nta.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hji.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://eeq.cashguo.top

Py:   for item in arr: print(item)
来源：http://bdw.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iuj.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://asl.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://spr.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pyo.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ixz.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://uir.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ctv.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://qah.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nku.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wtp.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zoq.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zjn.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hxe.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qku.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pyo.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cak.zhiwuduotai.top

[B07] while 循环
来源：http://mxb.yueranfly.top

Py:   while i < 10: i += 1
来源：http://uwc.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://lvo.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://bya.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://ivy.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://epq.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hzq.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://bfa.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://ygm.pycfn.com

[B08] do-while（至少执行一次）
来源：http://jxt.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://ypv.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://qjb.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://axt.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://mpy.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://cdl.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tvj.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://jmo.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://xda.fanxiaobao.xyz

[B09] break 与 continue
来源：http://wjf.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gtw.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sft.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkf.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjf.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsd.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jdn.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bos.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wys.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://kgo.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xjp.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blr.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tlf.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gja.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gjw.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dtp.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lrs.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jel.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://lye.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://nxh.yj20258.top

PHP:  range(0, 10, 2);
来源：http://ysc.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://njw.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rst.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lci.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opx.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://jel.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gel.cheryme.top

[B12] 跳出多层循环
来源：http://pdl.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wfl.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qjx.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpy.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hup.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ykv.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ffx.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pkt.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hyn.epnwcf.com

[B13] 判断是否为数字
来源：http://ujh.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://ozl.andypj.xyz

PHP:  is_numeric($x)
来源：http://wnw.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rot.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dyq.dianchejie.cn

Java: x instanceof Number
来源：http://wyc.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jqo.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://wit.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://wud.vehdjk.com

[B14] 判断值是否在集合内
来源：http://fqj.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://roj.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pon.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://hgm.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://hvr.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://exx.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cwa.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://agq.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fjr.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://muu.nanxuanxn.top

Py:   a and b or not c
来源：http://tts.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://zdg.wangshuangyany.cn

JS:   a && b || !c
来源：http://sqh.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://ilx.yanxiufei.cn

Java: a && b || !c
来源：http://gyk.pengpengdd.cyou

Go:   a && b || !c
来源：http://hqm.iojbl.cn

Ruby: a && b || !c
来源：http://icj.316326.xyz

C#:   a && b || !c
来源：http://ufq.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://kgy.zycfv.cn

Py:   if not data: return
来源：http://nqx.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://upk.chenjidiqi.icu

JS:   if (!data) return;
来源：http://for.dashuyun.cn

TS:   if (!data) return;
来源：http://nrr.xuetiantiany.cn

Java: if (data == null) return;
来源：http://tsr.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://oeo.yvedp.cn

Ruby: return if data.nil?
来源：http://ogg.yongpay.top

C#:   if (data == null) return;
来源：http://bhw.sjlbkw.cn

================================================================================
来源：http://soo.haohaochexian.top

C. 函数与作用域
来源：http://dka.dashuyun.cn

================================================================================
来源：http://iuu.hesvh.cn

[C01] 定义函数
来源：http://dic.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://nqs.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sem.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://ise.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymz.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wyw.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ayz.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://tjo.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://biz.havefunace.top

[C02] 默认参数
来源：http://vdf.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://ryc.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://axx.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://pnj.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ueb.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lzg.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://upu.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://tmb.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://amp.guowangkeji.top

[C03] 可变参数
来源：http://pnd.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://zim.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pni.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://npf.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://arb.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ldw.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bsc.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://xxd.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dcp.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://hgd.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cwm.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kew.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://out.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpq.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gsw.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://aev.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://mgx.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://axi.zhengqikj.top

[C05] 返回多个值
来源：http://wsh.cqqwz.cn

Py:   return a, b
来源：http://rif.gzhubu.top

PHP:  return [$a, $b];
来源：http://tmd.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://crs.hfpthk.cn

TS:   return { a, b };
来源：http://wbi.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://feo.ydzc1.top

Go:   return a, b
来源：http://okb.iojbl.cn

Ruby: return a, b
来源：http://eti.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://vpg.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://aqs.xinyue.icu

Py:   square = lambda x: x * x
来源：http://deu.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yea.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://lec.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://rdd.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wyu.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://pmr.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://qvl.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://nbm.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://pmo.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kcn.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mwq.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://seh.sjlbkw.cn

TS:   arr.map(String)
来源：http://cex.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ngh.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bwe.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://zxk.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gwi.gotoacloud.top

[C08] 闭包
来源：http://dqw.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gju.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zsi.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tnv.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jre.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bqf.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://amv.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gen.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iaz.andypj.xyz

[C09] 递归
来源：http://qym.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nrg.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yni.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hhr.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jss.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://emk.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rua.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjc.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jta.gzhubu.top

[C10] 变量作用域
来源：http://pdx.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fey.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://osj.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pgl.zhiwuduotai.top

TS:   同 JS
来源：http://ntr.tarul.cn

Java: 方法内为块级作用域
来源：http://zrq.nanxinkj.top

Go:   花括号块级作用域
来源：http://yzt.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://syw.xuanzx.com

C#:   块级作用域
来源：http://dav.ctjpmb.com

[C11] 模块导入与导出
来源：http://mrt.ppjwa.cn

Py:   from module import func
来源：http://cdx.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xps.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://thb.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jya.hongshengwenyu.top

Java: import java.util.List;
来源：http://eae.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vei.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://hbz.chenjidiqi.icu

C#:   using System.Text;
来源：http://grk.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://imi.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://jkh.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://gue.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://som.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://ffp.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fpf.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://rdt.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://ntv.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://pqy.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://bwp.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://icr.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehd.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tzo.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://trj.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://kla.zhixingplan.top

Go:   func add(a, b int) int
来源：http://rhr.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hdg.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://khr.xuanzx.com

[C14] 泛型函数
来源：http://gje.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qpz.bjfxy.top

PHP:  // 无泛型
来源：http://nur.aibaodan.cn

JS:   // 无泛型
来源：http://tek.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wvg.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jos.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmz.chenlongwang.top

Ruby: # 无泛型
来源：http://qrz.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ouj.vehdjk.com

[C15] 解构 / 展开参数
来源：http://hsd.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sgd.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://qef.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qwr.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kiu.smart0.xyz

Java: // 无解构
来源：http://nzn.yj20258888.top

Go:   // 无解构
来源：http://yep.ydjk.org.cn

Ruby: a, b = pair
来源：http://qeo.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://mnz.smart0.xyz

[C16] 函数 / 方法重载
来源：http://rkm.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wci.iojbl.cn

PHP:  // 无重载
来源：http://kjn.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hvy.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://met.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vlc.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://qpx.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://qfl.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vcu.chenzaomai.com

================================================================================
来源：http://bco.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://sat.nanxinkj.top

================================================================================
来源：http://uew.316326.xyz

[D01] 创建数组 / 列表
来源：http://yhq.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nrw.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aqd.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yho.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vyi.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tje.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://mox.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://vjw.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hja.316326.xyz

[D02] 追加元素到末尾
来源：http://myw.jqgfzy.top


<!-- 参考信息 -->