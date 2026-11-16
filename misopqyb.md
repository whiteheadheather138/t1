代发 wailian999

C#:   x is int or double or decimal
来源：http://lzh.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://wwp.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zey.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vuo.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pfr.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://qpz.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jgx.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mxr.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bpt.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jyx.guowangkeji.top

[B15] 布尔运算与取反
来源：http://vlo.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://yxa.cashguo.top

PHP:  $a && $b || !$c
来源：http://fsf.tian-w.cn

JS:   a && b || !c
来源：http://nsl.pengpengdd.cyou

TS:   a && b || !c
来源：http://swn.feifeiyinyue.top

Java: a && b || !c
来源：http://cmh.hywenlv.cn

Go:   a && b || !c
来源：http://rsf.pengpengdd.cyou

Ruby: a && b || !c
来源：http://los.cucudq.cn

C#:   a && b || !c
来源：http://njj.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wbi.havefunace.top

Py:   if not data: return
来源：http://qdp.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://hql.andypj.xyz

JS:   if (!data) return;
来源：http://mkz.zhongyouzk.top

TS:   if (!data) return;
来源：http://vql.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://tqc.tarul.cn

Go:   if data == nil { return }
来源：http://xmm.yuanzhike.top

Ruby: return if data.nil?
来源：http://jhz.meibo888.top

C#:   if (data == null) return;
来源：http://lsg.jinqigfzy.top

================================================================================
来源：http://mjl.tarul.cn

C. 函数与作用域
来源：http://sje.jinqigfzy.top

================================================================================
来源：http://emf.zhijiandao.cn

[C01] 定义函数
来源：http://jky.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://smf.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rvu.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://ypb.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gsc.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cku.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://rbl.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://owt.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ysv.bbcook.cn

[C02] 默认参数
来源：http://ggn.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://ngf.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://amu.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://ldf.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bwk.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zal.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lef.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://ced.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://vim.jyoumei.cn

[C03] 可变参数
来源：http://gcx.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://gix.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kes.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jbq.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qvb.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://piw.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gvq.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://pqk.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qpr.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://ynz.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rof.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zug.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pex.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iyr.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://ovy.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://fbo.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://uai.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://pnc.yj20258888.top

[C05] 返回多个值
来源：http://tqg.hnxiangtu.top

Py:   return a, b
来源：http://med.gogol.net.cn

PHP:  return [$a, $b];
来源：http://ops.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eol.gogol.net.cn

TS:   return { a, b };
来源：http://jsc.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://orm.xinyue.icu

Go:   return a, b
来源：http://jwr.xuanzx.com

Ruby: return a, b
来源：http://dhr.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://rvv.yonumen.top

[C06] 匿名函数 / lambda
来源：http://qiv.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://ooz.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rbn.c1oappe.top

JS:   const square = x => x * x;
来源：http://ios.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://qap.havefunace.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gmf.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xej.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://vce.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://flb.pycfn.com

[C07] 把函数作为参数传入
来源：http://lwk.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oqh.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://gmq.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bmh.nanxinkj.top

TS:   arr.map(String)
来源：http://sfh.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zap.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lmd.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://pbm.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eim.chenzaomai.com

[C08] 闭包
来源：http://ivk.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ecd.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rep.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://myb.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vru.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhl.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://doo.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yod.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://odp.quarkkingdee.top

[C09] 递归
来源：http://nzl.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wiy.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xpu.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bsg.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxp.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ayj.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iyy.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ntc.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ljh.fengsongda.top

[C10] 变量作用域
来源：http://tuo.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hgt.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://alq.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://skx.jlsjyb.cn

TS:   同 JS
来源：http://zvt.zhixingplan.top

Java: 方法内为块级作用域
来源：http://rxz.fzhhl.top

Go:   花括号块级作用域
来源：http://zbb.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xpi.tarul.cn

C#:   块级作用域
来源：http://xqh.dianchejie.cn

[C11] 模块导入与导出
来源：http://xpe.meibo888.top

Py:   from module import func
来源：http://tez.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hnj.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://esj.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ziv.ydjk.org.cn

Java: import java.util.List;
来源：http://nud.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://awx.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://mkm.yvedp.cn

C#:   using System.Text;
来源：http://pok.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://qlz.yongpay.top

Py:   (lambda: print("run"))()
来源：http://toq.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://sba.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://vmz.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://kzh.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ttr.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://rgm.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://jdq.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://lqo.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://ses.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hsp.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://trq.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jha.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://evb.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lml.fehbvm.com

Go:   func add(a, b int) int
来源：http://oqj.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kdu.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pnr.havefunace.top

[C14] 泛型函数
来源：http://lcc.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wbo.zhiwuduotai.top

PHP:  // 无泛型
来源：http://nqq.havefunace.top

JS:   // 无泛型
来源：http://ucr.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://whk.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ckw.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://skg.yonumen.top

Ruby: # 无泛型
来源：http://ywh.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vsq.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://qxk.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gde.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://ery.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lgg.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mnv.vehdjk.com

Java: // 无解构
来源：http://xwd.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://hgc.guannengcc.top

Ruby: a, b = pair
来源：http://ntk.tarul.cn

C#:   var (a, b) = pair;
来源：http://izc.daxiang520.top

[C16] 函数 / 方法重载
来源：http://pdp.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jjy.yfazqb.com

PHP:  // 无重载
来源：http://wue.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://eub.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://qyv.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rlh.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://lkd.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://lzq.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ezc.yuxming.cn

================================================================================
来源：http://lwc.316326.xyz

D. 数组 / 列表 / 集合
来源：http://fpl.xziqi.cn

================================================================================
来源：http://crh.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://fis.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mcc.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mgq.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mtz.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://rsk.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cms.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://lrp.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://tse.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uek.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://agk.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bmd.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qxa.vehdjk.com

JS:   arr.push(4);
来源：http://lnt.gotoacloud.top

TS:   arr.push(4);
来源：http://dsb.yonumen.top

Java: list.add(4);
来源：http://pra.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://tfn.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://jgj.zhijiandao.cn

C#:   list.Add(4);
来源：http://bke.jianghu66.top

[D03] 在指定位置插入元素
来源：http://jfa.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://zvh.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ibl.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gyg.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://mnr.vqdsnc.cn

Java: list.add(0, 0);
来源：http://zxf.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cvz.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uwe.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://cfw.yj202588.top

[D04] 删除元素
来源：http://yec.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bvk.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lmp.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xaz.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://luv.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hiz.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://msc.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fgf.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ckv.cucudq.cn

[D05] 访问与修改元素
来源：http://kuo.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bck.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://guh.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mmv.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://huz.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://bjh.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://gcw.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rpx.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jlg.yj20258.top

[D06] 数组长度
来源：http://iwi.daria6918.cn

Py:   len(arr)
来源：http://nad.jqgufenzy.top

PHP:  count($arr);
来源：http://gli.zhijiandao.cn

JS:   arr.length
来源：http://ynz.hcnkem.com

TS:   arr.length
来源：http://jol.yonumen.top

Java: list.size();
来源：http://gok.yuxming.cn

Go:   len(arr)
来源：http://rpc.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://qnp.hnxiangtu.top

C#:   list.Count;
来源：http://wrb.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://zmd.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jma.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://paj.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://xsf.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://zut.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://msm.gogol.net.cn

Go:   arr[1:4]
来源：http://wpf.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://ash.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://viw.nanxuanxn.top

[D08] 合并两个数组
来源：http://ydz.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://mjf.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://qtn.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xwu.andypj.xyz

TS:   [...a, ...b];
来源：http://yeo.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iwb.xuanzx.com

Go:   append(a, b...)
来源：http://aha.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://kgc.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://hww.hnxiangtu.top

[D09] 排序（升序）
来源：http://ccv.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ogc.fengsongda.top

PHP:  sort($arr);
来源：http://lwp.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kwf.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lcb.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ijb.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://day.yangfankeji.com

Ruby: arr.sort
来源：http://ler.hammf.cn

C#:   list.Sort();
来源：http://tyu.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ghg.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pxf.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wfo.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uxb.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iql.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://plj.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oxk.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tus.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://snm.ehwqpu.com

[D11] 反转数组
来源：http://xyq.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://tdx.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://igc.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rfm.gogol.net.cn

TS:   [...arr].reverse();
来源：http://gzi.yongpay.top

Java: Collections.reverse(list);
来源：http://hym.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://soj.yj202588.top

Ruby: arr.reverse
来源：http://tab.epnwcf.com

C#:   list.Reverse();
来源：http://rsf.daxiang520.top

[D12] 查找元素下标
来源：http://jkk.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://hby.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ewj.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://asi.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbj.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://avc.havefunace.top

Go:   slices.Index(arr, x)
来源：http://uwy.ctjpmb.com

Ruby: arr.index(x)
来源：http://zks.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://qwn.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://jel.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hub.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fdg.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://nlm.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://wms.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yvz.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbg.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://esp.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://sch.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://zbt.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dij.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pof.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://tfw.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://wni.andypj.xyz


<!-- 参考信息 -->