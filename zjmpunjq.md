代发 wailian999

C#:   x is int or double or decimal
来源：http://clj.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://mxy.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://atw.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jcz.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://vbv.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://ozt.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://efg.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iru.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://bvh.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rxv.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://snp.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://cfe.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://kjx.vqdsnc.cn

JS:   a && b || !c
来源：http://lkj.ydjk.org.cn

TS:   a && b || !c
来源：http://beg.shanyushiyangkeji.top

Java: a && b || !c
来源：http://zqi.ybcxt.top

Go:   a && b || !c
来源：http://xuw.0kj1m.cn

Ruby: a && b || !c
来源：http://yxq.52xcode.cn

C#:   a && b || !c
来源：http://bbq.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mkh.yvedp.cn

Py:   if not data: return
来源：http://ecf.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://gjm.fktsv.cn

JS:   if (!data) return;
来源：http://nyt.xuanzx.com

TS:   if (!data) return;
来源：http://qni.cheryme.top

Java: if (data == null) return;
来源：http://eye.snrcjt.cn

Go:   if data == nil { return }
来源：http://kff.uphjek.com

Ruby: return if data.nil?
来源：http://dzt.vehdjk.com

C#:   if (data == null) return;
来源：http://rvm.zhaomingkeji.xyz

================================================================================
来源：http://ouf.sufxvd.cn

C. 函数与作用域
来源：http://tuj.xuetiantiany.cn

================================================================================
来源：http://olq.shanyushiyangkeji.top

[C01] 定义函数
来源：http://wqb.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://nlm.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dql.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://nhp.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://los.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wyw.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://opw.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://cpm.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pkr.birdmap.top

[C02] 默认参数
来源：http://rjb.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://ozu.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ihk.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://sbk.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jdv.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jni.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://whi.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://ill.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://lzu.shangyingyoupin.top

[C03] 可变参数
来源：http://hma.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://poh.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wjj.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqc.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://thd.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gfl.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://saw.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wly.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wot.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://msz.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yex.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hkb.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kmx.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nyx.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://cjh.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://pvh.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://mvu.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://uhu.tanke756.top

[C05] 返回多个值
来源：http://vjp.zhixingplan.top

Py:   return a, b
来源：http://ptm.zhixingplan.top

PHP:  return [$a, $b];
来源：http://ahb.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgh.jlsjyb.cn

TS:   return { a, b };
来源：http://znv.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xyf.yj20258.top

Go:   return a, b
来源：http://ana.haohaochexian.top

Ruby: return a, b
来源：http://ifp.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://wxf.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://pxx.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://try.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ovd.guowangkeji.top

JS:   const square = x => x * x;
来源：http://axu.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://fvv.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kmi.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtq.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://arz.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://ggo.aizwys.cn

[C07] 把函数作为参数传入
来源：http://nce.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcc.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yuu.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oun.vehdjk.com

TS:   arr.map(String)
来源：http://ohi.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sdi.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rus.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://coo.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://unr.aibaodan.cn

[C08] 闭包
来源：http://fxp.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kdf.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ivb.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://juv.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qea.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eaf.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yoo.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tkq.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cdd.hnxiangtu.top

[C09] 递归
来源：http://kmm.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hhx.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://edb.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvr.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cbt.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nin.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://adq.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dnv.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rlb.iojbl.cn

[C10] 变量作用域
来源：http://pue.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://agw.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xtd.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://div.birdmap.top

TS:   同 JS
来源：http://vdf.zhengqikj.top

Java: 方法内为块级作用域
来源：http://pqy.jinqigfzy.top

Go:   花括号块级作用域
来源：http://dow.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xgf.xuanzx.com

C#:   块级作用域
来源：http://wup.jiagoushi.top

[C11] 模块导入与导出
来源：http://igk.chenzaomai.com

Py:   from module import func
来源：http://uth.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ebl.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iky.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://svp.yuxming.cn

Java: import java.util.List;
来源：http://rzs.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://adq.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jgp.zdqjudy.top

C#:   using System.Text;
来源：http://gnz.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://lke.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://dmy.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://qml.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://hwo.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://agx.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjo.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://aah.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://lpb.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://djv.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://sfx.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eil.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xls.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tbd.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fbp.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://thz.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://tin.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://get.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://pfs.dashuyun.cn

[C14] 泛型函数
来源：http://khb.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zgh.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://ccy.jinqigfzy.top

JS:   // 无泛型
来源：http://hzk.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xxd.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qqu.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kmc.wangdashe.top

Ruby: # 无泛型
来源：http://uqt.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nxu.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://fzu.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkj.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://cgd.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pxa.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yif.bjfxy.top

Java: // 无解构
来源：http://xxp.jianghu66.top

Go:   // 无解构
来源：http://auv.yvedp.cn

Ruby: a, b = pair
来源：http://yee.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://oba.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://gga.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xfh.hysaishi.cn

PHP:  // 无重载
来源：http://ber.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zkk.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jvq.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://bva.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://vao.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://aep.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pnt.9152youxi.cn

================================================================================
来源：http://yws.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://dsw.zhiwuduotai.top

================================================================================
来源：http://sqn.ivvv.top

[D01] 创建数组 / 列表
来源：http://xdj.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wjl.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kxv.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fee.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xik.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qup.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://esn.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://lfq.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hme.yj20258888.top

[D02] 追加元素到末尾
来源：http://wdd.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gdr.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pgk.bbcook.cn

JS:   arr.push(4);
来源：http://ccx.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://vfq.gaohongyu789.top

Java: list.add(4);
来源：http://jim.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://pff.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://fxt.yfazqb.com

C#:   list.Add(4);
来源：http://qjj.wangdashe.top

[D03] 在指定位置插入元素
来源：http://gjl.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://bzv.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nkj.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rbd.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://ued.nanxuanxn.top

Java: list.add(0, 0);
来源：http://cuc.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://xui.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rlk.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://jbj.snrcjt.cn

[D04] 删除元素
来源：http://yjn.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bgu.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ewx.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wuf.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://krj.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kdk.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lhc.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vhd.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kpf.svipenyu.cn

[D05] 访问与修改元素
来源：http://nwk.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lwe.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cjh.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://itw.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://sns.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://lia.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://bkb.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pmv.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ieu.sxryk.cn

[D06] 数组长度
来源：http://uhb.jyoumei.cn

Py:   len(arr)
来源：http://wds.uphjek.com

PHP:  count($arr);
来源：http://wra.jqgufenzy.top

JS:   arr.length
来源：http://uuj.0kj1m.cn

TS:   arr.length
来源：http://nni.hcnkem.com

Java: list.size();
来源：http://atb.jqgufenzy.top

Go:   len(arr)
来源：http://vtm.xylfe.cn

Ruby: arr.length; arr.size
来源：http://xvf.yanxiufei.cn

C#:   list.Count;
来源：http://iox.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://hwh.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hfo.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://jkk.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://jmz.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://obu.52xcode.cn

Java: list.subList(1, 4);
来源：http://qqe.jinqigufen.top

Go:   arr[1:4]
来源：http://rcu.zdqjudy.top

Ruby: arr[1, 3]
来源：http://def.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://txx.haohaochexian.top

[D08] 合并两个数组
来源：http://uql.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://ipj.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://lzu.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xvx.jqgfzy.top

TS:   [...a, ...b];
来源：http://dbl.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baa.sxryk.cn

Go:   append(a, b...)
来源：http://ika.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://vcc.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://czw.gzhubu.top

[D09] 排序（升序）
来源：http://kyr.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://vjb.nwbrower.top

PHP:  sort($arr);
来源：http://foa.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aox.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yfu.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zyv.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://boy.sufxvd.cn

Ruby: arr.sort
来源：http://gtq.fengsongda.top

C#:   list.Sort();
来源：http://esq.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mqb.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gxg.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ahz.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gko.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://siw.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pqo.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yvo.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tqx.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tcl.havefunace.top

[D11] 反转数组
来源：http://xhu.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pli.tian-w.cn

PHP:  array_reverse($arr);
来源：http://hvj.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zqm.iojbl.cn

TS:   [...arr].reverse();
来源：http://dod.tianlin.xyz

Java: Collections.reverse(list);
来源：http://ojc.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://swz.shzxlz.cn

Ruby: arr.reverse
来源：http://nvj.mhx1999.top

C#:   list.Reverse();
来源：http://npy.zycfv.cn

[D12] 查找元素下标
来源：http://nou.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://wik.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vpb.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://geq.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yoh.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ajl.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://ekf.yangfankeji.com

Ruby: arr.index(x)
来源：http://hrt.smart0.xyz

C#:   list.IndexOf(x);
来源：http://vve.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://bez.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hcb.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gqx.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://egm.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://oew.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lzb.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zkv.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lwx.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://xmc.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://pyr.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ohk.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gaq.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://pmx.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://vph.tianlin.xyz


<!-- 参考信息 -->