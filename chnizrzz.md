代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nup.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jtt.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://ymm.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dkb.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://por.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://ctx.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xcb.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ixl.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rva.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vud.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://atp.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://qal.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kms.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://qge.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ekn.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nuq.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qgz.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mjw.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ucz.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mvh.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://evj.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwu.tian-w.cn

[B07] while 循环
来源：http://yyt.bbcook.cn

Py:   while i < 10: i += 1
来源：http://sll.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ofy.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://fqe.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://wev.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://orv.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ovr.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://xpz.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://wef.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://ehl.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://lte.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://als.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://wxk.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://ite.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://wgb.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wna.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://kwu.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://oop.ppjwa.cn

[B09] break 与 continue
来源：http://mzj.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tbi.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hln.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dvr.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msp.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twz.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dvt.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aea.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmh.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://ojx.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ofn.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wam.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://izm.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mif.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uia.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ltl.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kue.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nsx.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://lqg.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://teq.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://bjx.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocj.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgg.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kxo.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vqq.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://guk.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://omb.xinyue.icu

[B12] 跳出多层循环
来源：http://gax.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://rhc.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kdk.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fkp.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://amu.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tdv.c1oappe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vig.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eqq.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nub.chenlongwang.top

[B13] 判断是否为数字
来源：http://nvl.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://yjw.birdmap.top

PHP:  is_numeric($x)
来源：http://euv.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://atg.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zmb.hnxiangtu.top

Java: x instanceof Number
来源：http://akm.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vpz.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://fzs.tarul.cn

C#:   x is int or double or decimal
来源：http://bho.yueranfly.top

[B14] 判断值是否在集合内
来源：http://ydh.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gjz.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://igd.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://ntr.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://mcx.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qnz.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://moe.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://afl.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rii.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://fhs.havefunace.top

Py:   a and b or not c
来源：http://yko.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://dsa.zhongyouzk.top

JS:   a && b || !c
来源：http://rpl.sxryk.cn

TS:   a && b || !c
来源：http://dyd.mhx1999.top

Java: a && b || !c
来源：http://zdd.haohaochexian.top

Go:   a && b || !c
来源：http://ikg.aizwys.cn

Ruby: a && b || !c
来源：http://pbx.ybcxt.top

C#:   a && b || !c
来源：http://vzi.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://skx.dianchejie.cn

Py:   if not data: return
来源：http://afn.uphjek.com

PHP:  if (!$data) { return; }
来源：http://kix.nanxuanxn.top

JS:   if (!data) return;
来源：http://ggb.hfpthk.cn

TS:   if (!data) return;
来源：http://lcg.svipenyu.cn

Java: if (data == null) return;
来源：http://bfe.yongpay.top

Go:   if data == nil { return }
来源：http://tlg.vqdsnc.cn

Ruby: return if data.nil?
来源：http://woc.meibo888.top

C#:   if (data == null) return;
来源：http://xyv.zhengqikj.top

================================================================================
来源：http://jlf.zhixingplan.top

C. 函数与作用域
来源：http://oxu.zhixingplan.top

================================================================================
来源：http://quy.chenzaomai.com

[C01] 定义函数
来源：http://qyt.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://glo.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvd.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://wdj.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcd.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bwx.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://huu.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://qpg.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jzs.pycfn.com

[C02] 默认参数
来源：http://oqd.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://qjg.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://rxy.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://efj.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://udu.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uwv.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ktf.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://ubq.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://hfm.hongshengwenyu.top

[C03] 可变参数
来源：http://ywt.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://dcn.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xit.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzk.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hcg.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ehu.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qke.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://czw.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sun.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://stl.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gvb.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwj.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ene.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wtk.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://fph.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://swl.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://zfn.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://sjk.yongpay.top

[C05] 返回多个值
来源：http://rav.pycfn.com

Py:   return a, b
来源：http://zmf.tanke756.top

PHP:  return [$a, $b];
来源：http://xtc.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://zyq.aizwys.cn

TS:   return { a, b };
来源：http://klw.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://clb.tian-w.cn

Go:   return a, b
来源：http://zyh.zhongyouzk.top

Ruby: return a, b
来源：http://fhu.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://goh.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://bgt.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://qgi.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://zjs.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://wyg.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://mrn.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xyp.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jse.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://zuw.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://wwr.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://wuo.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gbs.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://uny.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bht.cheryme.top

TS:   arr.map(String)
来源：http://glu.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwo.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yxm.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://bxn.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tip.sweek.top

[C08] 闭包
来源：http://vjh.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xrh.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zuu.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://car.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dzv.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qlz.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zht.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iit.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nat.shzxlz.cn

[C09] 递归
来源：http://bws.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wqe.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uye.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jfd.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wuf.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikq.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jbq.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dmt.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxq.vehdjk.com

[C10] 变量作用域
来源：http://jma.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nwm.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xue.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://agt.cashguo.top

TS:   同 JS
来源：http://mfn.guannengcc.top

Java: 方法内为块级作用域
来源：http://zbk.sysykeji.top

Go:   花括号块级作用域
来源：http://lqq.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sss.jqgufenzy.top

C#:   块级作用域
来源：http://yhf.nanxuanxn.top

[C11] 模块导入与导出
来源：http://zbf.shanyushiyangkeji.top

Py:   from module import func
来源：http://ngo.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eox.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ulf.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wdy.shuidangran.top

Java: import java.util.List;
来源：http://arb.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hji.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wwj.xinyue.icu

C#:   using System.Text;
来源：http://tat.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://jmu.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://hqa.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://esc.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://ntl.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://mtr.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lih.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://vch.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://otu.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ugi.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://knw.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ngk.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qea.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fgg.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qjl.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://wwa.vehdjk.com

Go:   func add(a, b int) int
来源：http://ntx.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htc.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://zxs.tarul.cn

[C14] 泛型函数
来源：http://dal.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lgi.haohaochexian.top

PHP:  // 无泛型
来源：http://pti.fengsongda.top

JS:   // 无泛型
来源：http://fpb.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dce.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tvz.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wfv.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://wnq.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gah.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://nvb.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://isv.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://ubi.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zad.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pkd.shangyingyoupin.top

Java: // 无解构
来源：http://ofq.sysykeji.top

Go:   // 无解构
来源：http://oho.jinqigufen.top

Ruby: a, b = pair
来源：http://ixs.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://cuy.yj20258888.top

[C16] 函数 / 方法重载
来源：http://jeh.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oja.shuidangran.top

PHP:  // 无重载
来源：http://egz.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qwv.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://nlx.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ixw.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://ugz.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://bjf.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mvc.ydzc1.top

================================================================================
来源：http://xpn.birdmap.top

D. 数组 / 列表 / 集合
来源：http://xam.ivvv.top

================================================================================
来源：http://cbl.pycfn.com

[D01] 创建数组 / 列表
来源：http://xsi.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bum.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rog.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sld.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://pmm.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aqx.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://tmr.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://rvv.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jsa.iojbl.cn

[D02] 追加元素到末尾
来源：http://gct.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qnv.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://foe.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://nhm.tanke756.top

TS:   arr.push(4);
来源：http://eob.fanxiaobao.xyz

Java: list.add(4);
来源：http://ldi.cashguo.top

Go:   arr = append(arr, 4)
来源：http://kdl.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://djo.zdqjudy.top

C#:   list.Add(4);
来源：http://jtn.cucudq.cn

[D03] 在指定位置插入元素
来源：http://pfj.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ckm.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wai.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zqh.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://snb.ivvv.top

Java: list.add(0, 0);
来源：http://ybf.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://huv.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ewn.sweek.top

C#:   list.Insert(0, 0);
来源：http://nen.aibaodan.cn

[D04] 删除元素
来源：http://bbc.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://swk.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hpg.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gga.yongpay.top

TS:   arr.splice(0, 1);
来源：http://yke.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksi.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yxo.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dju.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pwv.birdmap.top

[D05] 访问与修改元素
来源：http://ifc.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uyr.shanyushiyangtech.top


<!-- 参考信息 -->