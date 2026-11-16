代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://obw.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://bel.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://qil.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://ush.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://kzk.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://fpp.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://ced.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://btc.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://uwv.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ten.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://qqo.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://fio.aibaodan.cn

[B09] break 与 continue
来源：http://njy.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qkr.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kqs.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpz.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfq.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bev.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pyp.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ufr.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffq.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://izv.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iap.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wqp.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://avg.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zoo.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kxw.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gqf.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmb.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bru.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://qnv.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://neu.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://nil.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://isl.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dvg.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://phh.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tph.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://kgb.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tfm.hcnkem.com

[B12] 跳出多层循环
来源：http://rsr.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ulp.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ahb.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jly.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxk.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zre.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aet.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fjj.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oqe.jqgufenzy.top

[B13] 判断是否为数字
来源：http://agx.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://lfu.zycfv.cn

PHP:  is_numeric($x)
来源：http://obu.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcx.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jvo.zhijiandao.cn

Java: x instanceof Number
来源：http://ymu.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://olc.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://pvw.fengsongda.top

C#:   x is int or double or decimal
来源：http://abh.yfazqb.com

[B14] 判断值是否在集合内
来源：http://aon.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ave.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cal.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gbk.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://dup.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qqr.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wcp.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://mxc.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ruz.jianghu66.top

[B15] 布尔运算与取反
来源：http://frn.guowangkeji.top

Py:   a and b or not c
来源：http://irx.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://tsh.ydzc1.top

JS:   a && b || !c
来源：http://cvq.zdbjq.cn

TS:   a && b || !c
来源：http://oda.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://nmy.guannengcc.top

Go:   a && b || !c
来源：http://ivv.guowangkeji.top

Ruby: a && b || !c
来源：http://ntq.birdmap.top

C#:   a && b || !c
来源：http://hwt.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://rcu.aibaodan.cn

Py:   if not data: return
来源：http://ztk.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://mjy.yuxming.cn

JS:   if (!data) return;
来源：http://tqx.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://xol.zhijiandao.cn

Java: if (data == null) return;
来源：http://mst.bbcook.cn

Go:   if data == nil { return }
来源：http://ljy.ybcxt.top

Ruby: return if data.nil?
来源：http://esz.yueranfly.top

C#:   if (data == null) return;
来源：http://bok.zhengqikj.top

================================================================================
来源：http://wwe.havefunace.top

C. 函数与作用域
来源：http://eib.tarul.cn

================================================================================
来源：http://vdw.jinqigfzy.top

[C01] 定义函数
来源：http://iqd.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://ium.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lay.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ruw.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsl.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hfc.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ofo.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://hdk.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qtn.zhijiandao.cn

[C02] 默认参数
来源：http://ccp.ivvv.top

Py:   def greet(name="World"): return name
来源：http://bxk.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vkl.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://zab.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://mnk.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nna.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yjn.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://oow.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gnh.bbcook.cn

[C03] 可变参数
来源：http://kbd.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://wuh.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nxb.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpz.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxw.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uho.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nay.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://yoh.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ecf.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://zna.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zbn.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmx.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://njp.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://djx.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://ple.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://rvv.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://lsb.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://apa.jlsjyb.cn

[C05] 返回多个值
来源：http://fsd.wangshuangyany.cn

Py:   return a, b
来源：http://lbc.zhixingplan.top

PHP:  return [$a, $b];
来源：http://avt.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://twp.yonumen.top

TS:   return { a, b };
来源：http://hos.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://teu.fzhhl.top

Go:   return a, b
来源：http://gdg.tanke756.top

Ruby: return a, b
来源：http://qbe.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://nrn.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://rjg.fzhhl.top

Py:   square = lambda x: x * x
来源：http://fet.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zmg.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://vfi.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://xzq.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wwx.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://kkh.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://ffl.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://goa.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://lyi.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dvi.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oqo.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syg.zhijiandao.cn

TS:   arr.map(String)
来源：http://jfa.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bcg.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ams.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://ova.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qyi.c1oappe.top

[C08] 闭包
来源：http://fwx.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eko.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bwh.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qdo.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bmv.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mgm.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tus.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dkt.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kss.gogol.net.cn

[C09] 递归
来源：http://qdo.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hvz.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bwy.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pha.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nbq.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cat.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://abe.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iqq.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wue.jinghuilouyu.cn

[C10] 变量作用域
来源：http://ifv.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://acd.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfu.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rua.gzhubu.top

TS:   同 JS
来源：http://nhz.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://wqa.chenlongwang.top

Go:   花括号块级作用域
来源：http://ylk.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://clf.pengpengdd.cyou

C#:   块级作用域
来源：http://llm.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://dqx.dashuyun.cn

Py:   from module import func
来源：http://pgw.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lky.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eom.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oeu.fzhhl.top

Java: import java.util.List;
来源：http://yim.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hpv.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://vsr.yj202588.top

C#:   using System.Text;
来源：http://twe.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://lkb.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://kdz.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://kjr.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://fco.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://qds.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wpt.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://ypf.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://ims.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ldm.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://fow.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jtg.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://obg.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hud.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sfm.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vmz.bbcook.cn

Go:   func add(a, b int) int
来源：http://dgf.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://agg.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://ils.fanxiaobao.xyz

[C14] 泛型函数
来源：http://soh.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bqs.tarul.cn

PHP:  // 无泛型
来源：http://hvx.hysaishi.cn

JS:   // 无泛型
来源：http://ygs.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bfk.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vss.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ofb.yj20258888.top

Ruby: # 无泛型
来源：http://cpt.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ddc.shuidangran.top

[C15] 解构 / 展开参数
来源：http://ktu.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bde.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://wjy.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://omj.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zqd.xuanzx.com

Java: // 无解构
来源：http://sph.fktsv.cn

Go:   // 无解构
来源：http://bvl.zycfv.cn

Ruby: a, b = pair
来源：http://bvl.xinyue.icu

C#:   var (a, b) = pair;
来源：http://vzq.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://paz.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qse.gaohongyu789.top

PHP:  // 无重载
来源：http://xwh.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dem.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://vix.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zcn.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://rms.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://cqd.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mth.yanxiufei.cn

================================================================================
来源：http://dhu.316326.xyz

D. 数组 / 列表 / 集合
来源：http://lyn.aizwys.cn

================================================================================
来源：http://toh.wangdashe.top

[D01] 创建数组 / 列表
来源：http://emw.fanxiaobao.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://fqp.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yhh.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://int.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fdi.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ogh.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://lhk.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://fpn.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qhp.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://sfw.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oot.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ywh.jqgufenzy.top

JS:   arr.push(4);
来源：http://qaf.tarul.cn

TS:   arr.push(4);
来源：http://vgl.xylfe.cn

Java: list.add(4);
来源：http://tvw.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://qlw.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://zpe.pengpengdd.cyou

C#:   list.Add(4);
来源：http://vjg.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://smr.uphjek.com

Py:   arr.insert(0, 0)
来源：http://yry.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cyj.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tsb.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://xct.tian-w.cn

Java: list.add(0, 0);
来源：http://qul.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://urp.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cov.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://hmc.wangshuangyany.cn

[D04] 删除元素
来源：http://aci.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wey.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://isy.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jlv.yj20258.top

TS:   arr.splice(0, 1);
来源：http://tvd.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fov.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wzx.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yif.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mvz.hywenlv.cn

[D05] 访问与修改元素
来源：http://azj.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://roo.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yot.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kka.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://ddv.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://iwu.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://bwf.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jev.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dxa.dashuyun.cn

[D06] 数组长度
来源：http://tib.guannengcc.top

Py:   len(arr)
来源：http://olh.aizwys.cn

PHP:  count($arr);
来源：http://jmq.nanxuanxn.top

JS:   arr.length
来源：http://xkl.daria6918.cn

TS:   arr.length
来源：http://yni.ydzc1.top

Java: list.size();
来源：http://xfa.uphjek.com

Go:   len(arr)
来源：http://tot.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://whj.xuetiantiany.cn

C#:   list.Count;
来源：http://dtw.yj202588.top

[D07] 切片 / 取子数组
来源：http://zxx.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xzs.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://pmp.yj20258.top

JS:   arr.slice(1, 4);
来源：http://khq.pycfn.com

TS:   arr.slice(1, 4);
来源：http://nzo.sweek.top

Java: list.subList(1, 4);
来源：http://kmy.havefunace.top

Go:   arr[1:4]
来源：http://idt.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://via.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://sjr.gotoacloud.top

[D08] 合并两个数组
来源：http://ouu.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://kvf.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://obh.daria6918.cn


<!-- 参考信息 -->