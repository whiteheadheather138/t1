代发 wailian999

[B01] 条件判断 if / else
来源：http://nlm.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://vre.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mqj.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rjo.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ymv.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://smm.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fyf.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fdq.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nvo.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://eyo.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yfb.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vjv.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkw.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzm.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jlq.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vqv.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xct.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfp.haohaochexian.top

[B03] switch / match / case
来源：http://jdk.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://orh.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zdg.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ptp.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bli.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ubi.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hyz.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cji.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hrc.chenzaomai.com

[B04] for 计数循环
来源：http://amn.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://zap.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cmt.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qzu.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uks.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qqp.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gym.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://yds.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yve.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://uzv.tanke756.top

Py:   for item in arr: print(item)
来源：http://abb.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vvc.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mks.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rwq.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://chb.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cvk.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://bkf.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oby.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://tlr.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://plj.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://roi.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://omd.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxt.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qdw.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rxz.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hnv.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gio.sxryk.cn

[B07] while 循环
来源：http://iuw.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://pvf.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://usy.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://vmp.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://ztb.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://tlk.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://svf.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://ubz.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://oaw.xziqi.cn

[B08] do-while（至少执行一次）
来源：http://vje.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://rzm.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://omc.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://qoi.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://nac.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://cqo.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://loo.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://xkg.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://dsp.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://cjn.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qjy.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lpm.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icd.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lwn.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yeh.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kqv.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gam.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbw.52xcode.cn

[B10] 遍历同时拿索引
来源：http://aby.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://loj.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tbc.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rzy.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xzb.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cnb.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://flx.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://icx.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://npl.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://brh.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://cfz.yj202588.top

PHP:  range(0, 10, 2);
来源：http://sqe.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dap.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kmn.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xqa.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://esp.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://pzh.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pji.sweek.top

[B12] 跳出多层循环
来源：http://fcv.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://esz.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://yxl.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xle.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xpw.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fvk.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qkl.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jdj.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iiz.chenlongwang.top

[B13] 判断是否为数字
来源：http://cbt.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://bjw.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://tfy.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tou.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lsa.xziqi.cn

Java: x instanceof Number
来源：http://hbg.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://syx.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://ibh.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://zcq.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://qih.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wif.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jtg.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gns.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://kdx.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eok.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oru.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ywr.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ejk.52xcode.cn

[B15] 布尔运算与取反
来源：http://xyz.shanyushiyangtech.top

Py:   a and b or not c
来源：http://cgg.vehdjk.com

PHP:  $a && $b || !$c
来源：http://fcx.quarkkingdee.top

JS:   a && b || !c
来源：http://uxs.redwolf501.top

TS:   a && b || !c
来源：http://ulg.yvedp.cn

Java: a && b || !c
来源：http://igd.yangfankeji.com

Go:   a && b || !c
来源：http://ljq.jyoumei.cn

Ruby: a && b || !c
来源：http://ezv.yfazqb.com

C#:   a && b || !c
来源：http://bef.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fdp.shangyingyoupin.top

Py:   if not data: return
来源：http://doe.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://cvc.andypj.xyz

JS:   if (!data) return;
来源：http://crb.epnwcf.com

TS:   if (!data) return;
来源：http://hsr.yongpay.top

Java: if (data == null) return;
来源：http://jnj.dashuyun.cn

Go:   if data == nil { return }
来源：http://pgd.cqqwz.cn

Ruby: return if data.nil?
来源：http://fno.hesvh.cn

C#:   if (data == null) return;
来源：http://nwo.jlsjyb.cn

================================================================================
来源：http://ujs.zhiwuduotai.top

C. 函数与作用域
来源：http://xhq.fanxiaobao.xyz

================================================================================
来源：http://jwd.jiagoushi.top

[C01] 定义函数
来源：http://wad.meibo888.top

Py:   def add(a, b): return a + b
来源：http://udr.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rnd.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://trg.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://orv.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://dkm.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://qyf.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://tyr.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gla.fengsongda.top

[C02] 默认参数
来源：http://wvz.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://gbd.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://jyx.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://trx.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hgk.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pxy.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wjr.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://ley.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://duw.havefunace.top

[C03] 可变参数
来源：http://qpc.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://yqq.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bsb.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yph.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lgu.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://irt.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zpj.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://dqc.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://opz.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://jwh.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eee.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hta.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hqm.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gyt.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://zvm.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://zcu.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://wph.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://tec.jyoumei.cn

[C05] 返回多个值
来源：http://hhr.sjlbkw.cn

Py:   return a, b
来源：http://uau.xziqi.cn

PHP:  return [$a, $b];
来源：http://age.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fpx.nwbrower.top

TS:   return { a, b };
来源：http://poi.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://omr.jqgufenzy.top

Go:   return a, b
来源：http://ijf.zhengqikj.top

Ruby: return a, b
来源：http://kkp.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://lzr.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://ejn.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://xtd.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wlz.bbcook.cn

JS:   const square = x => x * x;
来源：http://hbz.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://hqo.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bxj.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://wiw.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://usr.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://mbi.yj20258888.top

[C07] 把函数作为参数传入
来源：http://ngw.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tmu.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://ulx.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yoy.hammf.cn

TS:   arr.map(String)
来源：http://env.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bwh.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rwu.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://xhd.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qfx.wangshuangyany.cn

[C08] 闭包
来源：http://uqf.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yxx.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tyw.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ely.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kqf.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://now.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rne.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rtc.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jvv.0kj1m.cn

[C09] 递归
来源：http://vhd.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mnk.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://djt.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nep.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvc.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dgu.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rrv.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cen.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fcv.shzxlz.cn

[C10] 变量作用域
来源：http://upi.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fic.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eqx.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tpf.ivvv.top

TS:   同 JS
来源：http://tlw.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://cef.shzxlz.cn

Go:   花括号块级作用域
来源：http://dix.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nnb.9152youxi.cn

C#:   块级作用域
来源：http://xnk.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://lla.jqgfzy.top

Py:   from module import func
来源：http://itr.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vcf.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wsg.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vtf.hysaishi.cn

Java: import java.util.List;
来源：http://klo.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ehe.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://ytv.fktsv.cn

C#:   using System.Text;
来源：http://ddx.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://uao.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://dhs.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://swn.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://twy.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://gtf.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlf.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://kiu.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://hbu.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wyq.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://rgl.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pbp.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mlf.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sqv.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axd.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://yos.birdmap.top

Go:   func add(a, b int) int
来源：http://xaw.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qni.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gjo.yfazqb.com

[C14] 泛型函数
来源：http://pwu.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkz.wangshuangyany.cn

PHP:  // 无泛型
来源：http://mxu.hcnkem.com

JS:   // 无泛型
来源：http://uzf.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bpn.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kxu.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://web.yj20258888.top

Ruby: # 无泛型
来源：http://kuo.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fmc.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://xhi.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvr.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://zpz.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://afe.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wow.smart0.xyz

Java: // 无解构
来源：http://ozw.zhaomingkeji.xyz

Go:   // 无解构
来源：http://tth.xuanzx.com

Ruby: a, b = pair
来源：http://utn.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://eig.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://iqc.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pzr.yonumen.top

PHP:  // 无重载
来源：http://pfk.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://igh.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://pin.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ujt.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://hkb.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://zhn.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sly.pycfn.com

================================================================================
来源：http://wdt.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://eso.hfpthk.cn

================================================================================
来源：http://zhs.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://rby.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://euh.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lir.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ope.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zvq.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cja.yvedp.cn


<!-- 参考信息 -->