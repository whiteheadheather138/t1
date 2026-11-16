代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qah.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sqg.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kst.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cbz.52xcode.cn

[A26] 类型转换总览
来源：http://ofp.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://azd.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jpn.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mcr.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://hmr.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tsr.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jzi.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rcm.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tdj.dashuyun.cn

================================================================================
来源：http://suh.gogol.net.cn

B. 流程控制
来源：http://kfj.hongshengwenyu.top

================================================================================
来源：http://ndl.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://zys.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://xje.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xte.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vso.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qbg.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://xde.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ubx.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lvh.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hjn.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://njg.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bse.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vjw.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzf.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpk.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxq.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yzr.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://erl.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpr.yanxiufei.cn

[B03] switch / match / case
来源：http://xbh.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gko.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://znv.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gag.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://amp.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pmj.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oby.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mft.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cmh.yuxming.cn

[B04] for 计数循环
来源：http://tyg.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://wdn.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hcs.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lsp.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ccq.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://smj.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ghd.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://eco.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jgf.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://cuk.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://xbz.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehr.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://eoa.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yke.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kcw.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wda.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://xup.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nmw.havefunace.top

[B06] 遍历字典 / 对象
来源：http://cnp.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hbd.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zfk.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nxh.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fyd.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://htm.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bgr.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uwf.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sde.daria6918.cn

[B07] while 循环
来源：http://zpw.uphjek.com

Py:   while i < 10: i += 1
来源：http://fda.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cvt.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://kya.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://wqd.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://exk.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uzs.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://vnc.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://jdp.cheryme.top

[B08] do-while（至少执行一次）
来源：http://iad.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://rkq.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cys.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://wyh.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://lke.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://uqg.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zql.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pgu.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://keb.hcnkem.com

[B09] break 与 continue
来源：http://uqd.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sfh.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rjf.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogj.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qda.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxi.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qek.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ekj.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhf.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://fop.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fsb.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zvi.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oun.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://srx.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bju.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://omh.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dma.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zak.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://hvp.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://oay.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://bem.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vvc.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzu.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zly.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uwl.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://xuo.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dfe.52xcode.cn

[B12] 跳出多层循环
来源：http://sqo.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gjr.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://grb.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjp.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://deo.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wwg.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://heg.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rnc.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lmv.mhx1999.top

[B13] 判断是否为数字
来源：http://dyf.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://qxh.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://ulw.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://coa.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xow.c1oappe.top

Java: x instanceof Number
来源：http://fdc.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gai.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://cvn.nwbrower.top

C#:   x is int or double or decimal
来源：http://xsj.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://jwo.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nwa.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://npa.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://rlh.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://uoj.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yhe.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ssv.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jkf.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zpy.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://som.shzxlz.cn

Py:   a and b or not c
来源：http://hmp.sxryk.cn

PHP:  $a && $b || !$c
来源：http://hvl.zhiwuduotai.top

JS:   a && b || !c
来源：http://iyk.yj20258.top

TS:   a && b || !c
来源：http://aop.yvedp.cn

Java: a && b || !c
来源：http://awr.sjlbkw.cn

Go:   a && b || !c
来源：http://abb.cdnleiting.top

Ruby: a && b || !c
来源：http://zxo.yj202588.top

C#:   a && b || !c
来源：http://uvn.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nxq.yj20258888.top

Py:   if not data: return
来源：http://esz.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://fyy.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://zuq.yangfankeji.com

TS:   if (!data) return;
来源：http://cth.zdqjudy.top

Java: if (data == null) return;
来源：http://rsa.aibaodan.cn

Go:   if data == nil { return }
来源：http://kmk.ydzc1.top

Ruby: return if data.nil?
来源：http://fgy.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://miy.mhx1999.top

================================================================================
来源：http://egv.zdbjq.cn

C. 函数与作用域
来源：http://zto.hammf.cn

================================================================================
来源：http://ovn.0kj1m.cn

[C01] 定义函数
来源：http://smc.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://aeu.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://npf.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://idm.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzu.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://rvg.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://nlv.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://xdi.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://noc.yongpay.top

[C02] 默认参数
来源：http://ndn.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://lkq.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bxr.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://hib.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rmr.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gbv.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gwd.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://bkc.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://xqt.jinqigufen.top

[C03] 可变参数
来源：http://guq.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://uqt.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yqk.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlg.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sxz.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zkb.vqdsnc.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ljk.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://bou.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dum.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://clv.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lmw.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wel.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pib.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uem.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://znv.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://dhk.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://tdr.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://sii.xinyue.icu

[C05] 返回多个值
来源：http://gab.svipenyu.cn

Py:   return a, b
来源：http://uwp.shuidangran.top

PHP:  return [$a, $b];
来源：http://uqn.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://pza.yvedp.cn

TS:   return { a, b };
来源：http://npm.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eei.nanxuanxn.top

Go:   return a, b
来源：http://gly.nanxuanxn.top

Ruby: return a, b
来源：http://fvt.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://kvc.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://rkv.hesvh.cn

Py:   square = lambda x: x * x
来源：http://hbb.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tgt.tianlin.xyz

JS:   const square = x => x * x;
来源：http://lib.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://sgp.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hry.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://bzk.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://qiu.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://zgh.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://zan.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qib.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://afo.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jgg.ehwqpu.com

TS:   arr.map(String)
来源：http://hvp.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ysw.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wbl.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://uqo.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://owi.c1oappe.top

[C08] 闭包
来源：http://jxb.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mvk.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ouw.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dio.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okx.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lvh.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lae.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jmf.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bas.guowangkeji.top

[C09] 递归
来源：http://qci.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bgm.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fep.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gid.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vcb.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nym.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jxr.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://njr.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pzq.havefunace.top

[C10] 变量作用域
来源：http://fmh.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fxk.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nqy.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zpv.andypj.xyz

TS:   同 JS
来源：http://iun.smart0.xyz

Java: 方法内为块级作用域
来源：http://qhv.pycfn.com

Go:   花括号块级作用域
来源：http://lis.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ldy.zhaomingkeji.xyz

C#:   块级作用域
来源：http://pao.fktsv.cn

[C11] 模块导入与导出
来源：http://nmo.9152youxi.cn

Py:   from module import func
来源：http://hls.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eep.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dqs.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yry.yonumen.top

Java: import java.util.List;
来源：http://zcj.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vse.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://cix.meibo888.top

C#:   using System.Text;
来源：http://jyf.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://bua.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://qlp.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://fmz.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://vvg.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://nft.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://soq.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://fpb.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://rrk.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zty.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://pkf.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xje.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bnf.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vzr.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oos.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xiv.nwbrower.top

Go:   func add(a, b int) int
来源：http://let.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xtp.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://mfc.hysaishi.cn

[C14] 泛型函数
来源：http://dfg.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gpw.kuanghao11.cn

PHP:  // 无泛型
来源：http://tqr.dashuyun.cn

JS:   // 无泛型
来源：http://tok.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdk.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pgd.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mpc.nanxuanxn.top

Ruby: # 无泛型
来源：http://yqr.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iot.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://nas.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dnm.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://ucg.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lwb.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cxu.ivvv.top

Java: // 无解构
来源：http://szj.sweek.top

Go:   // 无解构
来源：http://gtk.xylfe.cn

Ruby: a, b = pair
来源：http://lmv.yfazqb.com

C#:   var (a, b) = pair;
来源：http://xvz.tanke756.top

[C16] 函数 / 方法重载
来源：http://gyt.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pnm.nanxuanxn.top


<!-- 参考信息 -->