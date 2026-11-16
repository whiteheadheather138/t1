代发 wailian999

PHP:  range(0, 10, 2);
来源：http://rfe.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxc.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qta.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yic.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://afn.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://rkt.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oji.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://ppv.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rxt.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://trm.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uzw.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rca.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ftb.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://npd.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eqc.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kev.fengsongda.top

[B13] 判断是否为数字
来源：http://npb.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://czf.hfpthk.cn

PHP:  is_numeric($x)
来源：http://xln.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qpn.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgj.gotoacloud.top

Java: x instanceof Number
来源：http://qbv.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hwf.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://fzy.xinyue.icu

C#:   x is int or double or decimal
来源：http://emi.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://pjs.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xhb.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lrf.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://xyj.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://xgz.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wed.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vwo.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://bdz.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfc.svipenyu.cn

[B15] 布尔运算与取反
来源：http://vss.pycfn.com

Py:   a and b or not c
来源：http://utd.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://evc.pengpengdd.cyou

JS:   a && b || !c
来源：http://vdy.ivvv.top

TS:   a && b || !c
来源：http://jmx.zhengqikj.top

Java: a && b || !c
来源：http://qce.pengpengdd.cyou

Go:   a && b || !c
来源：http://cja.yongpay.top

Ruby: a && b || !c
来源：http://bud.epnwcf.com

C#:   a && b || !c
来源：http://snk.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ntx.zhijiandao.cn

Py:   if not data: return
来源：http://tpj.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://fpo.fehbvm.com

JS:   if (!data) return;
来源：http://etf.hnxiangtu.top

TS:   if (!data) return;
来源：http://oey.andypj.xyz

Java: if (data == null) return;
来源：http://uwd.yuanzhike.top

Go:   if data == nil { return }
来源：http://mxc.yongpay.top

Ruby: return if data.nil?
来源：http://hij.gaohongyu789.top

C#:   if (data == null) return;
来源：http://rwc.xylfe.cn

================================================================================
来源：http://fkt.uphjek.com

C. 函数与作用域
来源：http://dgp.nanxinkj.top

================================================================================
来源：http://job.epnwcf.com

[C01] 定义函数
来源：http://jza.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://imf.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lmb.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://jdp.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://igb.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://txb.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://zpn.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://cok.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cmn.birdmap.top

[C02] 默认参数
来源：http://vcn.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://phv.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tde.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://evt.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jis.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fvm.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsf.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://axs.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://htc.andypj.xyz

[C03] 可变参数
来源：http://arl.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://iih.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gyg.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lhx.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylj.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gpf.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bsc.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://jdt.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgh.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://obd.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rlb.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fvc.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hay.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qsc.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://gqr.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://fkg.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://aqm.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://irb.cqqwz.cn

[C05] 返回多个值
来源：http://iqe.316326.xyz

Py:   return a, b
来源：http://idi.ctjpmb.com

PHP:  return [$a, $b];
来源：http://jty.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ttv.zhiwuduotai.top

TS:   return { a, b };
来源：http://jiw.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wxc.yfazqb.com

Go:   return a, b
来源：http://yyi.tian-w.cn

Ruby: return a, b
来源：http://jqe.sufxvd.cn

C#:   return (a, b);              // ValueTuple
来源：http://yus.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://ubw.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://rmn.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xnk.nanxinkj.top

JS:   const square = x => x * x;
来源：http://uab.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://lid.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://owr.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://yni.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://nmc.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://qvy.c1oappe.top

[C07] 把函数作为参数传入
来源：http://pdt.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ida.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zhw.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xrw.zhongyouzk.top

TS:   arr.map(String)
来源：http://nhi.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pgf.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hvq.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://yit.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mmv.sufxvd.cn

[C08] 闭包
来源：http://irn.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ofa.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tjv.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rtr.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ldf.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://olf.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbg.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jpl.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ipc.zhijiandao.cn

[C09] 递归
来源：http://vzv.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://knz.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tqj.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mzn.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fqe.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kts.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xnr.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ftx.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nqw.quarkkingdee.top

[C10] 变量作用域
来源：http://azo.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uwi.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ojn.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gpq.vehdjk.com

TS:   同 JS
来源：http://tfi.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://htm.yj202588.top

Go:   花括号块级作用域
来源：http://rwz.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qfy.tarul.cn

C#:   块级作用域
来源：http://yvv.vqdsnc.cn

[C11] 模块导入与导出
来源：http://ukz.xylfe.cn

Py:   from module import func
来源：http://dze.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tlk.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qwn.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lti.aibaodan.cn

Java: import java.util.List;
来源：http://zbp.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wpc.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://llc.ctjpmb.com

C#:   using System.Text;
来源：http://dzu.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://rkt.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://zjx.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://zes.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://lxi.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://joy.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kpp.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://uoi.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://fyf.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://byn.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://agm.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yeo.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwv.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ioi.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wpq.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://imu.xinyue.icu

Go:   func add(a, b int) int
来源：http://udg.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gwg.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://pin.yj202588.top

[C14] 泛型函数
来源：http://fmw.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zon.hongshengwenyu.top

PHP:  // 无泛型
来源：http://ghd.tarul.cn

JS:   // 无泛型
来源：http://hyd.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mbo.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kos.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://efa.hysaishi.cn

Ruby: # 无泛型
来源：http://tdt.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hdk.aizwys.cn

[C15] 解构 / 展开参数
来源：http://zjr.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pzy.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://jgo.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hog.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ndq.yangfankeji.com

Java: // 无解构
来源：http://otu.tian-w.cn

Go:   // 无解构
来源：http://fpn.vehdjk.com

Ruby: a, b = pair
来源：http://bdy.316326.xyz

C#:   var (a, b) = pair;
来源：http://hgu.uphjek.com

[C16] 函数 / 方法重载
来源：http://scx.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iuj.hysaishi.cn

PHP:  // 无重载
来源：http://yja.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vji.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ujx.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dka.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://stf.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://zhh.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iro.sxryk.cn

================================================================================
来源：http://qdi.yongpay.top

D. 数组 / 列表 / 集合
来源：http://xki.chenlongwang.top

================================================================================
来源：http://len.jianghu66.top

[D01] 创建数组 / 列表
来源：http://eyf.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://btl.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjq.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yaq.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://dkf.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wot.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://ujn.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://gmn.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kmu.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://bdx.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ogt.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oyh.jyoumei.cn

JS:   arr.push(4);
来源：http://gst.iojbl.cn

TS:   arr.push(4);
来源：http://jqf.vqdsnc.cn

Java: list.add(4);
来源：http://kjy.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://grs.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://tnn.zdqjudy.top

C#:   list.Add(4);
来源：http://oob.sysykeji.top

[D03] 在指定位置插入元素
来源：http://ktq.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://une.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://odk.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wkl.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://bxn.ppjwa.cn

Java: list.add(0, 0);
来源：http://iym.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://bap.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pjh.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://ydg.quarkkingdee.top

[D04] 删除元素
来源：http://riq.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vux.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dcd.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gcq.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://cba.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dyb.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hwf.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fsu.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ors.bjfxy.top

[D05] 访问与修改元素
来源：http://olq.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uea.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bra.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ypy.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://vzi.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dct.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://dlx.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nva.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pgs.svipenyu.cn

[D06] 数组长度
来源：http://hiu.hnqzz.top

Py:   len(arr)
来源：http://gzx.fktsv.cn

PHP:  count($arr);
来源：http://xej.redwolf501.top

JS:   arr.length
来源：http://goh.jinqigufen.top

TS:   arr.length
来源：http://gif.fengsongda.top

Java: list.size();
来源：http://hgy.zhiwuduotai.top

Go:   len(arr)
来源：http://klt.guannengcc.top

Ruby: arr.length; arr.size
来源：http://ven.yj20258.top

C#:   list.Count;
来源：http://qes.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://eho.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hpz.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://tvf.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://zbt.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://veu.gotoacloud.top

Java: list.subList(1, 4);
来源：http://bel.guannengcc.top

Go:   arr[1:4]
来源：http://wmy.haohaochexian.top

Ruby: arr[1, 3]
来源：http://ytq.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://mml.yanxiufei.cn

[D08] 合并两个数组
来源：http://ekb.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://xdw.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://bhc.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pph.sxryk.cn

TS:   [...a, ...b];
来源：http://gbb.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://stb.316326.xyz

Go:   append(a, b...)
来源：http://vue.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://lib.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://xal.jinqigufen.top

[D09] 排序（升序）
来源：http://icm.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://zfp.gotoacloud.top

PHP:  sort($arr);
来源：http://okk.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jhm.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qaw.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oll.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qjg.nanxuanxn.top

Ruby: arr.sort
来源：http://mlu.zhengqikj.top

C#:   list.Sort();
来源：http://icc.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://snw.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gma.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzx.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://geq.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sqx.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oyd.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ezi.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mhi.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xha.hammf.cn

[D11] 反转数组
来源：http://aqj.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ofg.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://lqh.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fap.cashguo.top

TS:   [...arr].reverse();
来源：http://mhf.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://bva.yonumen.top

Go:   slices.Reverse(arr)
来源：http://spz.pycfn.com

Ruby: arr.reverse
来源：http://wth.sxryk.cn


<!-- 参考信息 -->