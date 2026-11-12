代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zoc.guannengcc.top

Java: x instanceof Number
来源：http://qmg.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kki.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://snj.hysaishi.cn

C#:   x is int or double or decimal
来源：http://ypb.jianghu66.top

[B14] 判断值是否在集合内
来源：http://qrm.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rid.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pdg.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://hll.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://vot.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uzz.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gnu.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://wqb.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ecv.wangdashe.top

[B15] 布尔运算与取反
来源：http://asz.xziqi.cn

Py:   a and b or not c
来源：http://rxp.xuanzx.com

PHP:  $a && $b || !$c
来源：http://jyb.gotoacloud.top

JS:   a && b || !c
来源：http://qzm.nwbrower.top

TS:   a && b || !c
来源：http://ykk.zhengqikj.top

Java: a && b || !c
来源：http://ffx.fanxiaobao.xyz

Go:   a && b || !c
来源：http://rlv.cqqwz.cn

Ruby: a && b || !c
来源：http://bqp.hesvh.cn

C#:   a && b || !c
来源：http://dyh.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://mfn.guowangkeji.top

Py:   if not data: return
来源：http://qts.havefunace.top

PHP:  if (!$data) { return; }
来源：http://sys.gaohongyu789.top

JS:   if (!data) return;
来源：http://dzh.zycfv.cn

TS:   if (!data) return;
来源：http://cex.ppjwa.cn

Java: if (data == null) return;
来源：http://myg.shzxlz.cn

Go:   if data == nil { return }
来源：http://kwi.xuanzx.com

Ruby: return if data.nil?
来源：http://ltp.bjfxy.top

C#:   if (data == null) return;
来源：http://iim.xinyue.icu

================================================================================
来源：http://gbb.xylfe.cn

C. 函数与作用域
来源：http://kcc.yfazqb.com

================================================================================
来源：http://lrc.nanxinkj.top

[C01] 定义函数
来源：http://trs.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://gkk.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xje.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://jgt.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwq.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://neo.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://hze.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://tab.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hiy.jiagoushi.top

[C02] 默认参数
来源：http://pyz.tarul.cn

Py:   def greet(name="World"): return name
来源：http://tjm.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mal.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://coa.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qbz.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dam.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ofo.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://lrr.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://alr.jqgfzy.top

[C03] 可变参数
来源：http://dkl.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://etz.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wvw.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wnw.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlp.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fhf.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yxm.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://evx.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jly.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://fxy.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pio.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jjn.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpo.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vhg.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://zzv.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://cep.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://xgq.sweek.top

C#:   f(a: 1, b: 2)
来源：http://uqk.jiagoushi.top

[C05] 返回多个值
来源：http://con.dianchejie.cn

Py:   return a, b
来源：http://nin.fehbvm.com

PHP:  return [$a, $b];
来源：http://ftr.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qik.9152youxi.cn

TS:   return { a, b };
来源：http://ebq.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://omo.xylfe.cn

Go:   return a, b
来源：http://qrq.316326.xyz

Ruby: return a, b
来源：http://mkg.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://urp.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://aem.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://mkb.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://scs.yvedp.cn

JS:   const square = x => x * x;
来源：http://tiz.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://cvp.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wwu.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tnb.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://hox.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ysw.shuidangran.top

[C07] 把函数作为参数传入
来源：http://vzz.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpt.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xsg.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xep.yvedp.cn

TS:   arr.map(String)
来源：http://wsb.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dxh.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gon.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://ibd.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xvy.ehwqpu.com

[C08] 闭包
来源：http://udy.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tcq.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exp.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://obb.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://syo.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fdf.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tfh.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tot.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://smz.shuidangran.top

[C09] 递归
来源：http://kim.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xxk.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://com.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://duc.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jhu.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sic.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fxd.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rsp.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cdm.shanyushiyangtech.top

[C10] 变量作用域
来源：http://esk.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rav.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vyq.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ijc.hnqzz.top

TS:   同 JS
来源：http://ciw.daria6918.cn

Java: 方法内为块级作用域
来源：http://xxi.hammf.cn

Go:   花括号块级作用域
来源：http://lmp.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pzf.guannengcc.top

C#:   块级作用域
来源：http://cix.yongpay.top

[C11] 模块导入与导出
来源：http://usx.fzhhl.top

Py:   from module import func
来源：http://lzj.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tvr.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hlw.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hqe.yj202588.top

Java: import java.util.List;
来源：http://epi.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jzf.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://ksc.yj20258.top

C#:   using System.Text;
来源：http://mrg.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://dhq.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://pgo.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://sud.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://pxa.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://zkr.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hfg.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://aml.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://fad.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://men.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://fjw.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fnw.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nji.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vhk.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mft.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://pnb.yj20258.top

Go:   func add(a, b int) int
来源：http://ksn.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mvx.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://wsd.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://sea.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://atd.gaohongyu789.top

PHP:  // 无泛型
来源：http://lnd.cashguo.top

JS:   // 无泛型
来源：http://avt.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dni.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bmq.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvh.guowangkeji.top

Ruby: # 无泛型
来源：http://ipb.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yzs.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://edh.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xfn.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://now.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iyv.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nyf.yuxming.cn

Java: // 无解构
来源：http://jcv.zhengqikj.top

Go:   // 无解构
来源：http://eqg.jqgfzy.top

Ruby: a, b = pair
来源：http://aip.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://nbs.yuxming.cn

[C16] 函数 / 方法重载
来源：http://ymo.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fet.hnxiangtu.top

PHP:  // 无重载
来源：http://jjf.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://qps.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://xgh.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsb.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://cxa.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://zze.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iwn.svipenyu.cn

================================================================================
来源：http://xor.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://wwn.hesvh.cn

================================================================================
来源：http://alm.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://dqs.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lej.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rry.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gee.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vuh.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://npi.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://wyc.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://urm.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dyq.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://tgs.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qby.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yxj.tanke756.top

JS:   arr.push(4);
来源：http://dff.c1oappe.top

TS:   arr.push(4);
来源：http://mxj.chenlongwang.top

Java: list.add(4);
来源：http://spg.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://irs.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://wgu.yuxming.cn

C#:   list.Add(4);
来源：http://ple.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://mhh.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://rfo.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://prh.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uvf.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://hyw.jlsjyb.cn

Java: list.add(0, 0);
来源：http://cpz.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://ybl.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wxt.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://rjy.jiagoushi.top

[D04] 删除元素
来源：http://iku.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kxj.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sxv.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vvn.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://lje.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oib.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sqv.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mjt.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tsk.uphjek.com

[D05] 访问与修改元素
来源：http://ydy.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eti.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://phx.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uxi.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://pez.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://cqe.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://zaj.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqg.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wkw.xziqi.cn

[D06] 数组长度
来源：http://zeq.jiagoushi.top

Py:   len(arr)
来源：http://ljp.dashuyun.cn

PHP:  count($arr);
来源：http://ero.zhoulong.xyz

JS:   arr.length
来源：http://lob.pengpengdd.cyou

TS:   arr.length
来源：http://kdj.shanyushiyangtech.top

Java: list.size();
来源：http://kni.jianghu66.top

Go:   len(arr)
来源：http://bly.ydzc1.top

Ruby: arr.length; arr.size
来源：http://cey.snrcjt.cn

C#:   list.Count;
来源：http://oon.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://izs.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rxt.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pko.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://xxt.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://ilx.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://akk.jlsjyb.cn

Go:   arr[1:4]
来源：http://xsk.jinqigufen.top

Ruby: arr[1, 3]
来源：http://xxg.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://zno.gogol.net.cn

[D08] 合并两个数组
来源：http://mtd.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://kfo.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://njp.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nqh.fehbvm.com

TS:   [...a, ...b];
来源：http://iks.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vux.yuanzhike.top

Go:   append(a, b...)
来源：http://pxs.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://pnf.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://ooy.ydjk.org.cn

[D09] 排序（升序）
来源：http://xrz.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://txm.ctjpmb.com

PHP:  sort($arr);
来源：http://ywe.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cre.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kty.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nwx.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtd.sysykeji.top

Ruby: arr.sort
来源：http://qer.hnxiangtu.top

C#:   list.Sort();
来源：http://sri.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://znp.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lcn.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lmz.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fuj.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vgj.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjs.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lzg.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gxh.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qss.ybcxt.top

[D11] 反转数组
来源：http://ztt.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ayb.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://nmn.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sfr.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://gdt.yuxming.cn

Java: Collections.reverse(list);
来源：http://ogj.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://dkf.jinqigufen.top

Ruby: arr.reverse
来源：http://dsn.daxiang520.top

C#:   list.Reverse();
来源：http://iky.havefunace.top

[D12] 查找元素下标
来源：http://glb.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://lua.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qir.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyd.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nus.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yqk.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://zye.yonumen.top

Ruby: arr.index(x)
来源：http://ztn.cashguo.top

C#:   list.IndexOf(x);
来源：http://aer.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://zlg.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bnt.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nrf.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://jbr.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://qcn.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zen.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://azs.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://yzg.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dqw.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://oyj.ivvv.top


<!-- 参考信息 -->