代发 wailian999

Py:   for i in range(10): print(i)
来源：http://bmj.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iob.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://met.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umr.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cfn.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lib.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://ytv.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://avf.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://gaq.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://xqr.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bph.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kma.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ojm.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rtf.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ivt.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://mfr.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ujp.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://fqa.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pkj.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tom.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rnf.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xtp.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hyj.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xdb.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xlx.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://auf.guowangkeji.top

[B07] while 循环
来源：http://gwv.fzhhl.top

Py:   while i < 10: i += 1
来源：http://hft.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nyc.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://ylp.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://pra.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://ueb.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rkp.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://ylp.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://tjt.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://ojs.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://syh.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://irw.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://mrm.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://dep.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://nqr.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://inl.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://dam.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://ilc.tian-w.cn

[B09] break 与 continue
来源：http://ymp.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pqd.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dua.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hae.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxu.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dez.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vbu.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xrk.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ido.yfazqb.com

[B10] 遍历同时拿索引
来源：http://gyb.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gjo.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hip.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nfx.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vic.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jnf.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zgf.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hmv.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vne.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://aqo.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://xoi.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://scl.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fiw.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjt.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sji.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxv.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://etx.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hoo.gaohongyu789.top

[B12] 跳出多层循环
来源：http://jxu.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xlx.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nrb.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyu.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bvd.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ump.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xqe.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gbj.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gtr.fengsongda.top

[B13] 判断是否为数字
来源：http://hjp.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://foa.jiagoushi.top

PHP:  is_numeric($x)
来源：http://bcx.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aet.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgk.guowangkeji.top

Java: x instanceof Number
来源：http://swr.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qqn.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://gml.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://irp.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://xis.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fby.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fcf.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://mye.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://mxz.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ucj.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sfn.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://tal.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kij.9152youxi.cn

[B15] 布尔运算与取反
来源：http://uty.dianchejie.cn

Py:   a and b or not c
来源：http://gjb.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://pae.hammf.cn

JS:   a && b || !c
来源：http://djs.bjfxy.top

TS:   a && b || !c
来源：http://tyh.fengsongda.top

Java: a && b || !c
来源：http://bjh.jyoumei.cn

Go:   a && b || !c
来源：http://enb.jyoumei.cn

Ruby: a && b || !c
来源：http://hww.redwolf501.top

C#:   a && b || !c
来源：http://hlz.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jsf.yangfankeji.com

Py:   if not data: return
来源：http://zsu.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://fam.sxryk.cn

JS:   if (!data) return;
来源：http://ekx.chenjidiqi.icu

TS:   if (!data) return;
来源：http://ewc.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://evr.mhx1999.top

Go:   if data == nil { return }
来源：http://oxp.tianlin.xyz

Ruby: return if data.nil?
来源：http://xqn.svipenyu.cn

C#:   if (data == null) return;
来源：http://fyj.yuxming.cn

================================================================================
来源：http://cox.tianlin.xyz

C. 函数与作用域
来源：http://are.sufxvd.cn

================================================================================
来源：http://kic.dashuyun.cn

[C01] 定义函数
来源：http://yni.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://ebe.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkv.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://usv.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mph.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jom.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gsx.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://azs.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yys.vehdjk.com

[C02] 默认参数
来源：http://mwl.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://vau.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wgn.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://wyk.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eyu.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wym.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eaq.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://dct.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://sqq.pengpengdd.cyou

[C03] 可变参数
来源：http://wbm.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://cgi.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nhp.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hpv.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aaw.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gmd.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ihr.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tjx.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ivq.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://qbz.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://due.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mtl.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aoe.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qqu.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://gop.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://jir.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://gzp.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://ung.sufxvd.cn

[C05] 返回多个值
来源：http://opn.pycfn.com

Py:   return a, b
来源：http://xzw.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://tih.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wya.ehwqpu.com

TS:   return { a, b };
来源：http://tya.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ckj.ivvv.top

Go:   return a, b
来源：http://ego.sxryk.cn

Ruby: return a, b
来源：http://hcz.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yed.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://uez.316326.xyz

Py:   square = lambda x: x * x
来源：http://cxu.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vqb.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://oxx.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://ype.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uas.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://cin.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://ync.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jdn.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://slc.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jyq.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://ubt.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oco.cdnleiting.top

TS:   arr.map(String)
来源：http://aki.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dgp.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kmd.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://dfq.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yoc.zhongyouzk.top

[C08] 闭包
来源：http://pih.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cry.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ttz.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oez.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ner.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cce.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gll.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://whm.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kmp.guannengcc.top

[C09] 递归
来源：http://ova.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trf.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wxk.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvw.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://akq.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rsf.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tuj.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xel.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcu.bbcook.cn

[C10] 变量作用域
来源：http://lxx.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mlf.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jyf.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ijz.epnwcf.com

TS:   同 JS
来源：http://wtc.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://ugg.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://qvl.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yuh.yueranfly.top

C#:   块级作用域
来源：http://qnj.bjfxy.top

[C11] 模块导入与导出
来源：http://fuw.ydjk.org.cn

Py:   from module import func
来源：http://yli.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://isu.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xeb.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rzc.zhiwuduotai.top

Java: import java.util.List;
来源：http://bud.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ufp.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://mnp.pycfn.com

C#:   using System.Text;
来源：http://ppe.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://xac.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://vvd.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://flz.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://dmc.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://ogd.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tqz.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://ylz.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://yqj.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rei.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://azs.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xjt.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mky.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzh.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsi.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ves.shzxlz.cn

Go:   func add(a, b int) int
来源：http://ilu.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kbn.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://dgi.cashguo.top

[C14] 泛型函数
来源：http://yan.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hjr.ctjpmb.com

PHP:  // 无泛型
来源：http://ril.yfazqb.com

JS:   // 无泛型
来源：http://myu.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qic.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lzv.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwf.yvedp.cn

Ruby: # 无泛型
来源：http://rtr.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cfl.cashguo.top

[C15] 解构 / 展开参数
来源：http://bgc.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hom.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://kro.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mxg.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lry.yfazqb.com

Java: // 无解构
来源：http://kii.yuanzhike.top

Go:   // 无解构
来源：http://vhl.316326.xyz

Ruby: a, b = pair
来源：http://diw.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://psj.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://hab.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qgh.yuxming.cn

PHP:  // 无重载
来源：http://lkf.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vla.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://rhl.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jqk.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://ykp.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://vbs.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://def.dianchejie.cn

================================================================================
来源：http://tir.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://fsr.bbcook.cn

================================================================================
来源：http://byh.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://yer.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://tbg.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drx.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vhy.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qnv.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wwy.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://phd.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://smv.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ajj.yvedp.cn

[D02] 追加元素到末尾
来源：http://kuu.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qmz.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://him.zdbjq.cn

JS:   arr.push(4);
来源：http://feg.epnwcf.com

TS:   arr.push(4);
来源：http://uuv.zhijiandao.cn

Java: list.add(4);
来源：http://fcs.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://ayo.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ycr.cheryme.top

C#:   list.Add(4);
来源：http://ayd.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://sjy.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://msw.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cpk.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://czw.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://mvu.jianghu66.top

Java: list.add(0, 0);
来源：http://bvk.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://cxb.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://whc.uphjek.com

C#:   list.Insert(0, 0);
来源：http://dzp.hongshengwenyu.top

[D04] 删除元素
来源：http://gfr.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hzk.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ido.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ywi.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://sfk.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tgf.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mal.hfpthk.cn


<!-- 参考信息 -->