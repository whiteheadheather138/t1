代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mni.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://itx.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lyf.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qei.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtu.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uaq.jlsjyb.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxx.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vjs.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwa.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkw.cucudq.cn

[B03] switch / match / case
来源：http://eqn.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lrh.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fyo.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rbf.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uau.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wzm.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://msm.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eqc.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fkd.wangshuangyany.cn

[B04] for 计数循环
来源：http://jio.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://nvu.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ozx.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bdu.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sxn.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cch.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zqr.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://kxo.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://voa.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://dpt.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://srv.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ewb.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zkz.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://mva.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uqm.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nft.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://jdx.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ckp.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://obu.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://qla.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://krd.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lpg.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://izf.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bkn.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cvm.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xvd.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ecv.yuxming.cn

[B07] while 循环
来源：http://kjk.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://amv.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://lld.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://lng.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://cjd.pycfn.com

Java: while (i < 10) { i++; }
来源：http://cww.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fng.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://vyt.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://lxs.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://unl.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://ggr.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kvd.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://sxj.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://yos.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://ezn.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cdm.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cij.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://ccm.hfpthk.cn

[B09] break 与 continue
来源：http://ijm.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bit.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rbg.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsx.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrs.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzs.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bga.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cik.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://his.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://niu.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://amm.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tun.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qcl.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tou.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://and.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cqe.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gcf.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qzt.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://jwi.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://nrk.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://zqo.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gum.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://axe.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dpx.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vxe.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://wsz.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oob.zycfv.cn

[B12] 跳出多层循环
来源：http://xwy.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://erx.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pah.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yja.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyr.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jqu.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dof.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ysy.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ixg.zhengqikj.top

[B13] 判断是否为数字
来源：http://njo.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://yoy.316326.xyz

PHP:  is_numeric($x)
来源：http://xvv.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://znm.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fnv.tarul.cn

Java: x instanceof Number
来源：http://dmg.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kvj.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://xjf.yuxming.cn

C#:   x is int or double or decimal
来源：http://xsn.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://mzu.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ybv.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ikk.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://czk.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://ojn.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dvm.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dby.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://srx.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xcb.chenlongwang.top

[B15] 布尔运算与取反
来源：http://oki.cqqwz.cn

Py:   a and b or not c
来源：http://cmt.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://hyf.shuidangran.top

JS:   a && b || !c
来源：http://fmo.52xcode.cn

TS:   a && b || !c
来源：http://vai.zhoulong.xyz

Java: a && b || !c
来源：http://rpc.jinqigfzy.top

Go:   a && b || !c
来源：http://vyi.havefunace.top

Ruby: a && b || !c
来源：http://tjw.pycfn.com

C#:   a && b || !c
来源：http://vba.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://vst.gzhubu.top

Py:   if not data: return
来源：http://gwq.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://gou.ppjwa.cn

JS:   if (!data) return;
来源：http://wwl.daxiang520.top

TS:   if (!data) return;
来源：http://zcc.0kj1m.cn

Java: if (data == null) return;
来源：http://soq.9152youxi.cn

Go:   if data == nil { return }
来源：http://gny.jlsjyb.cn

Ruby: return if data.nil?
来源：http://rtk.yueranfly.top

C#:   if (data == null) return;
来源：http://ufs.316326.xyz

================================================================================
来源：http://dyu.hnqzz.top

C. 函数与作用域
来源：http://vmc.gzhubu.top

================================================================================
来源：http://jys.hysaishi.cn

[C01] 定义函数
来源：http://sas.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://vtc.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ysm.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://szr.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxe.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://xhn.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://lyz.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://yyu.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lye.feifeiyinyue.top

[C02] 默认参数
来源：http://uaq.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://pxm.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jgm.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://xmi.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vvu.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yhz.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zkw.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://akp.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://atp.zycfv.cn

[C03] 可变参数
来源：http://crb.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://ruj.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yzx.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vlk.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wsi.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ujg.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kkt.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://sac.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ada.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://ptr.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kwa.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vrb.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nwi.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qak.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://ick.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://itn.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://qhr.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://waq.hnqzz.top

[C05] 返回多个值
来源：http://okc.havefunace.top

Py:   return a, b
来源：http://nrt.316326.xyz

PHP:  return [$a, $b];
来源：http://wmg.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rwa.jinghuilouyu.cn

TS:   return { a, b };
来源：http://vxp.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pdr.fehbvm.com

Go:   return a, b
来源：http://fyq.fktsv.cn

Ruby: return a, b
来源：http://vqi.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://ybb.hammf.cn

[C06] 匿名函数 / lambda
来源：http://tmx.smart0.xyz

Py:   square = lambda x: x * x
来源：http://ljr.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jbv.yfazqb.com

JS:   const square = x => x * x;
来源：http://qsr.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://pjf.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wib.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://ohi.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://lsk.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ucb.uphjek.com

[C07] 把函数作为参数传入
来源：http://vuq.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iwp.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dqc.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ieq.smart0.xyz

TS:   arr.map(String)
来源：http://kki.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://abi.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://upw.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://fxl.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yeh.sjlbkw.cn

[C08] 闭包
来源：http://cko.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aut.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gca.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hfk.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptb.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nwm.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jnp.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://boo.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tll.jianghu66.top

[C09] 递归
来源：http://cug.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gov.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cmw.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://inz.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grc.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://giq.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://shx.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bth.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mtv.hcnkem.com

[C10] 变量作用域
来源：http://gvj.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://src.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://doq.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rgj.52xcode.cn

TS:   同 JS
来源：http://veg.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://zve.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://wsn.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yos.chenjidiqi.icu

C#:   块级作用域
来源：http://wxf.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://rim.jiagoushi.top

Py:   from module import func
来源：http://nyf.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vdo.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://acz.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qbo.bbcook.cn

Java: import java.util.List;
来源：http://mlt.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ehd.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://lam.aibaodan.cn

C#:   using System.Text;
来源：http://btp.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://ftc.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://coz.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://ide.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://bxt.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://zwt.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wwc.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://ioo.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://dqp.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://sdz.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://cyj.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://txj.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lyt.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://usl.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iju.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oig.fengsongda.top

Go:   func add(a, b int) int
来源：http://pff.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://erg.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://tqh.cashguo.top

[C14] 泛型函数
来源：http://iqc.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dpd.0kj1m.cn

PHP:  // 无泛型
来源：http://xwm.c1oappe.top

JS:   // 无泛型
来源：http://gao.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gnr.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jol.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ctp.hfpthk.cn

Ruby: # 无泛型
来源：http://kuj.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://shz.zycfv.cn

[C15] 解构 / 展开参数
来源：http://ail.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bws.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://psn.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lsf.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hxc.hywenlv.cn

Java: // 无解构
来源：http://fbf.kuanghao11.cn

Go:   // 无解构
来源：http://qsi.316326.xyz

Ruby: a, b = pair
来源：http://gqv.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://vwp.hammf.cn

[C16] 函数 / 方法重载
来源：http://yyy.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zbh.epnwcf.com

PHP:  // 无重载
来源：http://pfj.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://shb.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://fsr.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://icv.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://sbb.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://kqt.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://idc.0kj1m.cn

================================================================================
来源：http://ibp.ivvv.top

D. 数组 / 列表 / 集合
来源：http://zil.zycfv.cn

================================================================================
来源：http://fxc.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://zxn.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovn.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dgz.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://svm.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ycs.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uns.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://wub.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://zbc.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ikb.yuxming.cn

[D02] 追加元素到末尾
来源：http://frk.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gie.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fog.hysaishi.cn

JS:   arr.push(4);
来源：http://cxy.c1oappe.top

TS:   arr.push(4);
来源：http://mpl.0kj1m.cn


<!-- 参考信息 -->