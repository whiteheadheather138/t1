代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kfp.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybu.cucudq.cn

[B03] switch / match / case
来源：http://zsa.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cpa.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://skc.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gie.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wdy.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pwi.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uuy.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jcd.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ltz.andypj.xyz

[B04] for 计数循环
来源：http://vht.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://pat.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xrc.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mco.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://evo.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cwp.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vnq.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://yac.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iqg.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://nfw.hnqzz.top

Py:   for item in arr: print(item)
来源：http://mwn.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lrv.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://glr.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vai.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dgw.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sgr.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://yvs.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgv.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://lwx.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fhl.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kzu.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsv.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smj.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ykw.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nws.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gyy.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wqq.epnwcf.com

[B07] while 循环
来源：http://amc.xylfe.cn

Py:   while i < 10: i += 1
来源：http://oqi.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ejq.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://new.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://gqm.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://jjs.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kqp.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://ive.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://tks.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://cur.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://ncg.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qar.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://qqj.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://ydq.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://acn.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nbh.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://eqf.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://uiu.sysykeji.top

[B09] break 与 continue
来源：http://sud.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bqw.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqw.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdr.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znu.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxd.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iqw.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ffl.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjs.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://xud.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dxs.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hio.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zss.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cvp.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://efp.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vzp.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tud.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://naj.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://dan.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://uvc.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://wuy.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wuv.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzu.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qgn.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jcr.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://zmy.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zky.daxiang520.top

[B12] 跳出多层循环
来源：http://izz.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uap.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ctb.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vyk.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtt.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ivc.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vyc.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://klf.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dxm.quarkkingdee.top

[B13] 判断是否为数字
来源：http://ist.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://pdq.yfazqb.com

PHP:  is_numeric($x)
来源：http://rqj.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cva.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://myl.xuetiantiany.cn

Java: x instanceof Number
来源：http://eot.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hyw.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://qqw.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://gtf.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://cqc.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ikk.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wxu.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xna.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://atk.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yyv.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://isc.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://gmd.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kjk.hammf.cn

[B15] 布尔运算与取反
来源：http://uyy.zhiwuduotai.top

Py:   a and b or not c
来源：http://afd.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://rsk.gotoacloud.top

JS:   a && b || !c
来源：http://vtj.zdqjudy.top

TS:   a && b || !c
来源：http://eca.wangdashe.top

Java: a && b || !c
来源：http://zbn.fanxiaobao.xyz

Go:   a && b || !c
来源：http://uqz.redwolf501.top

Ruby: a && b || !c
来源：http://cfx.shanyushiyangtech.top

C#:   a && b || !c
来源：http://ztw.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://uok.yongpay.top

Py:   if not data: return
来源：http://mzt.tarul.cn

PHP:  if (!$data) { return; }
来源：http://bhp.fzhhl.top

JS:   if (!data) return;
来源：http://een.kuanghao11.cn

TS:   if (!data) return;
来源：http://gjx.xinyue.icu

Java: if (data == null) return;
来源：http://pyx.dianchejie.cn

Go:   if data == nil { return }
来源：http://gis.andypj.xyz

Ruby: return if data.nil?
来源：http://lew.xylfe.cn

C#:   if (data == null) return;
来源：http://cup.shangyingyoupin.top

================================================================================
来源：http://gca.hammf.cn

C. 函数与作用域
来源：http://eaa.yj20258888.top

================================================================================
来源：http://gid.bjfxy.top

[C01] 定义函数
来源：http://dji.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://iqb.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fua.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://gwv.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pge.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qzj.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://vfq.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://ttm.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwo.zhengqikj.top

[C02] 默认参数
来源：http://mwk.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://lem.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pzj.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://qdy.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ncf.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tri.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qoh.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://lyj.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://wtp.hammf.cn

[C03] 可变参数
来源：http://qyz.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://ooe.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxs.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmv.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kls.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ydu.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://njs.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://mgx.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xjh.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://wsm.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dcv.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qxy.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xdh.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dwj.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://hyo.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://uji.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://fgh.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://cab.jinqigfzy.top

[C05] 返回多个值
来源：http://hkl.yuxming.cn

Py:   return a, b
来源：http://wsz.andypj.xyz

PHP:  return [$a, $b];
来源：http://taj.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nuw.cdnleiting.top

TS:   return { a, b };
来源：http://tos.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jfr.sysykeji.top

Go:   return a, b
来源：http://ddq.bbcook.cn

Ruby: return a, b
来源：http://zhm.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://fcd.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://ekv.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://vvq.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://icm.xylfe.cn

JS:   const square = x => x * x;
来源：http://xqh.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://usj.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nqg.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xiq.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://ncw.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oak.uphjek.com

[C07] 把函数作为参数传入
来源：http://fhd.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kqi.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://mkr.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hib.316326.xyz

TS:   arr.map(String)
来源：http://xpc.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://anm.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qry.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://jgh.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lsb.zhongyouzk.top

[C08] 闭包
来源：http://nks.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tmo.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gkh.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ict.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gav.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yyj.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xpt.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://euz.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mvo.nanxuanxn.top

[C09] 递归
来源：http://yac.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dsx.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ida.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtq.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://isz.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ald.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://psd.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sff.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nsc.fktsv.cn

[C10] 变量作用域
来源：http://rfp.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dlc.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gjz.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yls.guowangkeji.top

TS:   同 JS
来源：http://yst.aizwys.cn

Java: 方法内为块级作用域
来源：http://rtq.jinqigufen.top

Go:   花括号块级作用域
来源：http://uhk.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tzf.yj20258.top

C#:   块级作用域
来源：http://lgw.9152youxi.cn

[C11] 模块导入与导出
来源：http://vlp.shuidangran.top

Py:   from module import func
来源：http://tuq.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://csr.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kbf.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://faw.aibaodan.cn

Java: import java.util.List;
来源：http://pbj.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hfg.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://zvi.chenlongwang.top

C#:   using System.Text;
来源：http://rkk.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://dgq.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://bgt.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://oja.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://qdv.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://avp.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xof.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://uzv.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://csq.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cwd.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://lxg.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eox.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkf.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkz.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwr.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://rqk.cheryme.top

Go:   func add(a, b int) int
来源：http://cnx.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://llk.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://oyc.jqgufenzy.top

[C14] 泛型函数
来源：http://omc.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bab.tianlin.xyz

PHP:  // 无泛型
来源：http://kzi.yvedp.cn

JS:   // 无泛型
来源：http://iov.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbu.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ccx.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hpw.wangdashe.top

Ruby: # 无泛型
来源：http://ynr.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://egx.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://tfy.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hyr.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://kvj.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bfb.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rzi.xingfuxueyuan.xyz

Java: // 无解构
来源：http://eww.quarkkingdee.top

Go:   // 无解构
来源：http://rda.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://ngs.yuxming.cn

C#:   var (a, b) = pair;
来源：http://zgg.fktsv.cn

[C16] 函数 / 方法重载
来源：http://pug.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://acu.hcnkem.com

PHP:  // 无重载
来源：http://ytz.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jzd.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://ifh.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dwj.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://epb.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://bks.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vgu.ybcxt.top

================================================================================
来源：http://cxb.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://cwo.quarkkingdee.top

================================================================================
来源：http://xic.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://ubp.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://umw.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qbk.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fzz.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wul.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zvn.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://usc.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://ujm.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bua.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://iog.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://psc.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gcw.bjfxy.top

JS:   arr.push(4);
来源：http://svw.yj20258888.top

TS:   arr.push(4);
来源：http://luu.sysykeji.top

Java: list.add(4);
来源：http://spr.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://efe.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://dav.tarul.cn

C#:   list.Add(4);
来源：http://yah.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://dff.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://wge.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ewk.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rht.jinqigufen.top


<!-- 参考信息 -->