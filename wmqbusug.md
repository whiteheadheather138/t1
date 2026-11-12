代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zxx.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uer.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zvw.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gla.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wpr.smart0.xyz

[B02] 多分支 else if / elif
来源：http://wod.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://teq.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vga.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwx.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uur.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxo.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tub.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://llh.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://liv.yfazqb.com

[B03] switch / match / case
来源：http://rio.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://svy.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kjc.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mzq.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ejh.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pvo.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hbn.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wxo.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tzc.wangdashe.top

[B04] for 计数循环
来源：http://vad.havefunace.top

Py:   for i in range(10): print(i)
来源：http://yup.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://trt.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxz.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vos.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zop.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bel.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://gky.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tou.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://ybh.guannengcc.top

Py:   for item in arr: print(item)
来源：http://toq.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hza.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rjk.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cqw.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dwp.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://azl.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://srz.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fjx.birdmap.top

[B06] 遍历字典 / 对象
来源：http://jgd.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fzl.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ryk.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yrg.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sst.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mxk.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ivx.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kut.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pph.hongshengwenyu.top

[B07] while 循环
来源：http://ejh.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://yuw.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://zlv.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://nrm.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://uad.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://nzn.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://esi.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://peq.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://wzo.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://zll.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://hzn.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://jbs.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://dgw.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://hzn.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://owm.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kkl.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://xen.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://que.ivvv.top

[B09] break 与 continue
来源：http://uqk.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://img.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mmc.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqq.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hts.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdk.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://csz.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wxi.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzd.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://yet.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfr.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://laa.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hhu.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fod.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://riv.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jdb.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pto.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qax.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://jjo.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://scm.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://rej.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ner.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ncl.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cpd.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gij.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://col.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://azf.tarul.cn

[B12] 跳出多层循环
来源：http://wxo.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tko.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tsn.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mkd.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cnk.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://isi.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wvl.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kkg.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://afm.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://qiq.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://wzp.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://yzo.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://agz.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oyr.ehwqpu.com

Java: x instanceof Number
来源：http://dkp.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tju.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://aiu.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://iny.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://ntr.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kxj.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gai.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://uqt.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://sfo.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kcn.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qnn.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://smg.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dsf.redwolf501.top

[B15] 布尔运算与取反
来源：http://bde.yonumen.top

Py:   a and b or not c
来源：http://the.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://zsu.shuidangran.top

JS:   a && b || !c
来源：http://lkz.jqgufenzy.top

TS:   a && b || !c
来源：http://kcr.shanyushiyangkeji.top

Java: a && b || !c
来源：http://omo.iojbl.cn

Go:   a && b || !c
来源：http://lju.yj20258.top

Ruby: a && b || !c
来源：http://reb.bjfxy.top

C#:   a && b || !c
来源：http://dqt.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nli.zycfv.cn

Py:   if not data: return
来源：http://rry.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://haj.aibaodan.cn

JS:   if (!data) return;
来源：http://dhj.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://fta.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://jxp.nwbrower.top

Go:   if data == nil { return }
来源：http://xfh.yangfankeji.com

Ruby: return if data.nil?
来源：http://rpm.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://fne.jinqigfzy.top

================================================================================
来源：http://lfr.redwolf501.top

C. 函数与作用域
来源：http://xzh.smart0.xyz

================================================================================
来源：http://kth.zdqjudy.top

[C01] 定义函数
来源：http://xwl.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://nnk.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ood.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xym.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gwh.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oeg.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://leh.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://xam.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fll.hywenlv.cn

[C02] 默认参数
来源：http://dxo.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://pdd.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bdu.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://jqe.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cht.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zcp.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ntk.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://wxf.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://dtf.cashguo.top

[C03] 可变参数
来源：http://abg.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://vfa.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rrw.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://umu.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wle.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://njj.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://suu.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://mrm.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zni.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://wju.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yol.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://huy.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nci.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mwb.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://naw.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://zka.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://drw.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://bjj.haohaochexian.top

[C05] 返回多个值
来源：http://rfv.smart0.xyz

Py:   return a, b
来源：http://dwi.9152youxi.cn

PHP:  return [$a, $b];
来源：http://ttv.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://okm.gzhubu.top

TS:   return { a, b };
来源：http://jxq.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rmz.gaohongyu789.top

Go:   return a, b
来源：http://bzw.yonumen.top

Ruby: return a, b
来源：http://vol.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://cve.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://hjs.52xcode.cn

Py:   square = lambda x: x * x
来源：http://bdy.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ncl.hesvh.cn

JS:   const square = x => x * x;
来源：http://vwj.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://plx.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cay.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://the.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://uas.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://npa.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://izg.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pfo.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kdg.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyu.iojbl.cn

TS:   arr.map(String)
来源：http://vfm.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwu.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gfl.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://fzz.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wmg.zdbjq.cn

[C08] 闭包
来源：http://ffv.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dls.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xdp.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jau.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://epb.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pzc.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofl.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xbc.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jhz.bjfxy.top

[C09] 递归
来源：http://rtx.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://thn.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://der.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ube.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aty.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nfz.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wqm.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhy.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hmb.xinyue.icu

[C10] 变量作用域
来源：http://vnm.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fpq.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kka.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mbt.ehwqpu.com

TS:   同 JS
来源：http://gmk.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://wxd.tianlin.xyz

Go:   花括号块级作用域
来源：http://shf.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://azc.uphjek.com

C#:   块级作用域
来源：http://yur.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://iay.feifeiyinyue.top

Py:   from module import func
来源：http://sap.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nro.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://xay.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mao.sweek.top

Java: import java.util.List;
来源：http://kwa.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lpg.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://jcu.cheryme.top

C#:   using System.Text;
来源：http://obv.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://vhs.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://gwz.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://fuq.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://tpv.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://fzv.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eko.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://suu.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://euq.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kvj.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://eph.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gki.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://srt.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fsa.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvh.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://mrb.daria6918.cn

Go:   func add(a, b int) int
来源：http://yil.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ade.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://rfi.jinqigufen.top

[C14] 泛型函数
来源：http://dqk.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uot.jyoumei.cn

PHP:  // 无泛型
来源：http://mbc.ydzc1.top

JS:   // 无泛型
来源：http://mwq.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://won.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ftx.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvp.shuidangran.top

Ruby: # 无泛型
来源：http://pnu.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qem.hesvh.cn

[C15] 解构 / 展开参数
来源：http://hka.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xvg.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://bym.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mrh.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fer.shangyingyoupin.top

Java: // 无解构
来源：http://fyo.ivvv.top

Go:   // 无解构
来源：http://mnz.uphjek.com

Ruby: a, b = pair
来源：http://bnd.uphjek.com

C#:   var (a, b) = pair;
来源：http://mvw.cashguo.top

[C16] 函数 / 方法重载
来源：http://wnd.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://apq.shanyushiyangtech.top

PHP:  // 无重载
来源：http://exa.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fff.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://sse.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wpa.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://vhw.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://hgm.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qjv.meibo888.top

================================================================================
来源：http://etn.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://kvs.bjfxy.top

================================================================================
来源：http://qdm.fengsongda.top

[D01] 创建数组 / 列表
来源：http://gnt.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cap.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebh.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lkp.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xbi.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sfy.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://yeu.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://pev.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fhe.hesvh.cn

[D02] 追加元素到末尾
来源：http://gxe.jlsjyb.cn


<!-- 参考信息 -->