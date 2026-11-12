代发 wailian999

[A26] 类型转换总览
来源：http://quc.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pzg.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tsd.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ocv.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://kvb.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mhn.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dvp.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kzf.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zjz.yfazqb.com

================================================================================
来源：http://wfi.zhiwuduotai.top

B. 流程控制
来源：http://tss.tian-w.cn

================================================================================
来源：http://gos.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://llm.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ekf.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ufz.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rdz.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hat.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rjz.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://drf.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ouj.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://znw.hesvh.cn

[B02] 多分支 else if / elif
来源：http://omt.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tws.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cgw.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nft.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otn.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtu.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uuq.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://apc.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cji.zycfv.cn

[B03] switch / match / case
来源：http://zpm.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aho.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://czt.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpa.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vba.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nei.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ars.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://woi.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vaa.svipenyu.cn

[B04] for 计数循环
来源：http://eqr.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://mik.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vaj.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kha.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gep.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fle.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zjg.birdmap.top

Ruby: 10.times { |i| puts i }
来源：http://vgb.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qay.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://maf.xziqi.cn

Py:   for item in arr: print(item)
来源：http://mrd.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://omy.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rst.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://biq.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lmn.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://swu.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://qlo.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpc.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://xmn.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uis.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lcp.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtm.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yxw.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ulb.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tor.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hee.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iqz.shanyushiyangkeji.top

[B07] while 循环
来源：http://xoy.tian-w.cn

Py:   while i < 10: i += 1
来源：http://ixj.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zwf.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://mej.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://ybk.meibo888.top

Java: while (i < 10) { i++; }
来源：http://nch.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vhl.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://vny.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://fvi.xziqi.cn

[B08] do-while（至少执行一次）
来源：http://afl.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://lgf.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://klc.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://ont.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://moq.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://dja.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aym.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nbl.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://jku.bbcook.cn

[B09] break 与 continue
来源：http://llm.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://htl.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ang.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktr.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idh.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvr.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evs.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fbv.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tad.xziqi.cn

[B10] 遍历同时拿索引
来源：http://wcl.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkz.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qdh.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://feg.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lrk.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qxk.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ipe.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iyp.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dda.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://kno.iojbl.cn

Py:   list(range(0, 10, 2))
来源：http://dyn.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://dzq.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggw.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dyo.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zuy.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fyk.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://dhd.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ocw.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://uzq.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://htg.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dxz.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kga.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xea.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tar.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://noq.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lsm.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eil.jqgufenzy.top

[B13] 判断是否为数字
来源：http://oup.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://jxj.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://zjh.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://psl.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sop.snrcjt.cn

Java: x instanceof Number
来源：http://eky.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nge.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://ivh.cdnleiting.top

C#:   x is int or double or decimal
来源：http://pbn.yvedp.cn

[B14] 判断值是否在集合内
来源：http://ygt.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://etu.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kkc.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://buk.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://uzo.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://snj.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://noi.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://srk.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rdy.yangfankeji.com

[B15] 布尔运算与取反
来源：http://dqg.jyoumei.cn

Py:   a and b or not c
来源：http://hyo.tarul.cn

PHP:  $a && $b || !$c
来源：http://ius.jlsjyb.cn

JS:   a && b || !c
来源：http://guk.jinqigufen.top

TS:   a && b || !c
来源：http://fnx.jiagoushi.top

Java: a && b || !c
来源：http://cph.9152youxi.cn

Go:   a && b || !c
来源：http://mrj.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://iqf.bjfxy.top

C#:   a && b || !c
来源：http://hpx.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nxw.gzhubu.top

Py:   if not data: return
来源：http://bcp.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://heq.wangshuangyany.cn

JS:   if (!data) return;
来源：http://bmg.yj20258.top

TS:   if (!data) return;
来源：http://ijs.cqqwz.cn

Java: if (data == null) return;
来源：http://efq.cashguo.top

Go:   if data == nil { return }
来源：http://mpw.quarkkingdee.top

Ruby: return if data.nil?
来源：http://wfe.dashuyun.cn

C#:   if (data == null) return;
来源：http://qzj.ppjwa.cn

================================================================================
来源：http://bkh.birdmap.top

C. 函数与作用域
来源：http://icu.quarkkingdee.top

================================================================================
来源：http://adh.cdnleiting.top

[C01] 定义函数
来源：http://ytx.sweek.top

Py:   def add(a, b): return a + b
来源：http://rxx.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lzy.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://dki.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wlq.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kqe.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://jig.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://qsf.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oit.cashguo.top

[C02] 默认参数
来源：http://yet.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://jne.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://uzt.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://hlo.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://raf.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uoj.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ltk.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://dtg.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://vjt.zhongyouzk.top

[C03] 可变参数
来源：http://nie.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://uxs.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hez.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nre.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpr.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tex.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://quo.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vim.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bhn.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://xjp.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aez.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xgm.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wjy.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jqt.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://zjn.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://xvu.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://ixo.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://rii.ppjwa.cn

[C05] 返回多个值
来源：http://mpk.birdmap.top

Py:   return a, b
来源：http://apf.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://gme.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://myd.gogol.net.cn

TS:   return { a, b };
来源：http://spc.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eha.havefunace.top

Go:   return a, b
来源：http://twb.jlsjyb.cn

Ruby: return a, b
来源：http://fzp.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ppx.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://hvp.fengsongda.top

Py:   square = lambda x: x * x
来源：http://xja.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pmn.cqqwz.cn

JS:   const square = x => x * x;
来源：http://kpo.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://iir.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zvn.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://xhi.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://whf.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://nvq.yj20258.top

[C07] 把函数作为参数传入
来源：http://vnr.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qbu.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iyc.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://civ.jlsjyb.cn

TS:   arr.map(String)
来源：http://ivv.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nkv.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nwx.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://kpi.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://doz.uphjek.com

[C08] 闭包
来源：http://cbv.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://edl.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gax.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://msa.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mku.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qdp.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sxt.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rbg.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hka.sjlbkw.cn

[C09] 递归
来源：http://qla.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jed.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bun.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mzz.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cjn.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qbj.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xre.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://itd.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qjv.zhiwuduotai.top

[C10] 变量作用域
来源：http://gqo.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ogt.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tui.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ibs.pengpengdd.cyou

TS:   同 JS
来源：http://elg.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://pji.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://yfx.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hjr.yvedp.cn

C#:   块级作用域
来源：http://lrz.cheryme.top

[C11] 模块导入与导出
来源：http://rbp.gotoacloud.top

Py:   from module import func
来源：http://ikx.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://umf.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bqx.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ycj.yongpay.top

Java: import java.util.List;
来源：http://dvc.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mdl.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://kna.yonumen.top

C#:   using System.Text;
来源：http://lme.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://weu.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://sxg.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://dma.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://del.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://its.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hqv.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://euf.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://tqc.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qqc.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://jjq.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kca.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rjb.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvb.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gts.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kex.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://zex.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kth.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://vfv.redwolf501.top

[C14] 泛型函数
来源：http://fum.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jsf.iojbl.cn

PHP:  // 无泛型
来源：http://bkf.fengsongda.top

JS:   // 无泛型
来源：http://eek.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vdi.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dak.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dzf.hnxiangtu.top

Ruby: # 无泛型
来源：http://kui.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcy.xziqi.cn

[C15] 解构 / 展开参数
来源：http://bqh.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rre.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://eef.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ugb.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fud.cashguo.top

Java: // 无解构
来源：http://ypx.quarkkingdee.top

Go:   // 无解构
来源：http://une.shangyingyoupin.top

Ruby: a, b = pair
来源：http://ihd.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://nne.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://hzs.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bwa.hywenlv.cn

PHP:  // 无重载
来源：http://iin.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ykm.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://rcu.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zcw.cqqwz.cn


<!-- 参考信息 -->