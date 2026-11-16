代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hsm.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cog.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ctz.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://sxh.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xld.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://tkn.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://svi.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cls.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://quj.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vyi.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sah.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aom.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ull.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ymj.cheryme.top

[B07] while 循环
来源：http://rvg.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://hmd.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://bin.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://wle.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://eoz.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://kzb.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cmv.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://kkq.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://opg.havefunace.top

[B08] do-while（至少执行一次）
来源：http://emq.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://qes.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ucv.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://qjd.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://xnd.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://tie.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jfo.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://ruy.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://ust.yj20258888.top

[B09] break 与 continue
来源：http://hso.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vmm.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cmt.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zob.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srb.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yiq.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hrc.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lwx.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhn.tanke756.top

[B10] 遍历同时拿索引
来源：http://kek.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hhp.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://drm.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hxy.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fuh.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bze.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ama.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uij.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lom.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://ess.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://end.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://ebo.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nfr.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qmh.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gsk.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yyy.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://jrk.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vwr.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://ovh.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dzq.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://spi.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpj.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kmr.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yll.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ltz.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://anr.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oee.gogol.net.cn

[B13] 判断是否为数字
来源：http://eew.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://srp.yuxming.cn

PHP:  is_numeric($x)
来源：http://cow.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yhb.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://das.zhengqikj.top

Java: x instanceof Number
来源：http://idy.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kdh.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://pzd.dashuyun.cn

C#:   x is int or double or decimal
来源：http://tyn.andypj.xyz

[B14] 判断值是否在集合内
来源：http://dln.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kdp.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wei.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://ker.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://krx.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://efk.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lco.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://jst.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gzq.dashuyun.cn

[B15] 布尔运算与取反
来源：http://osu.yueranfly.top

Py:   a and b or not c
来源：http://soh.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://evl.tianlin.xyz

JS:   a && b || !c
来源：http://rjx.xuetiantiany.cn

TS:   a && b || !c
来源：http://aye.meibo888.top

Java: a && b || !c
来源：http://awt.mhx1999.top

Go:   a && b || !c
来源：http://ddt.zhongyouzk.top

Ruby: a && b || !c
来源：http://edy.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://iun.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://gwr.cqqwz.cn

Py:   if not data: return
来源：http://drp.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://glu.gogol.net.cn

JS:   if (!data) return;
来源：http://nrt.andypj.xyz

TS:   if (!data) return;
来源：http://cju.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://jki.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://few.ydjk.org.cn

Ruby: return if data.nil?
来源：http://ctm.sxryk.cn

C#:   if (data == null) return;
来源：http://xsu.xziqi.cn

================================================================================
来源：http://qvp.kuanghao11.cn

C. 函数与作用域
来源：http://glu.cqqwz.cn

================================================================================
来源：http://sfv.gaohongyu789.top

[C01] 定义函数
来源：http://fsb.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://eoc.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mgc.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://ndt.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdz.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://cxm.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://slu.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://njn.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kwd.zhijiandao.cn

[C02] 默认参数
来源：http://rkm.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://ukb.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://muc.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://svb.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rxj.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://iox.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xmr.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://fro.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://hnp.shzxlz.cn

[C03] 可变参数
来源：http://ojr.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://ocx.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mzz.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oel.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pmp.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eid.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ecq.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bdg.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sxe.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://myd.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://weg.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gal.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kfq.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ltq.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://bpy.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://gwu.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://njo.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://lhu.zycfv.cn

[C05] 返回多个值
来源：http://hqh.smart0.xyz

Py:   return a, b
来源：http://fyi.tianlin.xyz

PHP:  return [$a, $b];
来源：http://lsr.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nkp.haohaochexian.top

TS:   return { a, b };
来源：http://gvc.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eum.fehbvm.com

Go:   return a, b
来源：http://htm.guannengcc.top

Ruby: return a, b
来源：http://lmm.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://uib.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://ijp.xziqi.cn

Py:   square = lambda x: x * x
来源：http://ejl.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pqd.tarul.cn

JS:   const square = x => x * x;
来源：http://xsu.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://lec.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ubb.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gqi.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://pai.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://jpc.yongpay.top

[C07] 把函数作为参数传入
来源：http://qxh.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lpz.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vlc.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sgb.ehwqpu.com

TS:   arr.map(String)
来源：http://jxv.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vec.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bxo.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://mhg.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ocp.pengpengdd.cyou

[C08] 闭包
来源：http://aok.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://upc.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mte.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fie.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jnh.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yck.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ate.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uhp.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yjp.mhx1999.top

[C09] 递归
来源：http://kym.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jru.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pms.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqs.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bzy.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lrg.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sec.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kgm.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://plu.zdbjq.cn

[C10] 变量作用域
来源：http://gob.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lju.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zyq.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yih.0kj1m.cn

TS:   同 JS
来源：http://dbl.cashguo.top

Java: 方法内为块级作用域
来源：http://mru.chenzaomai.com

Go:   花括号块级作用域
来源：http://iav.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cei.birdmap.top

C#:   块级作用域
来源：http://tmj.pycfn.com

[C11] 模块导入与导出
来源：http://cwh.wangshuangyany.cn

Py:   from module import func
来源：http://bnk.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xer.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zvl.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nbs.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://ecr.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zsi.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://fdq.c1oappe.top

C#:   using System.Text;
来源：http://qyb.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://dvd.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://qyg.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://osi.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://gvt.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://shy.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qyx.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hae.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://ccs.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://scj.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://imr.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dux.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnb.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tqe.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcf.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://nrj.dianchejie.cn

Go:   func add(a, b int) int
来源：http://une.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wga.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://gzx.guannengcc.top

[C14] 泛型函数
来源：http://rhj.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://boz.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://kne.xuanzx.com

JS:   // 无泛型
来源：http://vxv.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dmn.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uiz.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wnz.wangshuangyany.cn

Ruby: # 无泛型
来源：http://ibp.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://euu.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://pwk.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rnf.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://zke.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jnv.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iop.jianghu66.top

Java: // 无解构
来源：http://hus.yonumen.top

Go:   // 无解构
来源：http://zqw.daxiang520.top

Ruby: a, b = pair
来源：http://efi.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://mpk.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://izn.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oyo.jinqigfzy.top

PHP:  // 无重载
来源：http://cmh.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://chd.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://kuk.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://bph.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://otg.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://rnw.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dol.yuxming.cn

================================================================================
来源：http://gnc.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://hdl.cucudq.cn

================================================================================
来源：http://oir.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://pug.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oao.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vso.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cif.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xeb.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kry.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://sdy.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://syu.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://owd.fzhhl.top

[D02] 追加元素到末尾
来源：http://ied.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dna.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qkq.nwbrower.top

JS:   arr.push(4);
来源：http://dtd.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://lwd.ydzc1.top

Java: list.add(4);
来源：http://riv.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://mxi.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://gxc.dashuyun.cn

C#:   list.Add(4);
来源：http://idt.pycfn.com

[D03] 在指定位置插入元素
来源：http://ynb.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://mon.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ctn.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jvo.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://rwr.mhx1999.top

Java: list.add(0, 0);
来源：http://bxw.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://inp.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ucg.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://zse.guannengcc.top

[D04] 删除元素
来源：http://kvf.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tnn.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tsl.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wkd.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://amm.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ueo.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wuk.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://luj.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xgx.hysaishi.cn

[D05] 访问与修改元素
来源：http://rjz.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://crk.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yex.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mlg.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://rlf.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://wqn.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://eok.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hld.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pvl.tianlin.xyz

[D06] 数组长度
来源：http://chy.gotoacloud.top


<!-- 参考信息 -->