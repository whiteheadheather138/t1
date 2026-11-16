代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbj.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbh.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lri.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wit.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uza.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jna.jianghu66.top

[B03] switch / match / case
来源：http://cqi.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://khd.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://plj.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://obq.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tpa.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jnc.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xkh.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gwo.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fyy.aibaodan.cn

[B04] for 计数循环
来源：http://bjd.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://hzo.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fox.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuh.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfp.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://khl.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mhe.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://wjb.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jza.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://hmb.daxiang520.top

Py:   for item in arr: print(item)
来源：http://nzm.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ktx.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://uae.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sut.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xkg.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vmm.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://tjs.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wis.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://zgu.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pio.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bev.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tfz.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lau.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kmt.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zba.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ovp.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zkw.iojbl.cn

[B07] while 循环
来源：http://teh.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://plm.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://thu.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://vml.sweek.top

TS:   while (i < 10) { i++; }
来源：http://mqz.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://lru.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xjy.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://ugq.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://haf.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://nzn.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://zbn.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dwk.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://seq.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://xoj.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://uja.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://dio.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://anb.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://zvc.ehwqpu.com

[B09] break 与 continue
来源：http://ixx.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ref.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tvb.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ery.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjt.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdi.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bys.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nks.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://the.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://cnn.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bxx.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jiw.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rpp.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uri.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vkt.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qnb.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bpv.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ghq.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://jdx.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://lqq.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://vjy.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sbg.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xra.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qpq.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iwp.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://szu.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oyc.jlsjyb.cn

[B12] 跳出多层循环
来源：http://igw.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://zxk.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wyz.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ewb.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mij.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sib.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ikr.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xai.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cei.cucudq.cn

[B13] 判断是否为数字
来源：http://jkg.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://hdd.yangfankeji.com

PHP:  is_numeric($x)
来源：http://oap.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmr.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xzr.yfazqb.com

Java: x instanceof Number
来源：http://awx.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rjy.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://lsu.tian-w.cn

C#:   x is int or double or decimal
来源：http://uqg.tanke756.top

[B14] 判断值是否在集合内
来源：http://pxk.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zdd.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://syk.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://ihy.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://mnn.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ora.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cji.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xfv.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://occ.aizwys.cn

[B15] 布尔运算与取反
来源：http://dbr.svipenyu.cn

Py:   a and b or not c
来源：http://nit.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://pui.c1oappe.top

JS:   a && b || !c
来源：http://yrw.yvedp.cn

TS:   a && b || !c
来源：http://vhj.hnqzz.top

Java: a && b || !c
来源：http://qns.hnxiangtu.top

Go:   a && b || !c
来源：http://fwk.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://mrr.kuanghao11.cn

C#:   a && b || !c
来源：http://keq.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://qkm.uphjek.com

Py:   if not data: return
来源：http://ylb.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://xck.jlsjyb.cn

JS:   if (!data) return;
来源：http://jdj.havefunace.top

TS:   if (!data) return;
来源：http://ols.yj20258888.top

Java: if (data == null) return;
来源：http://iox.tarul.cn

Go:   if data == nil { return }
来源：http://xws.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://qpc.hesvh.cn

C#:   if (data == null) return;
来源：http://rey.yangfankeji.com

================================================================================
来源：http://axn.ydjk.org.cn

C. 函数与作用域
来源：http://sjt.jqgufenzy.top

================================================================================
来源：http://iqu.jinyuanbaomall.cn

[C01] 定义函数
来源：http://bgs.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://qid.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qgm.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://exq.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfp.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fcu.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://isn.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://enc.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cnm.shangyingyoupin.top

[C02] 默认参数
来源：http://gxv.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://pbr.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xtl.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://ode.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rfb.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kki.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kvo.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://ytq.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://vzg.ywan-chungtsiang.top

[C03] 可变参数
来源：http://imo.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://vcu.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tqc.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqx.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://alu.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kym.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kqc.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pbx.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vxc.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://gkj.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://znn.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dwm.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oed.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lpt.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://wje.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://box.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://icx.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://zma.smart0.xyz

[C05] 返回多个值
来源：http://svp.svipenyu.cn

Py:   return a, b
来源：http://eix.bbcook.cn

PHP:  return [$a, $b];
来源：http://xyr.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ewz.zdbjq.cn

TS:   return { a, b };
来源：http://elw.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jzk.hysaishi.cn

Go:   return a, b
来源：http://nsv.hesvh.cn

Ruby: return a, b
来源：http://uxl.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://ods.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://bum.hammf.cn

Py:   square = lambda x: x * x
来源：http://dpw.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://bys.hysaishi.cn

JS:   const square = x => x * x;
来源：http://scd.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://buz.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://frc.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://ohr.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://dnj.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://ebz.wangdashe.top

[C07] 把函数作为参数传入
来源：http://acn.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyy.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://aqs.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cqg.gotoacloud.top

TS:   arr.map(String)
来源：http://gjs.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fqg.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fwm.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://pnj.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nzd.ybcxt.top

[C08] 闭包
来源：http://rhm.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gdy.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bpg.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ncx.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xjt.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ivx.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iqc.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uug.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yac.zycfv.cn

[C09] 递归
来源：http://jwr.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aft.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://evx.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dje.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uji.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qqw.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://euc.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwj.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kvd.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://wye.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://anz.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwd.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://csz.tanke756.top

TS:   同 JS
来源：http://fgw.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://hfw.svipenyu.cn

Go:   花括号块级作用域
来源：http://swa.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rds.cashguo.top

C#:   块级作用域
来源：http://ygn.c1oappe.top

[C11] 模块导入与导出
来源：http://zae.yj20258.top

Py:   from module import func
来源：http://ufk.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lmc.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://adf.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ute.jinqigfzy.top

Java: import java.util.List;
来源：http://vyz.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vik.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://ogl.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://aqx.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://qyn.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://oic.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://pep.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://nuz.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://jjs.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwp.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://qby.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://xnj.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nxl.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://aih.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jxf.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lhi.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://owp.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fyc.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dgo.cqqwz.cn

Go:   func add(a, b int) int
来源：http://llv.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gss.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ini.yanxiufei.cn

[C14] 泛型函数
来源：http://ktj.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zaz.mhx1999.top

PHP:  // 无泛型
来源：http://uyo.yj20258888.top

JS:   // 无泛型
来源：http://vgc.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mqn.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://whp.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbg.sxryk.cn

Ruby: # 无泛型
来源：http://tca.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gzi.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://vqf.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rju.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://nbc.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jfy.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ocs.yj20258.top

Java: // 无解构
来源：http://qjj.vehdjk.com

Go:   // 无解构
来源：http://duc.9152youxi.cn

Ruby: a, b = pair
来源：http://zvv.fengsongda.top

C#:   var (a, b) = pair;
来源：http://egt.xylfe.cn

[C16] 函数 / 方法重载
来源：http://prm.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pzd.shzxlz.cn

PHP:  // 无重载
来源：http://sve.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vkh.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://jkz.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ccv.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://amx.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://pbj.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cxl.ydzc1.top

================================================================================
来源：http://gfm.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://xnb.jyoumei.cn

================================================================================
来源：http://nyu.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://ibm.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yoc.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ayj.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bcw.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://sdh.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tnq.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://bpq.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://qty.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rbi.vehdjk.com

[D02] 追加元素到末尾
来源：http://wqd.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dko.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sqj.sweek.top

JS:   arr.push(4);
来源：http://dym.xuetiantiany.cn

TS:   arr.push(4);
来源：http://mlx.pycfn.com

Java: list.add(4);
来源：http://qry.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://uhv.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://lhf.pycfn.com

C#:   list.Add(4);
来源：http://rsz.yj20258888.top


<!-- 参考信息 -->