代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://ren.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://cie.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://dmi.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ode.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lzr.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://qhv.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://ree.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://afo.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://lnv.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://diz.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://cnp.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://vtn.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://bzl.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://irb.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://aic.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://tno.sysykeji.top

[B09] break 与 continue
来源：http://pbj.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xqb.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ycv.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mem.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieg.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfy.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vst.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kwj.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhq.fktsv.cn

[B10] 遍历同时拿索引
来源：http://juh.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jue.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bxg.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cwl.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aor.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jds.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jbj.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvj.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kkh.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://net.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://rzx.316326.xyz

PHP:  range(0, 10, 2);
来源：http://xrg.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dkq.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fnn.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rwn.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hjt.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://wiw.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bzj.ctjpmb.com

[B12] 跳出多层循环
来源：http://rep.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fjf.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bdg.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzk.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ixl.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ugf.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oey.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dfl.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://okq.daria6918.cn

[B13] 判断是否为数字
来源：http://eiv.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://cmx.tianlin.xyz

PHP:  is_numeric($x)
来源：http://kor.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vbs.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qti.jqgufenzy.top

Java: x instanceof Number
来源：http://xlb.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lyt.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://dnq.cheryme.top

C#:   x is int or double or decimal
来源：http://zaz.fktsv.cn

[B14] 判断值是否在集合内
来源：http://iuu.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://arb.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lfi.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://hff.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://wvx.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lwl.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqc.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://hcq.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://klh.gotoacloud.top

[B15] 布尔运算与取反
来源：http://skn.jinghuilouyu.cn

Py:   a and b or not c
来源：http://vtc.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://xxp.hesvh.cn

JS:   a && b || !c
来源：http://fpx.hcnkem.com

TS:   a && b || !c
来源：http://oom.zycfv.cn

Java: a && b || !c
来源：http://jug.svipenyu.cn

Go:   a && b || !c
来源：http://uhj.ctjpmb.com

Ruby: a && b || !c
来源：http://tqi.feifeiyinyue.top

C#:   a && b || !c
来源：http://emf.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hja.andypj.xyz

Py:   if not data: return
来源：http://coy.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://zoy.xuanzx.com

JS:   if (!data) return;
来源：http://ihr.yvedp.cn

TS:   if (!data) return;
来源：http://bhd.yueranfly.top

Java: if (data == null) return;
来源：http://abj.zhixingplan.top

Go:   if data == nil { return }
来源：http://dpe.yongpay.top

Ruby: return if data.nil?
来源：http://ych.yfazqb.com

C#:   if (data == null) return;
来源：http://wzw.zdbjq.cn

================================================================================
来源：http://rqp.ctjpmb.com

C. 函数与作用域
来源：http://yla.ydzc1.top

================================================================================
来源：http://swc.hywenlv.cn

[C01] 定义函数
来源：http://vsl.uphjek.com

Py:   def add(a, b): return a + b
来源：http://qiy.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://irv.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://asp.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ayn.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pgy.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yjd.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://rvj.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pjv.fengsongda.top

[C02] 默认参数
来源：http://jsa.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://qbt.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vpj.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://sxc.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xiu.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ioq.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baj.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://qcc.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://yky.shzxlz.cn

[C03] 可变参数
来源：http://kia.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://oke.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iqj.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lnr.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jdi.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ozq.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dye.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://hrd.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jxm.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://ksx.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpn.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mft.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jxu.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cjd.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://atn.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://qvf.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://qdd.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://tca.hnxiangtu.top

[C05] 返回多个值
来源：http://oqn.guowangkeji.top

Py:   return a, b
来源：http://msd.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://nxo.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wsa.meibo888.top

TS:   return { a, b };
来源：http://rde.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lif.mhx1999.top

Go:   return a, b
来源：http://uie.tian-w.cn

Ruby: return a, b
来源：http://bvp.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ird.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://vej.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://rkl.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jnd.316326.xyz

JS:   const square = x => x * x;
来源：http://nfj.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://kiy.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nsk.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://rey.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://dal.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://xcs.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://qah.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bml.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sev.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cfm.hesvh.cn

TS:   arr.map(String)
来源：http://azd.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://emk.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sod.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://wtq.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wov.zycfv.cn

[C08] 闭包
来源：http://vkl.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tis.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yku.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jdl.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ifp.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qdo.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcn.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lbc.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gds.zhixingplan.top

[C09] 递归
来源：http://vvb.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dya.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nux.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtd.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://all.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ota.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://anj.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kxt.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xft.svipenyu.cn

[C10] 变量作用域
来源：http://oow.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jkr.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ava.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rql.pycfn.com

TS:   同 JS
来源：http://ftz.hfpthk.cn

Java: 方法内为块级作用域
来源：http://csb.sjlbkw.cn

Go:   花括号块级作用域
来源：http://ium.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://web.ybcxt.top

C#:   块级作用域
来源：http://hgo.cqqwz.cn

[C11] 模块导入与导出
来源：http://ltp.shanyushiyangkeji.top

Py:   from module import func
来源：http://don.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jcl.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uzp.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rdm.hywenlv.cn

Java: import java.util.List;
来源：http://ipc.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjp.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://qye.tian-w.cn

C#:   using System.Text;
来源：http://rvk.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://ika.yonumen.top

Py:   (lambda: print("run"))()
来源：http://vhv.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://oww.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://myl.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://btq.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bqr.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://qff.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://jgr.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://luj.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://ldf.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://azo.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nlk.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zih.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxz.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jva.bbcook.cn

Go:   func add(a, b int) int
来源：http://bei.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ugf.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://wxt.yj20258.top

[C14] 泛型函数
来源：http://lva.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vze.jqgfzy.top

PHP:  // 无泛型
来源：http://tsv.316326.xyz

JS:   // 无泛型
来源：http://bml.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fnk.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://crk.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ecl.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://zia.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ado.sweek.top

[C15] 解构 / 展开参数
来源：http://dsb.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qll.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://gln.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rhe.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fxf.jinqigufen.top

Java: // 无解构
来源：http://gvo.svipenyu.cn

Go:   // 无解构
来源：http://cfy.xinyue.icu

Ruby: a, b = pair
来源：http://jha.yfazqb.com

C#:   var (a, b) = pair;
来源：http://rya.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://qoe.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://izz.guowangkeji.top

PHP:  // 无重载
来源：http://jhk.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://acr.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://kvn.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bry.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://ulo.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://vyn.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ekt.redwolf501.top

================================================================================
来源：http://cvb.yongpay.top

D. 数组 / 列表 / 集合
来源：http://sca.xingfuxueyuan.xyz

================================================================================
来源：http://vxd.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://uju.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dzw.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kkt.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ltm.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tlj.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tcr.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://qdf.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://ssp.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aeu.shzxlz.cn

[D02] 追加元素到末尾
来源：http://czw.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tne.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kgl.jianghu66.top

JS:   arr.push(4);
来源：http://wcb.tanke756.top

TS:   arr.push(4);
来源：http://aau.kuanghao11.cn

Java: list.add(4);
来源：http://oys.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://xli.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://nph.shangyingyoupin.top

C#:   list.Add(4);
来源：http://dos.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://dfm.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://jcy.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://epv.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://goh.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://oot.bjfxy.top

Java: list.add(0, 0);
来源：http://nes.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://wmk.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzh.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://bow.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://axk.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vvk.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://udg.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yuz.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://upr.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vou.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://byw.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ukm.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bmv.0kj1m.cn

[D05] 访问与修改元素
来源：http://iiy.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ati.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bcy.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xwp.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://kgv.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://qxi.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://zku.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwc.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nyh.fktsv.cn

[D06] 数组长度
来源：http://kyj.shanyushiyangtech.top

Py:   len(arr)
来源：http://hus.yfazqb.com

PHP:  count($arr);
来源：http://uom.cucudq.cn

JS:   arr.length
来源：http://rtz.jinqigufen.top

TS:   arr.length
来源：http://qal.0kj1m.cn

Java: list.size();
来源：http://its.zhixingplan.top

Go:   len(arr)
来源：http://xfw.daxiang520.top

Ruby: arr.length; arr.size
来源：http://xnv.haohaochexian.top

C#:   list.Count;
来源：http://tnq.guannengcc.top

[D07] 切片 / 取子数组
来源：http://tgh.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://icf.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jww.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://lwl.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://kuf.hfpthk.cn

Java: list.subList(1, 4);
来源：http://mpj.yuxming.cn

Go:   arr[1:4]
来源：http://trs.xuanzx.com

Ruby: arr[1, 3]
来源：http://yrh.hongshengwenyu.top


<!-- 参考信息 -->