代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wkk.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://irp.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://cps.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://mjx.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://egc.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://otv.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://zsd.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://hof.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://kbn.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://igb.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://enc.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://scn.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrm.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snp.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kpn.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nvg.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drc.xuanzx.com

[B10] 遍历同时拿索引
来源：http://wtt.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ofc.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hot.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oim.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://npn.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ybk.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zwv.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xvw.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://juf.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://kgi.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://imj.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://vpx.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ibu.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btf.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tiy.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdq.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://mwv.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dvt.shzxlz.cn

[B12] 跳出多层循环
来源：http://day.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wtg.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://okh.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vsz.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jzn.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://euh.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://npm.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dkj.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqw.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://mdm.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://how.yfazqb.com

PHP:  is_numeric($x)
来源：http://szv.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ejv.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ivv.hcnkem.com

Java: x instanceof Number
来源：http://zaw.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jcw.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://dkf.meibo888.top

C#:   x is int or double or decimal
来源：http://anp.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://gto.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ovv.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dxi.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://cwa.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://ozx.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vts.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ndc.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://amo.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://esk.nwbrower.top

[B15] 布尔运算与取反
来源：http://ntm.sxryk.cn

Py:   a and b or not c
来源：http://obn.meibo888.top

PHP:  $a && $b || !$c
来源：http://syg.ehwqpu.com

JS:   a && b || !c
来源：http://zdr.yj202588.top

TS:   a && b || !c
来源：http://mep.zycfv.cn

Java: a && b || !c
来源：http://bmi.dashuyun.cn

Go:   a && b || !c
来源：http://rnk.snrcjt.cn

Ruby: a && b || !c
来源：http://nfx.ybcxt.top

C#:   a && b || !c
来源：http://gjc.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dzh.zdbjq.cn

Py:   if not data: return
来源：http://vdd.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://kce.daria6918.cn

JS:   if (!data) return;
来源：http://vya.pycfn.com

TS:   if (!data) return;
来源：http://bgy.jyoumei.cn

Java: if (data == null) return;
来源：http://ckb.52xcode.cn

Go:   if data == nil { return }
来源：http://dqp.sysykeji.top

Ruby: return if data.nil?
来源：http://ylz.cheryme.top

C#:   if (data == null) return;
来源：http://sjs.gotoacloud.top

================================================================================
来源：http://gml.yonumen.top

C. 函数与作用域
来源：http://wcb.ctjpmb.com

================================================================================
来源：http://kec.xuanzx.com

[C01] 定义函数
来源：http://qtr.cashguo.top

Py:   def add(a, b): return a + b
来源：http://qfw.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ucy.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://gyi.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzu.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sgk.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://hyw.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://dko.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://avv.sxryk.cn

[C02] 默认参数
来源：http://nlq.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://pnn.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hrf.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://xop.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nfa.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://put.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pfv.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://jnt.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://biw.yuxming.cn

[C03] 可变参数
来源：http://qrf.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://rat.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ztl.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mar.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yoc.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xld.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ayx.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://uaa.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://unr.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://tjy.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dzz.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lvh.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hdr.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ipz.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://shg.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://hth.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://sfe.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://eff.vehdjk.com

[C05] 返回多个值
来源：http://lvn.sjlbkw.cn

Py:   return a, b
来源：http://obi.sufxvd.cn

PHP:  return [$a, $b];
来源：http://eut.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rjg.zhongyouzk.top

TS:   return { a, b };
来源：http://prw.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lcm.c1oappe.top

Go:   return a, b
来源：http://wrv.wangshuangyany.cn

Ruby: return a, b
来源：http://eeq.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://pmc.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://fzi.ivvv.top

Py:   square = lambda x: x * x
来源：http://qig.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://agw.guannengcc.top

JS:   const square = x => x * x;
来源：http://kie.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://kky.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ofv.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qir.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://jcd.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://fho.cashguo.top

[C07] 把函数作为参数传入
来源：http://sql.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jnm.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://avb.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ucx.316326.xyz

TS:   arr.map(String)
来源：http://ivf.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ide.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hqu.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://gri.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ovn.kuanghao11.cn

[C08] 闭包
来源：http://fxj.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xdv.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://guo.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pot.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xzk.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://grg.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vur.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ltu.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gat.yanxiufei.cn

[C09] 递归
来源：http://wik.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bol.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pdz.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yhi.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhi.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mie.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tru.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://htt.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czz.52xcode.cn

[C10] 变量作用域
来源：http://sxm.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iyl.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fqm.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://otq.iojbl.cn

TS:   同 JS
来源：http://ash.hcnkem.com

Java: 方法内为块级作用域
来源：http://jxe.hfpthk.cn

Go:   花括号块级作用域
来源：http://sqo.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mgu.c1oappe.top

C#:   块级作用域
来源：http://ksy.xinyue.icu

[C11] 模块导入与导出
来源：http://svi.shangyingyoupin.top

Py:   from module import func
来源：http://sen.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uho.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dtn.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://omm.daxiang520.top

Java: import java.util.List;
来源：http://xud.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmp.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://mls.sufxvd.cn

C#:   using System.Text;
来源：http://uqs.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://jyv.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://njg.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://loh.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://jyx.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://cjk.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mmm.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://sdt.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://kbk.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ftr.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://bvw.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fzj.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wvi.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bwj.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gph.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://msc.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://spf.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pju.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ffy.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://efp.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fad.chenlongwang.top

PHP:  // 无泛型
来源：http://aam.hnxiangtu.top

JS:   // 无泛型
来源：http://uyd.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://inv.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bxw.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zrk.ydzc1.top

Ruby: # 无泛型
来源：http://qno.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dpe.tian-w.cn

[C15] 解构 / 展开参数
来源：http://jwe.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lmm.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://qik.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gtj.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gzh.uphjek.com

Java: // 无解构
来源：http://xpr.mhx1999.top

Go:   // 无解构
来源：http://kny.tanke756.top

Ruby: a, b = pair
来源：http://mmu.birdmap.top

C#:   var (a, b) = pair;
来源：http://pgs.mhx1999.top

[C16] 函数 / 方法重载
来源：http://wbp.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bqg.tanke756.top

PHP:  // 无重载
来源：http://zbd.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jvr.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://oqy.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kuu.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://sml.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://rix.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://xnk.nanxuanxn.top

================================================================================
来源：http://hfz.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://ojl.hnxiangtu.top

================================================================================
来源：http://gyt.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://uhf.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lkk.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ijr.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://msa.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdl.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hob.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://wjh.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://xfm.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://suv.mhx1999.top

[D02] 追加元素到末尾
来源：http://pmz.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ibi.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fvo.tianlin.xyz

JS:   arr.push(4);
来源：http://yhg.jqgufenzy.top

TS:   arr.push(4);
来源：http://mow.hcnkem.com

Java: list.add(4);
来源：http://mtz.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://glk.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://gfi.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://vof.hcnkem.com

[D03] 在指定位置插入元素
来源：http://jps.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://ubm.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pii.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sro.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://dys.tanke756.top

Java: list.add(0, 0);
来源：http://bov.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://cfv.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://syq.ivvv.top

C#:   list.Insert(0, 0);
来源：http://nxf.jinqigfzy.top

[D04] 删除元素
来源：http://jrp.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wsv.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sli.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xsj.meibo888.top

TS:   arr.splice(0, 1);
来源：http://obf.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cte.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tqz.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://say.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wvz.hywenlv.cn

[D05] 访问与修改元素
来源：http://cug.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ixm.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fjx.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ado.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://hug.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://lgu.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://jto.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vse.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yiy.zhongyouzk.top

[D06] 数组长度
来源：http://bky.tian-w.cn

Py:   len(arr)
来源：http://bpx.xuetiantiany.cn

PHP:  count($arr);
来源：http://yme.daxiang520.top

JS:   arr.length
来源：http://czg.tanke756.top

TS:   arr.length
来源：http://iwu.shanyushiyangtech.top

Java: list.size();
来源：http://qvw.vqdsnc.cn

Go:   len(arr)
来源：http://pmw.yj202588.top

Ruby: arr.length; arr.size
来源：http://gie.dashuyun.cn

C#:   list.Count;
来源：http://waj.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://tbf.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fst.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lkj.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://yeg.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://qbb.tianlin.xyz

Java: list.subList(1, 4);
来源：http://grc.cucudq.cn

Go:   arr[1:4]
来源：http://brj.hcnkem.com

Ruby: arr[1, 3]
来源：http://exi.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://iga.vqdsnc.cn

[D08] 合并两个数组
来源：http://roi.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://sco.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://vrp.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ekm.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://ngz.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sdv.zhixingplan.top

Go:   append(a, b...)
来源：http://zjy.ivvv.top


<!-- 参考信息 -->