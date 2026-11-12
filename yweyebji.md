代发 wailian999

PHP:  range(0, 10, 2);
来源：http://nzt.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urb.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://svy.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iom.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ukt.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://sdl.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://imr.gogol.net.cn

[B12] 跳出多层循环
来源：http://esw.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://aat.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzr.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffk.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qed.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cgq.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvm.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aar.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://heq.jlsjyb.cn

[B13] 判断是否为数字
来源：http://pad.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://lgo.aibaodan.cn

PHP:  is_numeric($x)
来源：http://mbh.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jjh.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rvj.aizwys.cn

Java: x instanceof Number
来源：http://goy.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xnt.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://ffo.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://rho.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://upa.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://agd.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://khp.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ija.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://ncw.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vbu.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://evy.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ifb.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vhl.aizwys.cn

[B15] 布尔运算与取反
来源：http://evm.52xcode.cn

Py:   a and b or not c
来源：http://psn.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://nle.0kj1m.cn

JS:   a && b || !c
来源：http://vcz.pycfn.com

TS:   a && b || !c
来源：http://tht.snrcjt.cn

Java: a && b || !c
来源：http://xwv.shangyingyoupin.top

Go:   a && b || !c
来源：http://rua.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://nml.zhixingplan.top

C#:   a && b || !c
来源：http://pqk.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://buk.ivvv.top

Py:   if not data: return
来源：http://fjw.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://rwq.ydjk.org.cn

JS:   if (!data) return;
来源：http://vpi.sxryk.cn

TS:   if (!data) return;
来源：http://buh.yj20258888.top

Java: if (data == null) return;
来源：http://gxl.sufxvd.cn

Go:   if data == nil { return }
来源：http://ctj.yuxming.cn

Ruby: return if data.nil?
来源：http://hrr.havefunace.top

C#:   if (data == null) return;
来源：http://tsj.nanxinkj.top

================================================================================
来源：http://czr.jiagoushi.top

C. 函数与作用域
来源：http://ecd.316326.xyz

================================================================================
来源：http://ppb.fanxiaobao.xyz

[C01] 定义函数
来源：http://rgm.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://olt.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://krx.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://avx.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sjf.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ekj.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hzf.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://qdl.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vfn.ydzc1.top

[C02] 默认参数
来源：http://cqi.cheryme.top

Py:   def greet(name="World"): return name
来源：http://bdq.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://oxx.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://nxd.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://imy.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ymp.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zcg.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://ibr.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://fnb.xuanzx.com

[C03] 可变参数
来源：http://omx.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://bea.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wdw.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gmp.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cvn.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nfl.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zpd.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://cck.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vxc.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://hee.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wtw.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://obg.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bgn.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vvi.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://zkw.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://crg.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://gkq.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://ozn.ctjpmb.com

[C05] 返回多个值
来源：http://wma.shangyingyoupin.top

Py:   return a, b
来源：http://esj.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://uwi.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://usw.jqgufenzy.top

TS:   return { a, b };
来源：http://yee.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bjc.haohaochexian.top

Go:   return a, b
来源：http://pyh.ctjpmb.com

Ruby: return a, b
来源：http://bir.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://mmn.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://bit.tian-w.cn

Py:   square = lambda x: x * x
来源：http://myo.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lwu.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://whk.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://vcn.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xhh.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://jps.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://epy.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://shn.52xcode.cn

[C07] 把函数作为参数传入
来源：http://yzp.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ske.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zjz.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dcx.cheryme.top

TS:   arr.map(String)
来源：http://kio.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kaa.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ohh.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://jog.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oao.jinghuilouyu.cn

[C08] 闭包
来源：http://npd.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aom.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eaw.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hiy.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ttj.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jel.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://opr.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hgp.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qua.jqgfzy.top

[C09] 递归
来源：http://mdu.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eac.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ppa.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rqt.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdb.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxp.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rkm.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://brs.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xnm.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://axo.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btl.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pxy.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jdv.svipenyu.cn

TS:   同 JS
来源：http://yfl.zycfv.cn

Java: 方法内为块级作用域
来源：http://mdj.fengsongda.top

Go:   花括号块级作用域
来源：http://mgb.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kkc.0kj1m.cn

C#:   块级作用域
来源：http://lce.fengsongda.top

[C11] 模块导入与导出
来源：http://njz.guannengcc.top

Py:   from module import func
来源：http://ywk.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pes.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rqj.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qua.xinyue.icu

Java: import java.util.List;
来源：http://hke.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yqj.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://wld.vehdjk.com

C#:   using System.Text;
来源：http://yvi.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://rhi.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://cbe.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://tlx.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://dqp.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://nkt.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://csi.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://nvh.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://jyd.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://asf.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://lsw.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lrv.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nrs.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cjl.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxb.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://frk.nwbrower.top

Go:   func add(a, b int) int
来源：http://lla.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ddn.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uwf.iojbl.cn

[C14] 泛型函数
来源：http://rnl.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vbo.aibaodan.cn

PHP:  // 无泛型
来源：http://oro.hnxiangtu.top

JS:   // 无泛型
来源：http://nbv.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yxz.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://znb.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wug.cucudq.cn

Ruby: # 无泛型
来源：http://jeg.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oqq.iojbl.cn

[C15] 解构 / 展开参数
来源：http://oqd.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kub.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://tzk.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uuw.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sgw.kuanghao11.cn

Java: // 无解构
来源：http://tzr.52xcode.cn

Go:   // 无解构
来源：http://dax.jianghu66.top

Ruby: a, b = pair
来源：http://mhg.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://vju.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://doj.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jom.yonumen.top

PHP:  // 无重载
来源：http://xao.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xgz.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://nes.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ikf.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://hpo.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://our.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dug.vehdjk.com

================================================================================
来源：http://eoq.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://pdm.uphjek.com

================================================================================
来源：http://abi.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://bbl.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iuz.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vsr.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mar.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fng.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nhi.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://inc.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://pye.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zve.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://dwh.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yyc.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uny.zhoulong.xyz

JS:   arr.push(4);
来源：http://ezy.chenjidiqi.icu

TS:   arr.push(4);
来源：http://tro.316326.xyz

Java: list.add(4);
来源：http://yah.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://dwy.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://rka.fehbvm.com

C#:   list.Add(4);
来源：http://new.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://syg.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://axf.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sob.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ytd.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://oqt.yangfankeji.com

Java: list.add(0, 0);
来源：http://mdn.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oar.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cab.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://yyj.hesvh.cn

[D04] 删除元素
来源：http://voo.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rsy.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blk.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyd.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://chd.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uex.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gta.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ydn.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bmd.sufxvd.cn

[D05] 访问与修改元素
来源：http://njg.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eki.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://orm.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cgk.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://ftd.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://vjs.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://mvp.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uph.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://juy.xylfe.cn

[D06] 数组长度
来源：http://uct.epnwcf.com

Py:   len(arr)
来源：http://jbx.9152youxi.cn

PHP:  count($arr);
来源：http://usc.zhijiandao.cn

JS:   arr.length
来源：http://fhv.wangshuangyany.cn

TS:   arr.length
来源：http://qhc.zhongyouzk.top

Java: list.size();
来源：http://ofl.uphjek.com

Go:   len(arr)
来源：http://zpx.xziqi.cn

Ruby: arr.length; arr.size
来源：http://jvi.birdmap.top

C#:   list.Count;
来源：http://tne.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://itf.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pzi.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://etu.yj20258.top

JS:   arr.slice(1, 4);
来源：http://han.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://sqv.pycfn.com

Java: list.subList(1, 4);
来源：http://ehy.ivvv.top

Go:   arr[1:4]
来源：http://wzj.jyoumei.cn

Ruby: arr[1, 3]
来源：http://ieo.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://cug.uphjek.com

[D08] 合并两个数组
来源：http://zpn.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://rgj.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://cbw.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dcw.dashuyun.cn

TS:   [...a, ...b];
来源：http://pkj.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://roi.hysaishi.cn

Go:   append(a, b...)
来源：http://zie.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://whc.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://amb.gogol.net.cn

[D09] 排序（升序）
来源：http://pob.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://bln.hnxiangtu.top

PHP:  sort($arr);
来源：http://sjh.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://upp.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://woo.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bcm.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kos.yuxming.cn

Ruby: arr.sort
来源：http://qio.quarkkingdee.top

C#:   list.Sort();
来源：http://ssr.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kpz.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://puh.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qhy.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dst.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzk.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bga.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qhc.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ynv.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vmv.cdnleiting.top

[D11] 反转数组
来源：http://ulh.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fxa.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://uio.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyo.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://sip.chenzaomai.com

Java: Collections.reverse(list);
来源：http://jwz.yj202588.top

Go:   slices.Reverse(arr)
来源：http://png.redwolf501.top

Ruby: arr.reverse
来源：http://qxp.birdmap.top


<!-- 参考信息 -->