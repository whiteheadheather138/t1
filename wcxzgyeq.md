代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wym.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gwk.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://udu.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://wct.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://gyz.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tqf.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://cif.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://qyj.hesvh.cn

[B09] break 与 continue
来源：http://nyq.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kgy.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wxp.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amy.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnd.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqw.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bca.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gdo.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nyw.iojbl.cn

[B10] 遍历同时拿索引
来源：http://zoh.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fwr.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ljl.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dnu.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pkl.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ydh.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://anw.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mon.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yoi.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ncz.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://kyj.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://hrn.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://phj.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tpg.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zhs.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ixp.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://vww.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ujx.guowangkeji.top

[B12] 跳出多层循环
来源：http://ame.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://urt.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vvl.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vcr.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkt.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vzz.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://puq.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://loz.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ubg.sxryk.cn

[B13] 判断是否为数字
来源：http://maj.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://qeq.cqqwz.cn

PHP:  is_numeric($x)
来源：http://kor.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ome.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aaf.zhoulong.xyz

Java: x instanceof Number
来源：http://jyu.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qrr.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://dir.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://alz.havefunace.top

[B14] 判断值是否在集合内
来源：http://ivo.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vzy.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://som.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://zis.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://izh.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://spd.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://byb.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pva.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zyc.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://cwy.cashguo.top

Py:   a and b or not c
来源：http://gng.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://vpx.birdmap.top

JS:   a && b || !c
来源：http://ngg.chenjidiqi.icu

TS:   a && b || !c
来源：http://ato.316326.xyz

Java: a && b || !c
来源：http://xvw.kuanghao11.cn

Go:   a && b || !c
来源：http://ekf.gaohongyu789.top

Ruby: a && b || !c
来源：http://kng.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://jkt.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tpt.ivvv.top

Py:   if not data: return
来源：http://wva.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://hvm.cucudq.cn

JS:   if (!data) return;
来源：http://kfr.zhixingplan.top

TS:   if (!data) return;
来源：http://ksb.ppjwa.cn

Java: if (data == null) return;
来源：http://ilt.hammf.cn

Go:   if data == nil { return }
来源：http://rku.cheryme.top

Ruby: return if data.nil?
来源：http://yze.jinqigufen.top

C#:   if (data == null) return;
来源：http://tlb.316326.xyz

================================================================================
来源：http://fmc.shanyushiyangtech.top

C. 函数与作用域
来源：http://jkq.zhixingplan.top

================================================================================
来源：http://mrv.nanxuanxn.top

[C01] 定义函数
来源：http://izo.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://lmn.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ysv.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://zdh.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lkw.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tel.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cdv.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://lkg.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mvo.zhixingplan.top

[C02] 默认参数
来源：http://tlt.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://xow.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xve.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://xiz.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://flj.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://upc.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nik.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://aou.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nxc.fanxiaobao.xyz

[C03] 可变参数
来源：http://pta.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://mqe.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tjz.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xjz.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgd.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uqm.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zld.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://itm.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qsc.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://vmt.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iia.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vbs.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://flp.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wnc.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://qom.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://hxd.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://bgz.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://jdc.ppjwa.cn

[C05] 返回多个值
来源：http://sht.ivvv.top

Py:   return a, b
来源：http://vhp.yueranfly.top

PHP:  return [$a, $b];
来源：http://sck.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fvc.sxryk.cn

TS:   return { a, b };
来源：http://dti.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://siq.xuetiantiany.cn

Go:   return a, b
来源：http://gaz.gzhubu.top

Ruby: return a, b
来源：http://ubu.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://vfd.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://tcz.yj20258.top

Py:   square = lambda x: x * x
来源：http://irf.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://imj.jiagoushi.top

JS:   const square = x => x * x;
来源：http://glh.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://qoh.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://czm.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://xic.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://ppo.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://aow.nwbrower.top

[C07] 把函数作为参数传入
来源：http://xfw.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jjq.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ryp.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mdo.wangdashe.top

TS:   arr.map(String)
来源：http://hfy.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fzj.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iaj.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://ufv.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zsu.ivvv.top

[C08] 闭包
来源：http://het.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rzf.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wyz.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cho.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hdy.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xfr.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oot.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gko.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dsx.yangfankeji.com

[C09] 递归
来源：http://haw.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zee.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oyy.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjk.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://trz.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://plg.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rjc.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbq.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rzt.hnqzz.top

[C10] 变量作用域
来源：http://zoa.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qiy.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://luz.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mzy.jinqigfzy.top

TS:   同 JS
来源：http://kgj.xylfe.cn

Java: 方法内为块级作用域
来源：http://zsk.shzxlz.cn

Go:   花括号块级作用域
来源：http://fdz.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zte.jyoumei.cn

C#:   块级作用域
来源：http://bge.52xcode.cn

[C11] 模块导入与导出
来源：http://bnk.xylfe.cn

Py:   from module import func
来源：http://xuz.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rbx.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fjk.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmd.hysaishi.cn

Java: import java.util.List;
来源：http://ube.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eum.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://sif.jinqigufen.top

C#:   using System.Text;
来源：http://hhn.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://kez.hfpthk.cn

Py:   (lambda: print("run"))()
来源：http://qun.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://qpz.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://ssf.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://khq.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://deu.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://xly.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://pha.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://knk.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://rbi.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kbp.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghz.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xvo.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://icn.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://wqm.gogol.net.cn

Go:   func add(a, b int) int
来源：http://cgy.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kmc.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://viy.sweek.top

[C14] 泛型函数
来源：http://ytr.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sho.fktsv.cn

PHP:  // 无泛型
来源：http://hxc.havefunace.top

JS:   // 无泛型
来源：http://jkj.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dwr.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ayq.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uyz.guowangkeji.top

Ruby: # 无泛型
来源：http://lwf.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gcr.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://rhy.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vsz.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://zdu.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jws.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xvc.shuidangran.top

Java: // 无解构
来源：http://ida.ydzc1.top

Go:   // 无解构
来源：http://oqc.sjlbkw.cn

Ruby: a, b = pair
来源：http://vqz.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://nhq.52xcode.cn

[C16] 函数 / 方法重载
来源：http://dek.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fwb.jinqigufen.top

PHP:  // 无重载
来源：http://cto.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qky.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://fgh.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://apu.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://tck.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://fub.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hip.smart0.xyz

================================================================================
来源：http://sam.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://doq.yj20258.top

================================================================================
来源：http://ngm.wangdashe.top

[D01] 创建数组 / 列表
来源：http://img.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gfb.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bvq.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oii.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lfq.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ukz.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://bas.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://vrs.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://arw.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://rzr.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ygj.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fhq.iojbl.cn

JS:   arr.push(4);
来源：http://tye.wangshuangyany.cn

TS:   arr.push(4);
来源：http://kof.jqgufenzy.top

Java: list.add(4);
来源：http://hkw.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://rav.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xpq.yonumen.top

C#:   list.Add(4);
来源：http://syh.sweek.top

[D03] 在指定位置插入元素
来源：http://cvj.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://tkx.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gwo.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qzq.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://okg.guowangkeji.top

Java: list.add(0, 0);
来源：http://emj.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://jgq.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qhg.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://xzt.epnwcf.com

[D04] 删除元素
来源：http://cgs.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dlr.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mwy.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://duj.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://uxq.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ysl.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vln.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eea.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tog.zhengqikj.top

[D05] 访问与修改元素
来源：http://kie.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tem.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vxa.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gou.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://vqq.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://wdc.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://gzm.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://llf.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ymx.hnxiangtu.top

[D06] 数组长度
来源：http://sdj.iojbl.cn

Py:   len(arr)
来源：http://mfl.hongshengwenyu.top

PHP:  count($arr);
来源：http://adz.snrcjt.cn

JS:   arr.length
来源：http://hkq.chenjidiqi.icu

TS:   arr.length
来源：http://lcm.yongpay.top

Java: list.size();
来源：http://hwa.tarul.cn

Go:   len(arr)
来源：http://pdh.yvedp.cn

Ruby: arr.length; arr.size
来源：http://fgk.quarkkingdee.top

C#:   list.Count;
来源：http://mvn.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://eow.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yog.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://zye.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://cmo.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://dbr.nanxinkj.top

Java: list.subList(1, 4);
来源：http://kht.bjfxy.top

Go:   arr[1:4]
来源：http://oyx.cucudq.cn

Ruby: arr[1, 3]
来源：http://vyd.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://tji.dianchejie.cn

[D08] 合并两个数组
来源：http://bxs.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://yer.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://ana.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pee.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://dsz.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mwc.hnqzz.top

Go:   append(a, b...)
来源：http://naj.nwbrower.top


<!-- 参考信息 -->