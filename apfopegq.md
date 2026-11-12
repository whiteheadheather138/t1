代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://mnj.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rpb.hfpthk.cn

[B15] 布尔运算与取反
来源：http://cij.zhiwuduotai.top

Py:   a and b or not c
来源：http://jbu.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://gzf.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://yqn.sufxvd.cn

TS:   a && b || !c
来源：http://jgt.jinyuanbaomall.cn

Java: a && b || !c
来源：http://qhx.meibo888.top

Go:   a && b || !c
来源：http://rvr.tian-w.cn

Ruby: a && b || !c
来源：http://zxc.pycfn.com

C#:   a && b || !c
来源：http://psy.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fol.yuanzhike.top

Py:   if not data: return
来源：http://kou.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://izf.yonumen.top

JS:   if (!data) return;
来源：http://bjo.hfpthk.cn

TS:   if (!data) return;
来源：http://iwz.ctjpmb.com

Java: if (data == null) return;
来源：http://wsg.zhixingplan.top

Go:   if data == nil { return }
来源：http://whz.xuanzx.com

Ruby: return if data.nil?
来源：http://pxs.guowangkeji.top

C#:   if (data == null) return;
来源：http://wox.pengpengdd.cyou

================================================================================
来源：http://hkr.yvedp.cn

C. 函数与作用域
来源：http://vna.smart0.xyz

================================================================================
来源：http://zpu.ydzc1.top

[C01] 定义函数
来源：http://dcy.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://exf.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lln.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://xdh.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nux.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://szl.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://msn.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://zgz.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://inj.havefunace.top

[C02] 默认参数
来源：http://wau.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://fms.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wvz.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://qxl.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qbv.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://swm.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wrq.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://xfx.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://cna.yueranfly.top

[C03] 可变参数
来源：http://zjk.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://lqr.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iak.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://chx.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://esb.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjm.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nvg.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://ubg.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dao.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://wtp.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fcy.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ipt.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hjd.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://njp.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://fdf.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://ets.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://vab.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://jwn.yvedp.cn

[C05] 返回多个值
来源：http://tur.ctjpmb.com

Py:   return a, b
来源：http://lce.xylfe.cn

PHP:  return [$a, $b];
来源：http://iqm.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://cib.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://wsi.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wdq.sweek.top

Go:   return a, b
来源：http://kgu.sysykeji.top

Ruby: return a, b
来源：http://swu.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://cvk.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://bop.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://gaj.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dpq.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://vzx.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://vgb.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rtp.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ffd.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://vuf.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rdh.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://knb.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xtd.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nch.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://flh.yj20258888.top

TS:   arr.map(String)
来源：http://zez.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bys.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kzg.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://vxr.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cfk.xinyue.icu

[C08] 闭包
来源：http://obx.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ztt.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fnf.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pux.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mda.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ihq.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vou.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mzl.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hdi.cqqwz.cn

[C09] 递归
来源：http://vku.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nov.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yae.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npv.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjd.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://etf.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ywh.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://voe.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdr.yangfankeji.com

[C10] 变量作用域
来源：http://oed.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vfn.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gkf.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://msj.epnwcf.com

TS:   同 JS
来源：http://yku.tarul.cn

Java: 方法内为块级作用域
来源：http://gks.ppjwa.cn

Go:   花括号块级作用域
来源：http://guw.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plf.redwolf501.top

C#:   块级作用域
来源：http://wch.guannengcc.top

[C11] 模块导入与导出
来源：http://jtp.jqgufenzy.top

Py:   from module import func
来源：http://kqs.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ehf.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://gqe.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://njs.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://gbr.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hvt.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://bpi.sufxvd.cn

C#:   using System.Text;
来源：http://bjn.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://utz.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://wck.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://iba.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://nmw.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://iju.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ziw.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://ozf.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://vnn.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sbn.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://afn.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ybf.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yed.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ggu.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efp.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://cwl.ybcxt.top

Go:   func add(a, b int) int
来源：http://ysj.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lwu.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rtd.shanyushiyangtech.top

[C14] 泛型函数
来源：http://jxo.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://znd.316326.xyz

PHP:  // 无泛型
来源：http://lik.chenzaomai.com

JS:   // 无泛型
来源：http://kcl.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://css.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ydn.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgf.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://yqg.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncs.smart0.xyz

[C15] 解构 / 展开参数
来源：http://viz.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oed.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://xht.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mgv.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rsj.jqgufenzy.top

Java: // 无解构
来源：http://qzn.hongshengwenyu.top

Go:   // 无解构
来源：http://wtm.xziqi.cn

Ruby: a, b = pair
来源：http://wbu.yj20258888.top

C#:   var (a, b) = pair;
来源：http://qan.andypj.xyz

[C16] 函数 / 方法重载
来源：http://wnm.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zop.xziqi.cn

PHP:  // 无重载
来源：http://zip.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hnv.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://njc.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ere.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://oxh.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://ydu.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ddh.birdmap.top

================================================================================
来源：http://fnb.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://any.zhoulong.xyz

================================================================================
来源：http://rkp.nwbrower.top

[D01] 创建数组 / 列表
来源：http://yrn.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ddd.hongshengwenyu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ypf.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://adn.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kkp.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jmp.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://mpl.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://pad.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fdi.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://ltv.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hzr.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qza.ydzc1.top

JS:   arr.push(4);
来源：http://eud.yuanzhike.top

TS:   arr.push(4);
来源：http://dni.ywan-chungtsiang.top

Java: list.add(4);
来源：http://iet.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://ftz.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://oes.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://how.yueranfly.top

[D03] 在指定位置插入元素
来源：http://qdh.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://xeo.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvm.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vqq.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://zox.yj20258888.top

Java: list.add(0, 0);
来源：http://kzz.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://pyj.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ycr.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://gln.yuxming.cn

[D04] 删除元素
来源：http://bii.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://luh.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cqu.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ktp.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://itq.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dxl.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ept.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aea.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gty.havefunace.top

[D05] 访问与修改元素
来源：http://vja.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kuu.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nsh.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mki.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://bve.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://eqp.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://hhe.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xyx.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rgs.tanke756.top

[D06] 数组长度
来源：http://wby.birdmap.top

Py:   len(arr)
来源：http://ylm.hfpthk.cn

PHP:  count($arr);
来源：http://uql.shzxlz.cn

JS:   arr.length
来源：http://ise.gogol.net.cn

TS:   arr.length
来源：http://gyv.gogol.net.cn

Java: list.size();
来源：http://gbo.ivvv.top

Go:   len(arr)
来源：http://vxl.gzhubu.top

Ruby: arr.length; arr.size
来源：http://fkp.pengpengdd.cyou

C#:   list.Count;
来源：http://raf.fengsongda.top

[D07] 切片 / 取子数组
来源：http://fho.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tyo.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zmp.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://icn.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://epu.cucudq.cn

Java: list.subList(1, 4);
来源：http://yyt.cdnleiting.top

Go:   arr[1:4]
来源：http://rcj.9152youxi.cn

Ruby: arr[1, 3]
来源：http://wjt.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://wpi.sjlbkw.cn

[D08] 合并两个数组
来源：http://wqa.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://zrd.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://son.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://egm.uphjek.com

TS:   [...a, ...b];
来源：http://lhi.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lsx.feifeiyinyue.top

Go:   append(a, b...)
来源：http://rca.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://cpn.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://grl.ybcxt.top

[D09] 排序（升序）
来源：http://vhy.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://dmy.fehbvm.com

PHP:  sort($arr);
来源：http://fpl.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tre.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iey.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zza.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lgk.dashuyun.cn

Ruby: arr.sort
来源：http://oed.yonumen.top

C#:   list.Sort();
来源：http://xlf.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://alm.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wjs.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvd.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dnj.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bud.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fto.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://erd.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://seo.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hme.zhiwuduotai.top

[D11] 反转数组
来源：http://irh.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://utg.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://hdx.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ule.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://zvt.daxiang520.top

Java: Collections.reverse(list);
来源：http://gyn.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://tzc.hywenlv.cn

Ruby: arr.reverse
来源：http://wgg.cucudq.cn

C#:   list.Reverse();
来源：http://rid.feifeiyinyue.top

[D12] 查找元素下标
来源：http://sel.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://rim.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xsn.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcl.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://afs.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rlt.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://mbv.epnwcf.com

Ruby: arr.index(x)
来源：http://kdl.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://hsb.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://nwh.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kas.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cgo.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://lfz.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://fea.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dse.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sfd.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://abr.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://joc.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://hcf.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://njk.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xqr.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://fkr.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://hqd.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://gnl.nanxuanxn.top

Go:   // 手写循环
来源：http://mwx.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cmz.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tiu.shuidangran.top

[D15] 去重
来源：http://mqz.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://stx.bjfxy.top

PHP:  array_unique($arr);
来源：http://tvm.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://sdz.yj202588.top


<!-- 参考信息 -->