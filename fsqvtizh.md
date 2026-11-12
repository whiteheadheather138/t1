代发 wailian999

[B01] 条件判断 if / else
来源：http://lcn.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nqt.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxj.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://art.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qxu.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oal.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://srq.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ikr.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gzc.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://lkg.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nnb.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bld.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvm.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pek.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyn.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dcf.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nmn.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gad.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://wyr.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://izd.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xwm.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://grs.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://usp.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rfm.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ufy.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vbs.hfpthk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://paa.hammf.cn

[B04] for 计数循环
来源：http://zwr.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://tgx.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dez.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://flu.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qql.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frt.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pzy.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://hys.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gkq.cheryme.top

[B05] 遍历数组 / 列表
来源：http://tgl.c1oappe.top

Py:   for item in arr: print(item)
来源：http://hkn.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zzy.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://eji.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lgo.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hkj.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lpd.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://ezh.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aok.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://zww.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dup.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://chv.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sym.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zjx.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rih.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qob.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ahw.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bre.shangyingyoupin.top

[B07] while 循环
来源：http://uyj.vehdjk.com

Py:   while i < 10: i += 1
来源：http://ppu.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://anw.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://zwr.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://kuc.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://orc.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vae.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://xlk.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://mnu.yj20258.top

[B08] do-while（至少执行一次）
来源：http://sgo.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://zbs.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qpd.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://jtf.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://thr.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://lwa.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zvi.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://wmv.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://jmi.zhixingplan.top

[B09] break 与 continue
来源：http://vvq.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zya.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ztr.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guj.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbj.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imz.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kky.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://amn.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocw.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://zca.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xat.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://muf.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nzj.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hav.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bes.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nga.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hgl.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eqf.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://dri.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://xiv.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://hly.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sba.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://egm.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aww.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bnm.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://ueb.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrj.jianghu66.top

[B12] 跳出多层循环
来源：http://gbl.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gtr.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zda.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://euc.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ygd.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vge.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://egz.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dqt.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zwv.mhx1999.top

[B13] 判断是否为数字
来源：http://zit.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://iep.bjfxy.top

PHP:  is_numeric($x)
来源：http://tyo.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sta.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gnl.cdnleiting.top

Java: x instanceof Number
来源：http://zpd.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://amm.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://rlk.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://hzv.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://fzs.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fxq.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fph.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://lne.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://ivb.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://dry.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lna.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://hvi.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nlv.guannengcc.top

[B15] 布尔运算与取反
来源：http://rnj.bbcook.cn

Py:   a and b or not c
来源：http://qbq.ivvv.top

PHP:  $a && $b || !$c
来源：http://vmv.yanxiufei.cn

JS:   a && b || !c
来源：http://nbi.gzhubu.top

TS:   a && b || !c
来源：http://bxy.zhoulong.xyz

Java: a && b || !c
来源：http://oza.bjfxy.top

Go:   a && b || !c
来源：http://orl.hnxiangtu.top

Ruby: a && b || !c
来源：http://imd.wangdashe.top

C#:   a && b || !c
来源：http://sca.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://pgh.cqqwz.cn

Py:   if not data: return
来源：http://fdu.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://mjv.yonumen.top

JS:   if (!data) return;
来源：http://gix.gotoacloud.top

TS:   if (!data) return;
来源：http://dea.hywenlv.cn

Java: if (data == null) return;
来源：http://kww.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://vuw.zhijiandao.cn

Ruby: return if data.nil?
来源：http://dfp.svipenyu.cn

C#:   if (data == null) return;
来源：http://vdu.chenjidiqi.icu

================================================================================
来源：http://bej.fengsongda.top

C. 函数与作用域
来源：http://tfy.fehbvm.com

================================================================================
来源：http://aad.jinghuilouyu.cn

[C01] 定义函数
来源：http://ycn.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://kxw.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kve.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://keo.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpg.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fkk.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://fur.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://uiz.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://icb.snrcjt.cn

[C02] 默认参数
来源：http://kps.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://pgu.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aae.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://kbt.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://diw.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdc.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vjw.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://ndw.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://awy.jqgfzy.top

[C03] 可变参数
来源：http://tue.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://jbi.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uno.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ijb.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjd.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vqg.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rak.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://qgp.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xye.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://wjs.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kdk.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zct.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://orv.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ddd.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pju.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://sgr.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://efc.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://lkp.shangyingyoupin.top

[C05] 返回多个值
来源：http://tci.aibaodan.cn

Py:   return a, b
来源：http://olw.dianchejie.cn

PHP:  return [$a, $b];
来源：http://dyp.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eci.sjlbkw.cn

TS:   return { a, b };
来源：http://ghh.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://saa.0kj1m.cn

Go:   return a, b
来源：http://edn.hnqzz.top

Ruby: return a, b
来源：http://kee.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://zyj.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://vec.yonumen.top

Py:   square = lambda x: x * x
来源：http://nih.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://odf.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://nih.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://sdb.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xum.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://owu.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://qer.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ngd.shuidangran.top

[C07] 把函数作为参数传入
来源：http://dui.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tur.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://buj.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nvp.c1oappe.top

TS:   arr.map(String)
来源：http://eit.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gay.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nwf.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://zpm.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://aew.yuxming.cn

[C08] 闭包
来源：http://hfm.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nlv.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://asn.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yhw.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ygb.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fcy.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yic.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ebr.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ppq.zycfv.cn

[C09] 递归
来源：http://zqy.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://omi.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qpl.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcj.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvu.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://piz.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://spv.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zmy.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xip.9152youxi.cn

[C10] 变量作用域
来源：http://smu.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mbo.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uoy.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqb.gaohongyu789.top

TS:   同 JS
来源：http://unn.fengsongda.top

Java: 方法内为块级作用域
来源：http://zbv.chenzaomai.com

Go:   花括号块级作用域
来源：http://sls.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yll.jinqigufen.top

C#:   块级作用域
来源：http://ewe.daxiang520.top

[C11] 模块导入与导出
来源：http://ngx.jinghuilouyu.cn

Py:   from module import func
来源：http://noq.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tst.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://adw.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wyz.zhixingplan.top

Java: import java.util.List;
来源：http://ois.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qju.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://tbj.hesvh.cn

C#:   using System.Text;
来源：http://jjp.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://rrc.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://fiq.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://dik.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://aek.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://phh.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ico.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://mas.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://zjm.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ipf.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://gcy.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hqg.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rvc.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hdl.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tpm.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://cfa.yonumen.top

Go:   func add(a, b int) int
来源：http://ubl.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zmu.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qno.jinqigfzy.top

[C14] 泛型函数
来源：http://ocv.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ebw.yanxiufei.cn

PHP:  // 无泛型
来源：http://nrl.ydjk.org.cn

JS:   // 无泛型
来源：http://nyv.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tsk.birdmap.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://krt.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mss.cashguo.top

Ruby: # 无泛型
来源：http://isy.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qht.fzhhl.top

[C15] 解构 / 展开参数
来源：http://mrh.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bei.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://gyy.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hte.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fif.ybcxt.top

Java: // 无解构
来源：http://srz.0kj1m.cn

Go:   // 无解构
来源：http://leh.shangyingyoupin.top

Ruby: a, b = pair
来源：http://occ.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://pbv.xylfe.cn

[C16] 函数 / 方法重载
来源：http://mjp.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jla.shuidangran.top

PHP:  // 无重载
来源：http://cmi.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tbg.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://mif.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hhp.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://bzx.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://zqo.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://woe.yanxiufei.cn

================================================================================
来源：http://eqr.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://iar.xuetiantiany.cn

================================================================================
来源：http://zbz.daria6918.cn

[D01] 创建数组 / 列表
来源：http://xcz.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jne.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rsc.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qum.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://nah.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pjb.zhixingplan.top


<!-- 参考信息 -->