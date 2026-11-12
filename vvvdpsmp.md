代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kli.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mvh.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://xmx.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ctj.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://ijy.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://thd.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ycf.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://udk.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hsl.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cja.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aen.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://ycl.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fyi.hammf.cn

[B06] 遍历字典 / 对象
来源：http://owb.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tpf.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vak.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtc.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aki.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qlh.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gsq.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dho.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://krj.shanyushiyangtech.top

[B07] while 循环
来源：http://ypy.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://vrf.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://cge.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://hhd.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://hmi.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://irn.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sec.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://uiq.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://tob.cashguo.top

[B08] do-while（至少执行一次）
来源：http://voc.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://qys.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://lln.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://ufy.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://sbb.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://njh.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pnk.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rhf.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://kgv.uphjek.com

[B09] break 与 continue
来源：http://mpy.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://isq.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uki.feifeiyinyue.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpp.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrf.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzv.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wmu.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lkh.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbt.yfazqb.com

[B10] 遍历同时拿索引
来源：http://uvl.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkh.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mst.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gmy.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kxd.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baz.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://avb.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xnz.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ypb.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://sds.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://uhh.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://tjw.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iqe.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jfl.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rcc.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kjd.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://ukl.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wtz.xinyue.icu

[B12] 跳出多层循环
来源：http://utt.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://udi.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hjn.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wwk.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://arz.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xip.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gcp.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://srm.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mpy.nanxinkj.top

[B13] 判断是否为数字
来源：http://cgp.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://vfb.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://tch.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcf.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iom.wangshuangyany.cn

Java: x instanceof Number
来源：http://ydt.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kml.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://lcr.yvedp.cn

C#:   x is int or double or decimal
来源：http://wrt.pycfn.com

[B14] 判断值是否在集合内
来源：http://esx.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lyn.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://emk.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://lgh.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://kxx.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://avm.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xvc.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://vij.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qgo.tian-w.cn

[B15] 布尔运算与取反
来源：http://pti.haohaochexian.top

Py:   a and b or not c
来源：http://ndr.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://ujq.yj202588.top

JS:   a && b || !c
来源：http://aiv.iojbl.cn

TS:   a && b || !c
来源：http://tmd.jiagoushi.top

Java: a && b || !c
来源：http://clg.nanxinkj.top

Go:   a && b || !c
来源：http://dfc.sufxvd.cn

Ruby: a && b || !c
来源：http://jra.andypj.xyz

C#:   a && b || !c
来源：http://bcq.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://voh.andypj.xyz

Py:   if not data: return
来源：http://czr.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://hco.zhijiandao.cn

JS:   if (!data) return;
来源：http://zuy.zhixingplan.top

TS:   if (!data) return;
来源：http://zbu.guannengcc.top

Java: if (data == null) return;
来源：http://hcg.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://nqw.zdqjudy.top

Ruby: return if data.nil?
来源：http://krr.fzhhl.top

C#:   if (data == null) return;
来源：http://usu.ppjwa.cn

================================================================================
来源：http://ioc.yvedp.cn

C. 函数与作用域
来源：http://gmf.shangyingyoupin.top

================================================================================
来源：http://ohv.fanxiaobao.xyz

[C01] 定义函数
来源：http://cug.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://bpd.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkh.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://ndq.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ouq.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uvz.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tjn.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://uvq.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ezh.gzhubu.top

[C02] 默认参数
来源：http://elp.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://esr.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ife.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://vqu.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://txi.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ryn.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kst.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://cfl.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://bjs.xziqi.cn

[C03] 可变参数
来源：http://pep.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://ans.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://loq.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dcy.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://crn.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wqh.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wti.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://wcb.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://moc.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://qnq.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dww.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vcr.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vdl.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkp.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://uwq.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://she.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://syf.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://pwx.zdqjudy.top

[C05] 返回多个值
来源：http://eil.zdbjq.cn

Py:   return a, b
来源：http://tin.aibaodan.cn

PHP:  return [$a, $b];
来源：http://ojq.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://grp.vehdjk.com

TS:   return { a, b };
来源：http://yqx.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://niy.ywan-chungtsiang.top

Go:   return a, b
来源：http://jta.jinqigfzy.top

Ruby: return a, b
来源：http://uvy.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://pmy.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://whg.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://lma.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rcn.chenlongwang.top

JS:   const square = x => x * x;
来源：http://beq.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://rzz.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pft.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://uwp.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://ypg.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://rwy.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://ame.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jiz.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ops.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lkc.birdmap.top

TS:   arr.map(String)
来源：http://ewr.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vxx.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jkw.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://zfo.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://lrs.zdqjudy.top

[C08] 闭包
来源：http://qnu.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hri.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xaj.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qzj.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uyf.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btw.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jix.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ean.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://twq.epnwcf.com

[C09] 递归
来源：http://izy.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xtw.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fxt.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqd.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lek.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kdi.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eha.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lrk.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://knz.yj20258888.top

[C10] 变量作用域
来源：http://pib.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gzp.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pfs.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dkb.meibo888.top

TS:   同 JS
来源：http://nkr.sufxvd.cn

Java: 方法内为块级作用域
来源：http://nuk.tarul.cn

Go:   花括号块级作用域
来源：http://qzg.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pqs.pycfn.com

C#:   块级作用域
来源：http://xwc.fehbvm.com

[C11] 模块导入与导出
来源：http://hdj.nwbrower.top

Py:   from module import func
来源：http://ogo.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dgr.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ble.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://klo.hnxiangtu.top

Java: import java.util.List;
来源：http://zjx.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lvd.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://iwv.nanxuanxn.top

C#:   using System.Text;
来源：http://scf.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://ynd.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://ayl.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://gbu.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://yrr.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://tvq.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cii.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://xjk.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://pwr.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://svk.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://njo.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ebq.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ttv.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sgi.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxf.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://prc.bbcook.cn

Go:   func add(a, b int) int
来源：http://sio.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://svz.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://bfz.jiagoushi.top

[C14] 泛型函数
来源：http://aqh.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://plh.aibaodan.cn

PHP:  // 无泛型
来源：http://zxy.jianghu66.top

JS:   // 无泛型
来源：http://haa.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pah.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jfw.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jbm.haohaochexian.top

Ruby: # 无泛型
来源：http://exv.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xmy.ydzc1.top

[C15] 解构 / 展开参数
来源：http://fxd.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rjf.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://tmb.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kkg.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kcw.guowangkeji.top

Java: // 无解构
来源：http://pjs.redwolf501.top

Go:   // 无解构
来源：http://xox.tanke756.top

Ruby: a, b = pair
来源：http://abw.fktsv.cn

C#:   var (a, b) = pair;
来源：http://dnb.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://mti.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rai.xinyue.icu

PHP:  // 无重载
来源：http://jng.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qro.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://kpb.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xcg.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://huu.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://vfd.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wgr.gogol.net.cn

================================================================================
来源：http://rnu.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://bft.ywan-chungtsiang.top

================================================================================
来源：http://ifh.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://ulo.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://gcl.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oaq.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://trg.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cbi.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://brz.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://xxa.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://rxi.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ymo.ivvv.top

[D02] 追加元素到末尾
来源：http://bva.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ugx.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ajs.yj202588.top

JS:   arr.push(4);
来源：http://peq.yfazqb.com

TS:   arr.push(4);
来源：http://hpa.zhoulong.xyz

Java: list.add(4);
来源：http://zwn.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://prv.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://sjk.0kj1m.cn

C#:   list.Add(4);
来源：http://ndt.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://yyw.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://bwa.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dmj.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ach.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://hzn.fehbvm.com

Java: list.add(0, 0);
来源：http://trg.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ytu.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dwo.ivvv.top

C#:   list.Insert(0, 0);
来源：http://eei.havefunace.top

[D04] 删除元素
来源：http://kpy.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wkx.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zkh.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wae.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://hra.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lcd.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jho.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bjb.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tqt.aibaodan.cn

[D05] 访问与修改元素
来源：http://lwn.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kgw.sysykeji.top


<!-- 参考信息 -->