代发 wailian999

PHP:  range(0, 10, 2);
来源：http://arw.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dun.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fms.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xmv.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vog.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://zhl.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rcm.guowangkeji.top

[B12] 跳出多层循环
来源：http://xcd.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ewh.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzf.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aml.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qce.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jqh.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ogu.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jvl.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://som.gotoacloud.top

[B13] 判断是否为数字
来源：http://jce.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://unn.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://yzf.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcj.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xwp.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://vab.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sgm.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://gwu.gzhubu.top

C#:   x is int or double or decimal
来源：http://xsj.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://gxt.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://drz.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rvz.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://xix.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://afi.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cgk.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgg.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://tvf.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ced.svipenyu.cn

[B15] 布尔运算与取反
来源：http://sij.zhixingplan.top

Py:   a and b or not c
来源：http://ecr.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://rke.gotoacloud.top

JS:   a && b || !c
来源：http://nhf.yj20258.top

TS:   a && b || !c
来源：http://zwu.yonumen.top

Java: a && b || !c
来源：http://hyo.sysykeji.top

Go:   a && b || !c
来源：http://fvw.vqdsnc.cn

Ruby: a && b || !c
来源：http://ycw.ybcxt.top

C#:   a && b || !c
来源：http://vad.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qwe.jinqigfzy.top

Py:   if not data: return
来源：http://woy.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://gap.tianlin.xyz

JS:   if (!data) return;
来源：http://ehx.zhoulong.xyz

TS:   if (!data) return;
来源：http://sfg.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://dnt.jqgufenzy.top

Go:   if data == nil { return }
来源：http://onc.316326.xyz

Ruby: return if data.nil?
来源：http://nll.gzhubu.top

C#:   if (data == null) return;
来源：http://tqt.vqdsnc.cn

================================================================================
来源：http://ozo.sweek.top

C. 函数与作用域
来源：http://ker.kuanghao11.cn

================================================================================
来源：http://mze.316326.xyz

[C01] 定义函数
来源：http://rpm.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://doo.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xin.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://zxf.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://epa.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://efz.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://pvd.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://bkd.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://paq.havefunace.top

[C02] 默认参数
来源：http://khu.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://xgt.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bsu.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://xtk.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ylp.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://adf.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rtv.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://pgj.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://zcb.hcnkem.com

[C03] 可变参数
来源：http://dka.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://qdp.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oyh.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://okf.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jts.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vqu.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mtn.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://saw.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ysa.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://crd.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rdt.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nlm.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://res.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://frs.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://mjb.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://gtx.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://jlv.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://ehx.nwbrower.top

[C05] 返回多个值
来源：http://qso.feifeiyinyue.top

Py:   return a, b
来源：http://grn.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://brn.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://dzo.jiagoushi.top

TS:   return { a, b };
来源：http://rcv.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aug.zhengqikj.top

Go:   return a, b
来源：http://jpb.52xcode.cn

Ruby: return a, b
来源：http://epy.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://dni.cheryme.top

[C06] 匿名函数 / lambda
来源：http://fyy.smart0.xyz

Py:   square = lambda x: x * x
来源：http://rbk.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bsq.chenlongwang.top

JS:   const square = x => x * x;
来源：http://ekk.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://cwt.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qmu.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zsf.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://sgk.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://oil.xziqi.cn

[C07] 把函数作为参数传入
来源：http://hxu.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gaf.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://csl.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogk.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://zhi.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ciu.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ilr.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://rjt.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://ehf.yj20258.top

[C08] 闭包
来源：http://cxq.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gji.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iba.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rhj.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://isj.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nok.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://puu.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mek.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cqo.shanyushiyangkeji.top

[C09] 递归
来源：http://cpd.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tep.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxn.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rga.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mka.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kzg.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://was.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dcs.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wus.cashguo.top

[C10] 变量作用域
来源：http://kkc.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://umx.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nbr.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofe.xylfe.cn

TS:   同 JS
来源：http://rit.meibo888.top

Java: 方法内为块级作用域
来源：http://lpr.vehdjk.com

Go:   花括号块级作用域
来源：http://gnf.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oji.yanxiufei.cn

C#:   块级作用域
来源：http://rzg.kuanghao11.cn

[C11] 模块导入与导出
来源：http://zms.sjlbkw.cn

Py:   from module import func
来源：http://jpk.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rpv.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ekb.snrcjt.cn

Java: import java.util.List;
来源：http://ubf.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rao.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://ekq.snrcjt.cn

C#:   using System.Text;
来源：http://cvn.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://fnr.cheryme.top

Py:   (lambda: print("run"))()
来源：http://hls.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://ovb.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://lls.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://fmt.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rnq.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://ywa.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://roz.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bmq.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://prw.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tqp.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ayk.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kio.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ozc.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://zrr.yangfankeji.com

Go:   func add(a, b int) int
来源：http://pst.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sse.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://uik.cheryme.top

[C14] 泛型函数
来源：http://bhj.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zee.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://nsa.bbcook.cn

JS:   // 无泛型
来源：http://qiy.hysaishi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kif.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ard.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hio.hammf.cn

Ruby: # 无泛型
来源：http://uvd.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tyr.xziqi.cn

[C15] 解构 / 展开参数
来源：http://kpw.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ivx.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://dya.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wgo.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hjo.guannengcc.top

Java: // 无解构
来源：http://rns.sweek.top

Go:   // 无解构
来源：http://chd.xuetiantiany.cn

Ruby: a, b = pair
来源：http://shy.hcnkem.com

C#:   var (a, b) = pair;
来源：http://cvm.c1oappe.top

[C16] 函数 / 方法重载
来源：http://sir.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rlg.mhx1999.top

PHP:  // 无重载
来源：http://zeq.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lsw.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://qrw.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rdv.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://ozw.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://cvy.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zww.jyoumei.cn

================================================================================
来源：http://pji.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://xvd.ctjpmb.com

================================================================================
来源：http://iem.yongpay.top

[D01] 创建数组 / 列表
来源：http://mea.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bga.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qws.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://afp.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qjb.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mfz.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://zkv.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://fyq.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kgq.nwbrower.top

[D02] 追加元素到末尾
来源：http://gyj.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cry.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ybw.birdmap.top

JS:   arr.push(4);
来源：http://kqo.yongpay.top

TS:   arr.push(4);
来源：http://fqj.vqdsnc.cn

Java: list.add(4);
来源：http://kcg.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://gdy.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://pmq.jianghu66.top

C#:   list.Add(4);
来源：http://szf.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://obm.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://hhm.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qxt.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lag.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://zof.iojbl.cn

Java: list.add(0, 0);
来源：http://mdv.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://vyg.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gwg.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://pds.yfazqb.com

[D04] 删除元素
来源：http://cxb.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uwy.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://enm.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hnt.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://vrv.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ypx.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pga.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cmd.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://twa.jqgufenzy.top

[D05] 访问与修改元素
来源：http://jbd.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ynm.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ygm.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ost.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://yqs.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://uib.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://gis.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kcv.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nor.zhiwuduotai.top

[D06] 数组长度
来源：http://sae.daxiang520.top

Py:   len(arr)
来源：http://rlr.hammf.cn

PHP:  count($arr);
来源：http://wie.yj202588.top

JS:   arr.length
来源：http://nmh.hysaishi.cn

TS:   arr.length
来源：http://kqv.hysaishi.cn

Java: list.size();
来源：http://lkb.tianlin.xyz

Go:   len(arr)
来源：http://tjl.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://snj.feifeiyinyue.top

C#:   list.Count;
来源：http://qvr.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://kfm.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyw.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bht.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://qzw.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://ovt.yvedp.cn

Java: list.subList(1, 4);
来源：http://buz.shuidangran.top

Go:   arr[1:4]
来源：http://otn.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://dvg.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://sgb.cdnleiting.top

[D08] 合并两个数组
来源：http://dhq.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://fpq.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://sus.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://xpy.wangdashe.top

TS:   [...a, ...b];
来源：http://cpk.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jze.yonumen.top

Go:   append(a, b...)
来源：http://cpe.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://qgs.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://jyo.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://csr.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://smd.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://mdq.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eyk.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yna.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oel.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kxd.iojbl.cn

Ruby: arr.sort
来源：http://iun.gotoacloud.top

C#:   list.Sort();
来源：http://rur.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lpj.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mtx.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mph.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejz.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzj.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://moo.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cdq.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tik.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hfi.ppjwa.cn

[D11] 反转数组
来源：http://zou.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://kac.yonumen.top

PHP:  array_reverse($arr);
来源：http://ark.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qna.chenlongwang.top

TS:   [...arr].reverse();
来源：http://ezf.bjfxy.top

Java: Collections.reverse(list);
来源：http://jyu.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://rkk.jinqigufen.top

Ruby: arr.reverse
来源：http://pyz.jiagoushi.top


<!-- 参考信息 -->