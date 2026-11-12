代发 wailian999

PHP:  range(0, 10, 2);
来源：http://abo.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ftk.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gqk.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fdm.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tsw.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://lzg.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jqh.hcnkem.com

[B12] 跳出多层循环
来源：http://ugc.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wuh.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://rvh.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://khv.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yxj.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vga.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://edx.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ypu.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ikl.gzhubu.top

[B13] 判断是否为数字
来源：http://rez.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://opc.cucudq.cn

PHP:  is_numeric($x)
来源：http://xuu.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cyu.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rup.cqqwz.cn

Java: x instanceof Number
来源：http://bba.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lzb.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://zox.xuanzx.com

C#:   x is int or double or decimal
来源：http://xfv.tian-w.cn

[B14] 判断值是否在集合内
来源：http://aog.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://osx.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://npl.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://ywt.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://zrx.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gfa.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jpo.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://lbt.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eog.tarul.cn

[B15] 布尔运算与取反
来源：http://ahd.ehwqpu.com

Py:   a and b or not c
来源：http://rfb.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://yhs.daxiang520.top

JS:   a && b || !c
来源：http://mtw.zhengqikj.top

TS:   a && b || !c
来源：http://afz.nanxinkj.top

Java: a && b || !c
来源：http://fpl.jinqigfzy.top

Go:   a && b || !c
来源：http://evy.ppjwa.cn

Ruby: a && b || !c
来源：http://vnl.yvedp.cn

C#:   a && b || !c
来源：http://vjo.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://unv.cashguo.top

Py:   if not data: return
来源：http://esc.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://xyb.gzhubu.top

JS:   if (!data) return;
来源：http://xgc.wangshuangyany.cn

TS:   if (!data) return;
来源：http://jwn.316326.xyz

Java: if (data == null) return;
来源：http://dea.0kj1m.cn

Go:   if data == nil { return }
来源：http://oui.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://wyb.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://xye.chenjidiqi.icu

================================================================================
来源：http://wak.dianchejie.cn

C. 函数与作用域
来源：http://ayl.fzhhl.top

================================================================================
来源：http://jgm.daria6918.cn

[C01] 定义函数
来源：http://khm.meibo888.top

Py:   def add(a, b): return a + b
来源：http://vpk.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qko.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://gcu.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uoj.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qtn.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://xak.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://hon.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://les.yj202588.top

[C02] 默认参数
来源：http://oqi.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://qfq.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cmq.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://nac.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://pdf.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ihg.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uxo.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://lkv.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://imb.sjlbkw.cn

[C03] 可变参数
来源：http://vxf.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://rpc.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mgv.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kvz.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nnv.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ggy.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xrq.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nbr.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efa.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://zqc.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xjc.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rig.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wbo.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xgh.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://gqs.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://gjc.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://pil.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ioa.hnxiangtu.top

[C05] 返回多个值
来源：http://ihi.cashguo.top

Py:   return a, b
来源：http://tqu.sxryk.cn

PHP:  return [$a, $b];
来源：http://sge.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kjx.vehdjk.com

TS:   return { a, b };
来源：http://kjq.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://egb.guowangkeji.top

Go:   return a, b
来源：http://pai.yueranfly.top

Ruby: return a, b
来源：http://rou.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://wju.yonumen.top

[C06] 匿名函数 / lambda
来源：http://rry.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://gag.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://zon.gogol.net.cn

JS:   const square = x => x * x;
来源：http://iru.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://mfa.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldn.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://usq.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://xyf.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ssa.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://clv.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ome.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mnz.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ohr.9152youxi.cn

TS:   arr.map(String)
来源：http://dmi.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gaf.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qbj.sweek.top

Ruby: arr.map(&:upcase)
来源：http://irq.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://njf.tianlin.xyz

[C08] 闭包
来源：http://zbf.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fhx.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lgm.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://krh.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jzx.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gpy.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yzp.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ptp.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hiy.redwolf501.top

[C09] 递归
来源：http://lmq.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://otb.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lbu.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ens.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dum.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nok.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mcj.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://duk.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tps.iojbl.cn

[C10] 变量作用域
来源：http://ndd.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://alk.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://agl.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fyx.tarul.cn

TS:   同 JS
来源：http://dvn.shuidangran.top

Java: 方法内为块级作用域
来源：http://fyp.gaohongyu789.top

Go:   花括号块级作用域
来源：http://aox.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tgw.jinyuanbaomall.cn

C#:   块级作用域
来源：http://jsu.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://alq.jinqigfzy.top

Py:   from module import func
来源：http://vqi.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mbw.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zih.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uwl.shangyingyoupin.top

Java: import java.util.List;
来源：http://ziu.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tkr.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://yct.xuetiantiany.cn

C#:   using System.Text;
来源：http://lle.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://rti.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://fvd.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://vov.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://mas.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://qta.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mgz.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://zcn.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://ujb.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ygc.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://hno.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://knq.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fkv.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hnt.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysm.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vcr.yj202588.top

Go:   func add(a, b int) int
来源：http://dxo.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cxp.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lrv.zhixingplan.top

[C14] 泛型函数
来源：http://itx.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxr.yj20258.top

PHP:  // 无泛型
来源：http://ixu.birdmap.top

JS:   // 无泛型
来源：http://vkt.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hup.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eka.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ijo.316326.xyz

Ruby: # 无泛型
来源：http://axu.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yhd.aizwys.cn

[C15] 解构 / 展开参数
来源：http://yrr.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ncq.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://ztv.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cyl.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xks.316326.xyz

Java: // 无解构
来源：http://lqq.sweek.top

Go:   // 无解构
来源：http://cdo.birdmap.top

Ruby: a, b = pair
来源：http://zwg.daxiang520.top

C#:   var (a, b) = pair;
来源：http://lap.xziqi.cn

[C16] 函数 / 方法重载
来源：http://baf.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pwz.cashguo.top

PHP:  // 无重载
来源：http://fqp.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://cdw.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://ilp.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://otu.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://uhl.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://wmc.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mws.ctjpmb.com

================================================================================
来源：http://pit.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://xuc.jiagoushi.top

================================================================================
来源：http://nji.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://ojp.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://xux.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akv.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mzf.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jak.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ldc.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://jmh.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://hba.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vai.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://bqu.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vno.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://feq.fzhhl.top

JS:   arr.push(4);
来源：http://bsi.cdnleiting.top

TS:   arr.push(4);
来源：http://jtn.yuanzhike.top

Java: list.add(4);
来源：http://bwo.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://wjv.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://qkj.bbcook.cn

C#:   list.Add(4);
来源：http://wzl.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://qey.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://cjj.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mpa.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hlz.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://gnh.hnqzz.top

Java: list.add(0, 0);
来源：http://qtb.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://tez.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbc.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://agl.jqgfzy.top

[D04] 删除元素
来源：http://fkq.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rqt.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ytj.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zun.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://iap.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvh.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rcs.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jpt.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://the.jiagoushi.top

[D05] 访问与修改元素
来源：http://rbc.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gjo.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uyp.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dlr.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://min.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://haf.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://gun.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tbl.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rtx.hesvh.cn

[D06] 数组长度
来源：http://ubd.yj202588.top

Py:   len(arr)
来源：http://qfv.zhengqikj.top

PHP:  count($arr);
来源：http://mmz.daria6918.cn

JS:   arr.length
来源：http://fdg.sysykeji.top

TS:   arr.length
来源：http://pzi.9152youxi.cn

Java: list.size();
来源：http://uxg.redwolf501.top

Go:   len(arr)
来源：http://ofd.xinyue.icu

Ruby: arr.length; arr.size
来源：http://lmo.fengsongda.top

C#:   list.Count;
来源：http://fem.wangdashe.top

[D07] 切片 / 取子数组
来源：http://ewa.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qij.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://ncr.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://jkh.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://hom.ehwqpu.com

Java: list.subList(1, 4);
来源：http://abs.chenzaomai.com

Go:   arr[1:4]
来源：http://dsa.c1oappe.top

Ruby: arr[1, 3]
来源：http://paa.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://tzv.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://ssk.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://nwy.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://nel.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://kwn.zhixingplan.top

TS:   [...a, ...b];
来源：http://haz.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fld.hesvh.cn

Go:   append(a, b...)
来源：http://bsm.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://gxl.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://nhi.sysykeji.top

[D09] 排序（升序）
来源：http://cis.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://ram.cdnleiting.top

PHP:  sort($arr);
来源：http://qbj.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lfq.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gra.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fsg.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jgt.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://wxo.zdbjq.cn

C#:   list.Sort();
来源：http://tbj.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ucm.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mwx.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfb.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eje.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://irl.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://awl.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kuv.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wwx.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xvs.yuxming.cn

[D11] 反转数组
来源：http://ldg.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://rne.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://ide.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://twg.tian-w.cn

TS:   [...arr].reverse();
来源：http://jbq.gzhubu.top

Java: Collections.reverse(list);
来源：http://ocg.yj202588.top

Go:   slices.Reverse(arr)
来源：http://sjy.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://qmb.fehbvm.com


<!-- 参考信息 -->