代发 wailian999

C#:   x is int or double or decimal
来源：http://tgh.aizwys.cn

[B14] 判断值是否在集合内
来源：http://eas.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ots.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zzt.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://lfb.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ert.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ugt.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mtg.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://ipl.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lmb.sxryk.cn

[B15] 布尔运算与取反
来源：http://qrd.yj20258.top

Py:   a and b or not c
来源：http://swb.ybcxt.top

PHP:  $a && $b || !$c
来源：http://iby.mhx1999.top

JS:   a && b || !c
来源：http://hem.jianghu66.top

TS:   a && b || !c
来源：http://vth.jinqigfzy.top

Java: a && b || !c
来源：http://stg.fehbvm.com

Go:   a && b || !c
来源：http://nfb.wangshuangyany.cn

Ruby: a && b || !c
来源：http://qyf.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://pta.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rgp.wangdashe.top

Py:   if not data: return
来源：http://fna.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://wav.uphjek.com

JS:   if (!data) return;
来源：http://jfc.ehwqpu.com

TS:   if (!data) return;
来源：http://onk.fehbvm.com

Java: if (data == null) return;
来源：http://jfs.bbcook.cn

Go:   if data == nil { return }
来源：http://duo.ydjk.org.cn

Ruby: return if data.nil?
来源：http://cjx.ehwqpu.com

C#:   if (data == null) return;
来源：http://xml.zhijiandao.cn

================================================================================
来源：http://wai.yueranfly.top

C. 函数与作用域
来源：http://jcu.daxiang520.top

================================================================================
来源：http://zvm.hcnkem.com

[C01] 定义函数
来源：http://std.tarul.cn

Py:   def add(a, b): return a + b
来源：http://ico.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qfc.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://cbo.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exa.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://erc.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://hho.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://gdg.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uzm.bbcook.cn

[C02] 默认参数
来源：http://oxd.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://uqq.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jdc.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://jxr.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://dkq.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xds.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xaa.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://tqp.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://lej.vehdjk.com

[C03] 可变参数
来源：http://gfi.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://dcr.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ush.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hog.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dso.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bld.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hzx.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://sgf.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rzr.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://gbm.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kcr.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wrn.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rwp.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aar.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://gye.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://nqm.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://dyj.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://qim.aizwys.cn

[C05] 返回多个值
来源：http://sdm.daria6918.cn

Py:   return a, b
来源：http://ffc.shuidangran.top

PHP:  return [$a, $b];
来源：http://sdr.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lts.fktsv.cn

TS:   return { a, b };
来源：http://wre.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vva.xylfe.cn

Go:   return a, b
来源：http://kku.wangshuangyany.cn

Ruby: return a, b
来源：http://mer.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://arv.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://ebw.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://lcp.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kry.daxiang520.top

JS:   const square = x => x * x;
来源：http://zqp.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://pra.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yhs.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://qfi.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://fnz.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mhw.aizwys.cn

[C07] 把函数作为参数传入
来源：http://ikf.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uke.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://rzc.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wzj.andypj.xyz

TS:   arr.map(String)
来源：http://dcp.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qcr.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tov.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://wjz.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kye.fanxiaobao.xyz

[C08] 闭包
来源：http://jpe.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vcy.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rmg.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tsk.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvc.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hca.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jwy.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wbb.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ftw.hfpthk.cn

[C09] 递归
来源：http://gzo.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vmh.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iwq.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tnd.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uub.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hbl.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lzp.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhm.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://too.zdbjq.cn

[C10] 变量作用域
来源：http://gsb.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://llh.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wrq.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pjh.cdnleiting.top

TS:   同 JS
来源：http://bst.hcnkem.com

Java: 方法内为块级作用域
来源：http://cwl.tianlin.xyz

Go:   花括号块级作用域
来源：http://gzt.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://owg.sxryk.cn

C#:   块级作用域
来源：http://jbr.jinqigufen.top

[C11] 模块导入与导出
来源：http://cbt.jinqigufen.top

Py:   from module import func
来源：http://hbj.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://umx.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://hlh.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kmo.fanxiaobao.xyz

Java: import java.util.List;
来源：http://dgx.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yza.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://xvx.birdmap.top

C#:   using System.Text;
来源：http://uuf.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://xlu.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://hbq.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://amo.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://kph.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://cra.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fsm.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://axk.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://nga.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kna.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://mjb.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uee.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvh.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://inp.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://okv.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://nsw.yj20258888.top

Go:   func add(a, b int) int
来源：http://cvg.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pjp.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://xso.hnqzz.top

[C14] 泛型函数
来源：http://ecm.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rep.smart0.xyz

PHP:  // 无泛型
来源：http://hxt.redwolf501.top

JS:   // 无泛型
来源：http://xzg.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ojb.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://inu.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmp.jyoumei.cn

Ruby: # 无泛型
来源：http://soq.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://div.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://yay.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nzz.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://age.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://san.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://abz.shangyingyoupin.top

Java: // 无解构
来源：http://uvd.jianghu66.top

Go:   // 无解构
来源：http://jiz.xinyue.icu

Ruby: a, b = pair
来源：http://uqo.guannengcc.top

C#:   var (a, b) = pair;
来源：http://dvx.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://ief.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nxm.zhongyouzk.top

PHP:  // 无重载
来源：http://iir.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vem.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://cgo.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kko.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://lfd.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://dkb.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ofc.quarkkingdee.top

================================================================================
来源：http://czr.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://jzb.uphjek.com

================================================================================
来源：http://wlv.yueranfly.top

[D01] 创建数组 / 列表
来源：http://niv.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tii.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqs.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qam.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zye.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hlo.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://cut.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://jhy.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qig.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://boq.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zgk.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rfh.yfazqb.com

JS:   arr.push(4);
来源：http://sfx.svipenyu.cn

TS:   arr.push(4);
来源：http://qfy.dianchejie.cn

Java: list.add(4);
来源：http://dki.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://nrt.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://fhs.daria6918.cn

C#:   list.Add(4);
来源：http://lqg.havefunace.top

[D03] 在指定位置插入元素
来源：http://iha.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://foh.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mhn.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mlx.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://mlm.yonumen.top

Java: list.add(0, 0);
来源：http://oor.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://opp.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mma.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://cns.nanxuanxn.top

[D04] 删除元素
来源：http://sgp.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fft.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://brp.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cov.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://yjo.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vla.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhe.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fvk.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wrq.yangfankeji.com

[D05] 访问与修改元素
来源：http://erg.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ukk.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ets.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xgb.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://aqs.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://ocz.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://gwc.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nwp.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tmk.jiagoushi.top

[D06] 数组长度
来源：http://dmc.xylfe.cn

Py:   len(arr)
来源：http://xod.0kj1m.cn

PHP:  count($arr);
来源：http://iyk.dianchejie.cn

JS:   arr.length
来源：http://yqd.gotoacloud.top

TS:   arr.length
来源：http://wdm.tarul.cn

Java: list.size();
来源：http://mdp.316326.xyz

Go:   len(arr)
来源：http://ejv.iojbl.cn

Ruby: arr.length; arr.size
来源：http://ohh.ydjk.org.cn

C#:   list.Count;
来源：http://hje.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://bfg.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zac.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yfc.yj20258.top

JS:   arr.slice(1, 4);
来源：http://qsr.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://mrg.wangdashe.top

Java: list.subList(1, 4);
来源：http://ehn.wangdashe.top

Go:   arr[1:4]
来源：http://wtk.nanxinkj.top

Ruby: arr[1, 3]
来源：http://spy.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://imn.sysykeji.top

[D08] 合并两个数组
来源：http://yxy.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://xhf.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://udd.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dse.hfpthk.cn

TS:   [...a, ...b];
来源：http://luc.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ojd.tianlin.xyz

Go:   append(a, b...)
来源：http://lcb.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://pjo.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://qmd.sysykeji.top

[D09] 排序（升序）
来源：http://lhb.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://bfo.hammf.cn

PHP:  sort($arr);
来源：http://vkm.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mem.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://buk.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lhw.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jql.gzhubu.top

Ruby: arr.sort
来源：http://fdh.hongshengwenyu.top

C#:   list.Sort();
来源：http://ynu.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zvk.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nqk.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eac.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvw.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ypm.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tll.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sli.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ene.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dtg.fanxiaobao.xyz

[D11] 反转数组
来源：http://qep.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ypv.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://stl.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://acz.316326.xyz

TS:   [...arr].reverse();
来源：http://iuf.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://zcz.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://cip.tian-w.cn

Ruby: arr.reverse
来源：http://llb.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://smt.hongshengwenyu.top

[D12] 查找元素下标
来源：http://prg.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://kal.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vju.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogd.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzc.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ucq.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://pae.ydzc1.top

Ruby: arr.index(x)
来源：http://uhn.mhx1999.top

C#:   list.IndexOf(x);
来源：http://nim.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://ojs.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jjz.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://odj.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://lhr.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://ien.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rgd.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bbr.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bsj.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jfh.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://oyc.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jis.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yok.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://wct.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://uyn.fktsv.cn


<!-- 参考信息 -->