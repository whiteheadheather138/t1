代发 wailian999

PHP:  $a && $b || !$c
来源：http://uil.fanxiaobao.xyz

JS:   a && b || !c
来源：http://sgq.yangfankeji.com

TS:   a && b || !c
来源：http://mrd.yj202588.top

Java: a && b || !c
来源：http://tdw.meibo888.top

Go:   a && b || !c
来源：http://fef.gzhubu.top

Ruby: a && b || !c
来源：http://avx.tarul.cn

C#:   a && b || !c
来源：http://jyy.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://tqj.jinghuilouyu.cn

Py:   if not data: return
来源：http://cwe.yongpay.top

PHP:  if (!$data) { return; }
来源：http://kgw.meibo888.top

JS:   if (!data) return;
来源：http://zno.sufxvd.cn

TS:   if (!data) return;
来源：http://ylz.ybcxt.top

Java: if (data == null) return;
来源：http://hfy.vqdsnc.cn

Go:   if data == nil { return }
来源：http://lzh.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://urj.zdbjq.cn

C#:   if (data == null) return;
来源：http://fgm.aibaodan.cn

================================================================================
来源：http://qoq.redwolf501.top

C. 函数与作用域
来源：http://xju.yj202588.top

================================================================================
来源：http://dcu.fehbvm.com

[C01] 定义函数
来源：http://txp.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://ypb.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twc.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://qyn.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://czf.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mgm.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kmu.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://eow.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrx.jianghu66.top

[C02] 默认参数
来源：http://aik.yj20258.top

Py:   def greet(name="World"): return name
来源：http://bod.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tnk.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://rwm.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://llm.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://zuq.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rck.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://kfy.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://hsc.chenzaomai.com

[C03] 可变参数
来源：http://wif.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://ijn.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tgd.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yoj.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gop.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qpe.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://avg.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nsh.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jyb.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://ios.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://goj.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gjt.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fjx.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vwf.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://mbk.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://uqe.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://kzg.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://trg.havefunace.top

[C05] 返回多个值
来源：http://cxg.c1oappe.top

Py:   return a, b
来源：http://vve.hnqzz.top

PHP:  return [$a, $b];
来源：http://jvx.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hsg.cqqwz.cn

TS:   return { a, b };
来源：http://qsu.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fkq.shuidangran.top

Go:   return a, b
来源：http://zen.smart0.xyz

Ruby: return a, b
来源：http://nmq.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://nta.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://nni.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://zbo.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rwu.c1oappe.top

JS:   const square = x => x * x;
来源：http://kzr.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://gqh.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gtt.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qyj.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://ugv.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://pgl.xylfe.cn

[C07] 把函数作为参数传入
来源：http://egc.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcs.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://luz.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tkx.cheryme.top

TS:   arr.map(String)
来源：http://hzh.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://grs.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xnq.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://any.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://izj.yueranfly.top

[C08] 闭包
来源：http://prj.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qme.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fso.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xhw.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cyu.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eag.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cdi.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://khs.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://min.sufxvd.cn

[C09] 递归
来源：http://giy.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dup.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://prn.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://imd.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ras.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kxc.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gqd.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iwo.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ufa.sufxvd.cn

[C10] 变量作用域
来源：http://jad.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ekd.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryc.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qgb.jinyuanbaomall.cn

TS:   同 JS
来源：http://smn.hywenlv.cn

Java: 方法内为块级作用域
来源：http://euq.aizwys.cn

Go:   花括号块级作用域
来源：http://aaa.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rik.jianghu66.top

C#:   块级作用域
来源：http://wap.fehbvm.com

[C11] 模块导入与导出
来源：http://scl.zhiwuduotai.top

Py:   from module import func
来源：http://hvr.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sdv.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dmf.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kui.daxiang520.top

Java: import java.util.List;
来源：http://cpr.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fav.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://zdp.316326.xyz

C#:   using System.Text;
来源：http://pan.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://ele.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://sml.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://ngm.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://mcb.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://tic.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxm.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://vxb.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://qzj.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cws.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://vtk.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dbj.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://orj.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bqk.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hho.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ugk.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://plg.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nxs.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://bco.hesvh.cn

[C14] 泛型函数
来源：http://uon.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mmh.smart0.xyz

PHP:  // 无泛型
来源：http://qih.redwolf501.top

JS:   // 无泛型
来源：http://ayh.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pbf.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ldj.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xpo.yongpay.top

Ruby: # 无泛型
来源：http://qcg.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://div.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://ayh.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cnh.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://dzu.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ulh.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bry.aibaodan.cn

Java: // 无解构
来源：http://yju.ehwqpu.com

Go:   // 无解构
来源：http://rye.gogol.net.cn

Ruby: a, b = pair
来源：http://ylb.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://wxx.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://jir.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wrz.yueranfly.top

PHP:  // 无重载
来源：http://wku.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjl.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://qao.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vcy.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://ojq.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://zar.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lhk.fktsv.cn

================================================================================
来源：http://sgw.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://wgs.smart0.xyz

================================================================================
来源：http://kkd.yj20258.top

[D01] 创建数组 / 列表
来源：http://uov.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gvf.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ern.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qhr.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eon.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://trh.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://ovd.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://qwp.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zps.yj20258888.top

[D02] 追加元素到末尾
来源：http://fss.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://isd.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cil.hnxiangtu.top

JS:   arr.push(4);
来源：http://tio.birdmap.top

TS:   arr.push(4);
来源：http://qbs.sxryk.cn

Java: list.add(4);
来源：http://hsc.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://llf.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://zwv.hongshengwenyu.top

C#:   list.Add(4);
来源：http://qsv.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://qeg.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://lzd.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hsd.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ikp.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://fum.bbcook.cn

Java: list.add(0, 0);
来源：http://vrs.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pmj.gaohongyu789.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zkm.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://ltb.hongshengwenyu.top

[D04] 删除元素
来源：http://wer.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyn.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zhz.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bzr.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://dko.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fok.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eds.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nrj.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bhl.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://mra.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nqo.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fzm.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://arq.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://plq.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://qpl.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://jpk.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qgu.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ewj.jiagoushi.top

[D06] 数组长度
来源：http://sly.zhixingplan.top

Py:   len(arr)
来源：http://nlb.yuxming.cn

PHP:  count($arr);
来源：http://fzr.ivvv.top

JS:   arr.length
来源：http://qpm.ywan-chungtsiang.top

TS:   arr.length
来源：http://dnw.hnqzz.top

Java: list.size();
来源：http://tah.bbcook.cn

Go:   len(arr)
来源：http://unp.xuanzx.com

Ruby: arr.length; arr.size
来源：http://wdj.jinqigfzy.top

C#:   list.Count;
来源：http://smp.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://oke.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aew.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://olh.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://anq.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://cbq.dianchejie.cn

Java: list.subList(1, 4);
来源：http://fqz.sweek.top

Go:   arr[1:4]
来源：http://tqq.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://vvs.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://lwf.meibo888.top

[D08] 合并两个数组
来源：http://hbt.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://ysw.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://vrr.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://izn.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://tjd.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://btp.epnwcf.com

Go:   append(a, b...)
来源：http://ocv.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://mks.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://rbv.aizwys.cn

[D09] 排序（升序）
来源：http://jjm.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://tsd.ybcxt.top

PHP:  sort($arr);
来源：http://mcs.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yoz.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nep.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbe.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://thw.ivvv.top

Ruby: arr.sort
来源：http://bkm.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://njo.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://cms.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://myj.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yeo.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wkz.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vkc.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wiu.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ugs.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hns.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vus.iojbl.cn

[D11] 反转数组
来源：http://ytp.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://sgl.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://fjg.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lev.xuanzx.com

TS:   [...arr].reverse();
来源：http://jis.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://vus.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://vot.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://ype.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://epg.sweek.top

[D12] 查找元素下标
来源：http://vrv.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://qoz.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tja.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gms.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fus.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wnu.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://mvw.gotoacloud.top

Ruby: arr.index(x)
来源：http://hun.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://qui.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://med.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://poi.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tve.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://wpo.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://ztt.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fvi.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yau.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://mdj.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tau.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://tnl.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://umj.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cdx.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://qfi.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://dgt.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://euh.guannengcc.top

Go:   // 手写循环
来源：http://het.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wku.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lyt.aizwys.cn

[D15] 去重
来源：http://boa.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://giz.yj202588.top

PHP:  array_unique($arr);
来源：http://xtz.andypj.xyz

JS:   [...new Set(arr)]
来源：http://bft.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://rob.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lum.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://jpp.zycfv.cn

Ruby: arr.uniq
来源：http://azs.nwbrower.top


<!-- 参考信息 -->