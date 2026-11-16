代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lms.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fco.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://juc.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rfl.yonumen.top

[A26] 类型转换总览
来源：http://wbw.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xwn.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pwp.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zvc.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://qfk.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jmk.zhaomingkeji.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zrr.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mqm.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mdu.aibaodan.cn

================================================================================
来源：http://zvc.ydzc1.top

B. 流程控制
来源：http://wze.zhengqikj.top

================================================================================
来源：http://odb.aibaodan.cn

[B01] 条件判断 if / else
来源：http://rwa.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qqa.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://klo.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ygn.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rnb.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aan.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uke.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pll.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://smf.hnqzz.top

[B02] 多分支 else if / elif
来源：http://rkn.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uwo.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vnu.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxb.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://znd.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccx.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ptk.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ydn.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://abl.aibaodan.cn

[B03] switch / match / case
来源：http://hjj.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nti.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fod.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odw.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fkl.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xoo.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cml.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yyd.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://arx.zhoulong.xyz

[B04] for 计数循环
来源：http://yvd.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://ycw.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://muw.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vhl.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lek.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lzy.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://doy.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://gro.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jhy.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://viy.c1oappe.top

Py:   for item in arr: print(item)
来源：http://kzh.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://niq.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qhs.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ehf.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ynb.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tfj.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://puo.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lve.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://nhx.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qsi.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://adh.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbk.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spf.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ugo.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kuv.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sps.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eiy.jianghu66.top

[B07] while 循环
来源：http://vyp.redwolf501.top

Py:   while i < 10: i += 1
来源：http://zva.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://aap.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://dxz.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://jwu.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://iwb.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ozi.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://laa.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://igk.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://sew.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://acg.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xyy.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://brk.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://wuz.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://sqj.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kkm.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://hvk.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://fqd.sweek.top

[B09] break 与 continue
来源：http://wlu.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qiy.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bpx.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqv.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://etz.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lrl.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://izw.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dvp.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybd.ybcxt.top

[B10] 遍历同时拿索引
来源：http://cnp.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lck.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dqi.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jbx.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jvt.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bai.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kpo.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kuy.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://imd.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://ith.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://rwm.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://zto.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urp.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://upd.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://odg.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jgn.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://itv.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fat.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://ezq.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sdo.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lln.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpp.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vko.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wwy.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://prb.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wql.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yhp.nanxuanxn.top

[B13] 判断是否为数字
来源：http://osr.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://kli.guowangkeji.top

PHP:  is_numeric($x)
来源：http://iad.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzf.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pjw.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://ewf.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oqt.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://fle.hfpthk.cn

C#:   x is int or double or decimal
来源：http://xqd.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://qrs.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rno.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bjl.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://ott.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://yhn.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qer.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://htj.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qdo.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qoa.fzhhl.top

[B15] 布尔运算与取反
来源：http://vyx.shzxlz.cn

Py:   a and b or not c
来源：http://cpn.gzhubu.top

PHP:  $a && $b || !$c
来源：http://byw.yj20258888.top

JS:   a && b || !c
来源：http://xoc.hammf.cn

TS:   a && b || !c
来源：http://qxw.tarul.cn

Java: a && b || !c
来源：http://oem.hywenlv.cn

Go:   a && b || !c
来源：http://uis.pengpengdd.cyou

Ruby: a && b || !c
来源：http://nuh.aibaodan.cn

C#:   a && b || !c
来源：http://ndj.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://xzy.sweek.top

Py:   if not data: return
来源：http://sgr.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://qnf.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://ghg.zhongyouzk.top

TS:   if (!data) return;
来源：http://ygf.jqgufenzy.top

Java: if (data == null) return;
来源：http://ecu.birdmap.top

Go:   if data == nil { return }
来源：http://lnr.svipenyu.cn

Ruby: return if data.nil?
来源：http://nre.smart0.xyz

C#:   if (data == null) return;
来源：http://vzm.yuxming.cn

================================================================================
来源：http://qkl.jiagoushi.top

C. 函数与作用域
来源：http://txy.fanxiaobao.xyz

================================================================================
来源：http://zky.yuxming.cn

[C01] 定义函数
来源：http://mrd.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://vbp.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yeb.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://eef.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zvz.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ogx.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://jfw.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://hif.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxb.redwolf501.top

[C02] 默认参数
来源：http://bql.pycfn.com

Py:   def greet(name="World"): return name
来源：http://ram.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cct.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://jof.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xqi.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://rld.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ude.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://ceu.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://neb.hammf.cn

[C03] 可变参数
来源：http://kas.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://qug.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://whp.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kbd.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ytb.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pby.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mcd.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://gzs.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ann.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://ngw.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fde.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ttt.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oon.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ubv.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://gnw.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://uuq.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://qxq.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://too.daxiang520.top

[C05] 返回多个值
来源：http://nqj.vehdjk.com

Py:   return a, b
来源：http://xjz.nwbrower.top

PHP:  return [$a, $b];
来源：http://kie.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nfd.mhx1999.top

TS:   return { a, b };
来源：http://bnb.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xod.sysykeji.top

Go:   return a, b
来源：http://npr.haohaochexian.top

Ruby: return a, b
来源：http://yys.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://wyn.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://qqe.birdmap.top

Py:   square = lambda x: x * x
来源：http://ion.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ojn.0kj1m.cn

JS:   const square = x => x * x;
来源：http://gtv.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://urn.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hnv.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zjb.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://paj.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ser.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://rlj.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mbi.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://tpw.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vre.bbcook.cn

TS:   arr.map(String)
来源：http://lmn.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nhk.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qxo.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://pal.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://puo.yj20258.top

[C08] 闭包
来源：http://urp.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ril.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fbc.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xuq.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kju.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cdb.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zhz.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lxm.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ynt.snrcjt.cn

[C09] 递归
来源：http://ccx.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lki.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wrt.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdu.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nga.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jir.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zhp.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pcq.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hym.yangfankeji.com

[C10] 变量作用域
来源：http://dab.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://den.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gjc.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sgx.chenlongwang.top

TS:   同 JS
来源：http://tai.guannengcc.top

Java: 方法内为块级作用域
来源：http://lwz.meibo888.top

Go:   花括号块级作用域
来源：http://oht.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qxu.sweek.top

C#:   块级作用域
来源：http://bxo.yangfankeji.com

[C11] 模块导入与导出
来源：http://bzf.fzhhl.top

Py:   from module import func
来源：http://ltm.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jny.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eld.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nym.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://fhw.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eus.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://qit.yangfankeji.com

C#:   using System.Text;
来源：http://dmj.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://pxe.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://eai.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://jey.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://mqm.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://nxq.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://trm.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://crq.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://smh.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wvn.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://dbk.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fgm.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ugz.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lga.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsu.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vrc.hywenlv.cn

Go:   func add(a, b int) int
来源：http://nqm.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://swn.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://jds.cheryme.top

[C14] 泛型函数
来源：http://nlw.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jqx.zhongyouzk.top

PHP:  // 无泛型
来源：http://rxj.mhx1999.top

JS:   // 无泛型
来源：http://mue.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hak.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baf.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://okt.52xcode.cn

Ruby: # 无泛型
来源：http://jxd.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qbe.yfazqb.com

[C15] 解构 / 展开参数
来源：http://tzr.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fsq.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://nox.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lxa.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://def.shangyingyoupin.top

Java: // 无解构
来源：http://der.shanyushiyangkeji.top

Go:   // 无解构
来源：http://hzb.gaohongyu789.top

Ruby: a, b = pair
来源：http://ncs.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://bsp.ivvv.top

[C16] 函数 / 方法重载
来源：http://anf.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://csf.quarkkingdee.top


<!-- 参考信息 -->