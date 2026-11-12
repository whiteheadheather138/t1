代发 wailian999

[B01] 条件判断 if / else
来源：http://fll.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cgw.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ddc.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zoh.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pbd.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eob.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yvc.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yob.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sjc.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://boj.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tqk.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ruv.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://adh.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzk.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfq.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bnz.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mzg.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uys.hywenlv.cn

[B03] switch / match / case
来源：http://itf.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://syh.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qmb.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpj.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqa.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uvy.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kvg.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dlh.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ska.snrcjt.cn

[B04] for 计数循环
来源：http://yhk.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://ffv.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xmg.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ldg.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hlu.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygd.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zaf.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://xtm.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fwg.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://qis.yfazqb.com

Py:   for item in arr: print(item)
来源：http://ecg.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eqx.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uom.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sup.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qos.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wnk.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://suu.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zvk.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://eui.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wwg.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yuw.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qdq.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pey.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oyo.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ztq.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hrj.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://muf.chenjidiqi.icu

[B07] while 循环
来源：http://zns.fktsv.cn

Py:   while i < 10: i += 1
来源：http://dvn.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vcb.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://mju.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://wbm.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://fvh.zhengqikj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bkq.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://dou.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://kyo.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://jxq.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://ywb.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rox.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://cff.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://fsv.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://rtm.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gda.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://ekx.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://xry.jinqigufen.top

[B09] break 与 continue
来源：http://ykq.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mns.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jbx.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncy.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zeo.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhq.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yvp.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pfu.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdb.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://dmi.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://szv.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bgi.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lex.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nyh.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qff.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://smq.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yfp.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://loq.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://wad.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://vby.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://wjd.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://anc.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ovr.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wgq.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aid.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://ntk.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xbu.yj202588.top

[B12] 跳出多层循环
来源：http://kdk.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://myj.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kjr.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dff.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mub.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ami.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xcv.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ahw.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zmn.svipenyu.cn

[B13] 判断是否为数字
来源：http://epx.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://phe.sweek.top

PHP:  is_numeric($x)
来源：http://sqm.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pku.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nop.hnqzz.top

Java: x instanceof Number
来源：http://khw.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://say.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://hzh.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://hpu.redwolf501.top

[B14] 判断值是否在集合内
来源：http://fli.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fdt.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upb.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://fpc.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://kot.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yzl.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://isb.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://wuw.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vkn.sufxvd.cn

[B15] 布尔运算与取反
来源：http://xgx.yvedp.cn

Py:   a and b or not c
来源：http://nnz.redwolf501.top

PHP:  $a && $b || !$c
来源：http://bju.9152youxi.cn

JS:   a && b || !c
来源：http://vca.jiagoushi.top

TS:   a && b || !c
来源：http://qrh.chenlongwang.top

Java: a && b || !c
来源：http://ckp.xuanzx.com

Go:   a && b || !c
来源：http://sxj.c1oappe.top

Ruby: a && b || !c
来源：http://nrs.fzhhl.top

C#:   a && b || !c
来源：http://ghq.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rnk.zdbjq.cn

Py:   if not data: return
来源：http://vtq.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://gcv.zhongyouzk.top

JS:   if (!data) return;
来源：http://ayo.0kj1m.cn

TS:   if (!data) return;
来源：http://lqr.nwbrower.top

Java: if (data == null) return;
来源：http://gmz.cucudq.cn

Go:   if data == nil { return }
来源：http://qnk.sxryk.cn

Ruby: return if data.nil?
来源：http://lpy.cheryme.top

C#:   if (data == null) return;
来源：http://fio.yonumen.top

================================================================================
来源：http://mtq.quarkkingdee.top

C. 函数与作用域
来源：http://fgn.uphjek.com

================================================================================
来源：http://wpb.tian-w.cn

[C01] 定义函数
来源：http://igt.tanke756.top

Py:   def add(a, b): return a + b
来源：http://img.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mtg.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://ijm.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwy.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://jek.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jyu.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://cvi.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iyt.yongpay.top

[C02] 默认参数
来源：http://dvn.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://tqf.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://amq.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://ctg.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jmm.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://obu.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mmh.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://lgy.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://lyg.yanxiufei.cn

[C03] 可变参数
来源：http://mlf.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://toz.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wsw.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://esj.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ajx.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jcz.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abf.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://jjl.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://krs.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://fbk.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://biz.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zen.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ihf.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qot.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://pyp.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://yzw.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://wmv.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://hwe.shanyushiyangtech.top

[C05] 返回多个值
来源：http://yaz.pengpengdd.cyou

Py:   return a, b
来源：http://azw.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://fbj.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yle.yuanzhike.top

TS:   return { a, b };
来源：http://vvj.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wxw.zhijiandao.cn

Go:   return a, b
来源：http://him.cucudq.cn

Ruby: return a, b
来源：http://qxt.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://snf.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://frg.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://scd.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dla.aizwys.cn

JS:   const square = x => x * x;
来源：http://fsk.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://mnl.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aij.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://odc.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://tiv.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rje.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://quy.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ypz.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://pkn.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hog.gaohongyu789.top

TS:   arr.map(String)
来源：http://jqp.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://odn.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usf.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://gbc.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rve.hongshengwenyu.top

[C08] 闭包
来源：http://aut.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vbh.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gwq.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kqo.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qmz.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eht.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xle.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lvs.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wkx.andypj.xyz

[C09] 递归
来源：http://elb.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kha.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yhf.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dyi.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvm.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwg.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iku.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://byv.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dwe.aizwys.cn

[C10] 变量作用域
来源：http://zdp.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fnl.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mlu.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kqj.xziqi.cn

TS:   同 JS
来源：http://hgq.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://smq.hfpthk.cn

Go:   花括号块级作用域
来源：http://jzd.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aie.9152youxi.cn

C#:   块级作用域
来源：http://wpw.cucudq.cn

[C11] 模块导入与导出
来源：http://hod.meibo888.top

Py:   from module import func
来源：http://cqy.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://fcv.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://heg.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nit.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://zpm.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vdt.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://lvw.cdnleiting.top

C#:   using System.Text;
来源：http://jeg.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://omj.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://jzh.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://emm.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://oef.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://fcx.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nwb.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://jct.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://awf.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ysx.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://mgl.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vax.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbe.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://elb.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvd.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://xao.tanke756.top

Go:   func add(a, b int) int
来源：http://znd.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://red.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gld.52xcode.cn

[C14] 泛型函数
来源：http://xlk.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ois.chenzaomai.com

PHP:  // 无泛型
来源：http://raf.aizwys.cn

JS:   // 无泛型
来源：http://rpi.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lcb.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://arc.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nup.yanxiufei.cn

Ruby: # 无泛型
来源：http://pjw.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qed.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://wdp.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jgo.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://nsu.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://elj.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ipb.snrcjt.cn

Java: // 无解构
来源：http://taz.xinyue.icu

Go:   // 无解构
来源：http://doo.gaohongyu789.top

Ruby: a, b = pair
来源：http://sdt.epnwcf.com

C#:   var (a, b) = pair;
来源：http://heq.fktsv.cn

[C16] 函数 / 方法重载
来源：http://koy.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nyd.zhixingplan.top

PHP:  // 无重载
来源：http://hwt.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gys.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://lyh.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pnd.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://qvx.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://prp.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jwl.zhijiandao.cn

================================================================================
来源：http://sfj.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://zby.daria6918.cn

================================================================================
来源：http://qtw.cucudq.cn

[D01] 创建数组 / 列表
来源：http://xkv.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tvl.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mro.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://itq.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zwu.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nwl.fehbvm.com


<!-- 参考信息 -->