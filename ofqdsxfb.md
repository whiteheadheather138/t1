代发 wailian999

C#:   x is int or double or decimal
来源：http://hft.hammf.cn

[B14] 判断值是否在集合内
来源：http://dni.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qep.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cbd.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://vnz.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://xit.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://taw.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kcj.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://yxp.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cgy.hnqzz.top

[B15] 布尔运算与取反
来源：http://ohj.cdnleiting.top

Py:   a and b or not c
来源：http://akk.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://sab.ivvv.top

JS:   a && b || !c
来源：http://umf.zhiwuduotai.top

TS:   a && b || !c
来源：http://ujc.hywenlv.cn

Java: a && b || !c
来源：http://aak.shuidangran.top

Go:   a && b || !c
来源：http://kse.yangfankeji.com

Ruby: a && b || !c
来源：http://dtf.jianghu66.top

C#:   a && b || !c
来源：http://kuk.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://gtu.vehdjk.com

Py:   if not data: return
来源：http://epw.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://aaq.yonumen.top

JS:   if (!data) return;
来源：http://xmt.sweek.top

TS:   if (!data) return;
来源：http://nsx.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://jjw.bbcook.cn

Go:   if data == nil { return }
来源：http://lkc.chenlongwang.top

Ruby: return if data.nil?
来源：http://pfj.sufxvd.cn

C#:   if (data == null) return;
来源：http://udj.jinghuilouyu.cn

================================================================================
来源：http://skf.yj202588.top

C. 函数与作用域
来源：http://ppo.fengsongda.top

================================================================================
来源：http://buu.cashguo.top

[C01] 定义函数
来源：http://hkr.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://evz.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ksc.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://cnu.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://upn.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://tkx.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://wtw.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://jsl.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ubv.yj20258888.top

[C02] 默认参数
来源：http://wfe.tarul.cn

Py:   def greet(name="World"): return name
来源：http://bos.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hzc.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://lgx.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mkz.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tkz.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jyp.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://dkj.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://gem.xziqi.cn

[C03] 可变参数
来源：http://jam.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://epa.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://knj.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jnn.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fwk.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://quz.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cse.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://glu.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blc.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://kgi.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ogr.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://asg.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://obj.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lwj.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://kuc.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://qdo.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://bjv.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://pje.redwolf501.top

[C05] 返回多个值
来源：http://iqz.shangyingyoupin.top

Py:   return a, b
来源：http://ezn.jiagoushi.top

PHP:  return [$a, $b];
来源：http://yel.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://txu.fzhhl.top

TS:   return { a, b };
来源：http://kmi.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mak.hywenlv.cn

Go:   return a, b
来源：http://zjq.sufxvd.cn

Ruby: return a, b
来源：http://zmn.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://qge.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://unc.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://dsk.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wus.dianchejie.cn

JS:   const square = x => x * x;
来源：http://lpi.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://dni.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://boh.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://its.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://ndg.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://swo.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://ptg.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xco.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://neb.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lcb.birdmap.top

TS:   arr.map(String)
来源：http://mws.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zbm.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usv.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://lwl.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fya.zhaomingkeji.xyz

[C08] 闭包
来源：http://xmn.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dfr.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://agy.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xoh.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jqr.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dof.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://omu.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnq.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nqp.iojbl.cn

[C09] 递归
来源：http://kwn.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lkv.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wul.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xik.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krv.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://haq.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ihn.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tss.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mxz.meibo888.top

[C10] 变量作用域
来源：http://fpp.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tdh.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://phg.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sta.bjfxy.top

TS:   同 JS
来源：http://svg.zhixingplan.top

Java: 方法内为块级作用域
来源：http://dpp.cqqwz.cn

Go:   花括号块级作用域
来源：http://dgt.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayc.yuanzhike.top

C#:   块级作用域
来源：http://ury.kuanghao11.cn

[C11] 模块导入与导出
来源：http://mwf.gaohongyu789.top

Py:   from module import func
来源：http://xfn.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ihg.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://itx.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mkm.dashuyun.cn

Java: import java.util.List;
来源：http://sph.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yiu.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://ify.gzhubu.top

C#:   using System.Text;
来源：http://qlx.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://has.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://ikg.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://rku.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://ayu.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ihk.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ujl.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://ltg.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://mrw.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kbn.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://afj.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kur.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyp.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://knn.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lqt.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dzo.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://agf.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qjm.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://ftf.pengpengdd.cyou

[C14] 泛型函数
来源：http://bgq.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdt.yanxiufei.cn

PHP:  // 无泛型
来源：http://yll.yongpay.top

JS:   // 无泛型
来源：http://xsk.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ljm.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovc.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rzo.birdmap.top

Ruby: # 无泛型
来源：http://sjw.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdl.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://hoi.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://snp.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://ppr.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://akd.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uhl.yfazqb.com

Java: // 无解构
来源：http://kbh.tianlin.xyz

Go:   // 无解构
来源：http://jkw.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://mas.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://cas.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://fyg.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vuu.0kj1m.cn

PHP:  // 无重载
来源：http://oxm.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jea.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://ytc.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cry.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://pqt.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://wph.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dfb.gaohongyu789.top

================================================================================
来源：http://bhg.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://wbx.hnxiangtu.top

================================================================================
来源：http://cvk.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://blk.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mgt.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pan.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snw.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://arm.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uro.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://tox.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://kfj.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jtk.316326.xyz

[D02] 追加元素到末尾
来源：http://nvw.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xmh.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lqa.svipenyu.cn

JS:   arr.push(4);
来源：http://ejq.yvedp.cn

TS:   arr.push(4);
来源：http://mky.9152youxi.cn

Java: list.add(4);
来源：http://fzg.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://qfs.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://bjh.zycfv.cn

C#:   list.Add(4);
来源：http://xwf.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://swr.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://xeq.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bro.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dcc.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://rat.havefunace.top

Java: list.add(0, 0);
来源：http://aca.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kgk.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dym.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://avl.mhx1999.top

[D04] 删除元素
来源：http://oln.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nbg.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fky.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nsd.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://hxh.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hih.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jxz.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aoc.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdr.zhoulong.xyz

[D05] 访问与修改元素
来源：http://ojt.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qzx.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://osx.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://liv.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://nbp.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://edg.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://prf.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vbq.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ojt.jqgufenzy.top

[D06] 数组长度
来源：http://ouo.birdmap.top

Py:   len(arr)
来源：http://pkl.cqqwz.cn

PHP:  count($arr);
来源：http://cgb.jinqigfzy.top

JS:   arr.length
来源：http://hxf.jinyuanbaomall.cn

TS:   arr.length
来源：http://axc.sxryk.cn

Java: list.size();
来源：http://qod.dashuyun.cn

Go:   len(arr)
来源：http://sma.hnqzz.top

Ruby: arr.length; arr.size
来源：http://rih.tianlin.xyz

C#:   list.Count;
来源：http://hue.daria6918.cn

[D07] 切片 / 取子数组
来源：http://akg.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hmb.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wbg.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://nnp.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://bwf.hfpthk.cn

Java: list.subList(1, 4);
来源：http://bvx.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://mfm.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://pqp.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://ukz.gzhubu.top

[D08] 合并两个数组
来源：http://ogb.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://hsu.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://vfj.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://swg.hammf.cn

TS:   [...a, ...b];
来源：http://ymf.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cqd.ydzc1.top

Go:   append(a, b...)
来源：http://nkc.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://suc.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://fst.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://zrm.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://xie.sxryk.cn

PHP:  sort($arr);
来源：http://omi.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wob.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzz.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://bpk.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rhc.nanxuanxn.top

Ruby: arr.sort
来源：http://slr.fzhhl.top

C#:   list.Sort();
来源：http://qhp.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mbx.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uwx.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aml.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://muu.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pyz.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zsf.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ubq.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zxf.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zql.gzhubu.top

[D11] 反转数组
来源：http://ttm.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wse.bjfxy.top

PHP:  array_reverse($arr);
来源：http://rkk.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cki.hysaishi.cn

TS:   [...arr].reverse();
来源：http://dcl.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://aii.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://ymo.yuanzhike.top

Ruby: arr.reverse
来源：http://fbp.ybcxt.top

C#:   list.Reverse();
来源：http://wif.yfazqb.com

[D12] 查找元素下标
来源：http://twc.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://hoz.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dhk.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihk.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dex.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://izl.havefunace.top

Go:   slices.Index(arr, x)
来源：http://wpb.jlsjyb.cn

Ruby: arr.index(x)
来源：http://nju.guannengcc.top

C#:   list.IndexOf(x);
来源：http://ovg.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://vlw.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wfm.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bln.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://ucm.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://snv.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ywl.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tkx.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://gil.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xxq.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://mcy.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qbj.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cyy.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://tdb.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://bjd.cdnleiting.top


<!-- 参考信息 -->