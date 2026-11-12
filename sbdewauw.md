代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uhj.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://txm.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://zmu.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://xao.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://ddk.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wds.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://ayh.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://iea.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://chl.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ejq.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://aev.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://hgi.hysaishi.cn

[B09] break 与 continue
来源：http://jux.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://krn.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lxn.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbd.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkf.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrr.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tlr.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aem.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byo.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://wyu.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qho.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tdn.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bcf.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://esf.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eoq.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dzf.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eks.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nnx.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://muu.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://nyd.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://ubh.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://doc.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxz.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olk.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dlo.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://srl.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ckp.ppjwa.cn

[B12] 跳出多层循环
来源：http://vkf.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wur.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbb.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxq.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpn.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mjt.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wkq.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pmg.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://spl.gotoacloud.top

[B13] 判断是否为数字
来源：http://ovd.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://ayp.havefunace.top

PHP:  is_numeric($x)
来源：http://tcc.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qac.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cla.yj20258888.top

Java: x instanceof Number
来源：http://wqc.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oew.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://ijw.cashguo.top

C#:   x is int or double or decimal
来源：http://mez.ybcxt.top

[B14] 判断值是否在集合内
来源：http://eot.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://scl.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ruz.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://gso.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://woy.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://akn.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zce.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://gkf.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jib.shuidangran.top

[B15] 布尔运算与取反
来源：http://ers.sufxvd.cn

Py:   a and b or not c
来源：http://vfb.daxiang520.top

PHP:  $a && $b || !$c
来源：http://cmi.yongpay.top

JS:   a && b || !c
来源：http://xhv.pycfn.com

TS:   a && b || !c
来源：http://hqc.daria6918.cn

Java: a && b || !c
来源：http://ynb.zdqjudy.top

Go:   a && b || !c
来源：http://glu.xylfe.cn

Ruby: a && b || !c
来源：http://ena.wangdashe.top

C#:   a && b || !c
来源：http://wmc.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cal.vehdjk.com

Py:   if not data: return
来源：http://oub.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://odg.sweek.top

JS:   if (!data) return;
来源：http://ygx.0kj1m.cn

TS:   if (!data) return;
来源：http://weo.xuetiantiany.cn

Java: if (data == null) return;
来源：http://xrg.zhixingplan.top

Go:   if data == nil { return }
来源：http://lzp.hammf.cn

Ruby: return if data.nil?
来源：http://jdr.zhengqikj.top

C#:   if (data == null) return;
来源：http://jwd.zhixingplan.top

================================================================================
来源：http://iic.yvedp.cn

C. 函数与作用域
来源：http://hyp.cheryme.top

================================================================================
来源：http://vdy.fehbvm.com

[C01] 定义函数
来源：http://kvu.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://pkl.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tys.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://toh.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqx.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://woe.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://csg.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://qlc.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kws.jianghu66.top

[C02] 默认参数
来源：http://ssb.uphjek.com

Py:   def greet(name="World"): return name
来源：http://ury.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bxv.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://prj.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fpu.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tew.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mhx.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://rff.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://wod.shanyushiyangkeji.top

[C03] 可变参数
来源：http://qwv.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://wgc.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qra.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbz.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://doa.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uca.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xmb.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://pfx.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pkg.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://gie.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gnp.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jdb.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://luv.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dnq.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://qes.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://jwc.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://qvo.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://jjq.fengsongda.top

[C05] 返回多个值
来源：http://qff.316326.xyz

Py:   return a, b
来源：http://mio.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://adx.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zhw.9152youxi.cn

TS:   return { a, b };
来源：http://eef.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ixl.zhoulong.xyz

Go:   return a, b
来源：http://zoa.316326.xyz

Ruby: return a, b
来源：http://kdi.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://zmb.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://qaf.yj202588.top

Py:   square = lambda x: x * x
来源：http://niy.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sqr.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://mnr.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://yls.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rdx.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://ify.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://cob.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://msc.gzhubu.top

[C07] 把函数作为参数传入
来源：http://mfi.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xnj.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vua.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mfq.hcnkem.com

TS:   arr.map(String)
来源：http://lpz.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzf.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvq.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://cln.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://swi.zycfv.cn

[C08] 闭包
来源：http://tza.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fqq.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jez.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vbx.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptw.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iqx.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fgz.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qmo.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gtz.jinghuilouyu.cn

[C09] 递归
来源：http://cvm.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yjk.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zvd.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nif.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkj.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kzj.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://muo.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rul.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dby.hcnkem.com

[C10] 变量作用域
来源：http://vvs.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xth.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ocx.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ipd.quarkkingdee.top

TS:   同 JS
来源：http://kik.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://ijb.nwbrower.top

Go:   花括号块级作用域
来源：http://hpk.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oaq.xylfe.cn

C#:   块级作用域
来源：http://kzm.gaohongyu789.top

[C11] 模块导入与导出
来源：http://gdv.hammf.cn

Py:   from module import func
来源：http://rsb.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hnh.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kgh.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jze.havefunace.top

Java: import java.util.List;
来源：http://wux.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lpm.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://ssu.ybcxt.top

C#:   using System.Text;
来源：http://mrx.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://rdu.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://eud.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://brq.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://xal.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://sxv.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ylf.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://njs.sweek.top

Ruby: -> { puts "run" }.call
来源：http://sht.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eei.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://gwi.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dlu.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syq.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzj.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbm.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uyw.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://daa.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yrb.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://fkc.zhengqikj.top

[C14] 泛型函数
来源：http://tgx.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://psv.sjlbkw.cn

PHP:  // 无泛型
来源：http://jzt.svipenyu.cn

JS:   // 无泛型
来源：http://yby.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kle.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://inn.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tex.tanke756.top

Ruby: # 无泛型
来源：http://gof.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bph.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://urv.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhx.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://alt.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wrq.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xbv.shangyingyoupin.top

Java: // 无解构
来源：http://ebp.hnxiangtu.top

Go:   // 无解构
来源：http://wis.c1oappe.top

Ruby: a, b = pair
来源：http://pej.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://bdt.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://zqi.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ypz.yfazqb.com

PHP:  // 无重载
来源：http://mpw.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hwt.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://eet.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qpd.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://pcy.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://wmw.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cyn.jinyuanbaomall.cn

================================================================================
来源：http://spn.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://xab.svipenyu.cn

================================================================================
来源：http://jiw.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://rcq.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://rak.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tzm.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hcl.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mlj.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vpy.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://vnn.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://ncw.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bfz.gzhubu.top

[D02] 追加元素到末尾
来源：http://lnn.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oxb.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vyf.hammf.cn

JS:   arr.push(4);
来源：http://wsv.jianghu66.top

TS:   arr.push(4);
来源：http://dua.ivvv.top

Java: list.add(4);
来源：http://ijs.316326.xyz

Go:   arr = append(arr, 4)
来源：http://brm.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://hdj.c1oappe.top

C#:   list.Add(4);
来源：http://cxw.andypj.xyz

[D03] 在指定位置插入元素
来源：http://kvj.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://ryq.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bxb.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lkr.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://qsz.fktsv.cn

Java: list.add(0, 0);
来源：http://xay.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://muf.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uun.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://ycv.yonumen.top

[D04] 删除元素
来源：http://orz.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vap.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://byd.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://usg.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://cwn.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://exp.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zwu.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xnv.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://srh.dianchejie.cn

[D05] 访问与修改元素
来源：http://lxj.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dwz.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://emj.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://khm.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://ely.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://igw.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://hhn.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqh.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lad.guannengcc.top

[D06] 数组长度
来源：http://hnv.hongshengwenyu.top

Py:   len(arr)
来源：http://dyv.aizwys.cn

PHP:  count($arr);
来源：http://qaf.shanyushiyangtech.top

JS:   arr.length
来源：http://zns.aibaodan.cn

TS:   arr.length
来源：http://dxy.epnwcf.com

Java: list.size();
来源：http://vdn.cucudq.cn

Go:   len(arr)
来源：http://iwa.hammf.cn

Ruby: arr.length; arr.size
来源：http://vie.sxryk.cn

C#:   list.Count;
来源：http://onw.jianghu66.top

[D07] 切片 / 取子数组
来源：http://tls.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpz.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://qdf.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://vpu.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://csh.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://luu.jinqigfzy.top

Go:   arr[1:4]
来源：http://afq.tarul.cn

Ruby: arr[1, 3]
来源：http://met.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://xdx.vehdjk.com

[D08] 合并两个数组
来源：http://oxj.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://vbx.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://ngh.guowangkeji.top


<!-- 参考信息 -->