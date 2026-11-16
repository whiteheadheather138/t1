代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlv.aizwys.cn

Java: x instanceof Number
来源：http://cki.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jzr.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://kqc.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://akb.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://vtn.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zjw.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oqw.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://cvi.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://dcy.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mgy.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydy.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://sxm.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zea.snrcjt.cn

[B15] 布尔运算与取反
来源：http://eok.shangyingyoupin.top

Py:   a and b or not c
来源：http://ubj.smart0.xyz

PHP:  $a && $b || !$c
来源：http://klg.yvedp.cn

JS:   a && b || !c
来源：http://thy.havefunace.top

TS:   a && b || !c
来源：http://flo.havefunace.top

Java: a && b || !c
来源：http://mqt.yj20258.top

Go:   a && b || !c
来源：http://aop.hysaishi.cn

Ruby: a && b || !c
来源：http://cgf.yonumen.top

C#:   a && b || !c
来源：http://fka.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://xbr.fehbvm.com

Py:   if not data: return
来源：http://fqe.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://fvt.meibo888.top

JS:   if (!data) return;
来源：http://okr.daxiang520.top

TS:   if (!data) return;
来源：http://ofx.dashuyun.cn

Java: if (data == null) return;
来源：http://zud.fehbvm.com

Go:   if data == nil { return }
来源：http://sgk.sjlbkw.cn

Ruby: return if data.nil?
来源：http://fen.tanke756.top

C#:   if (data == null) return;
来源：http://vup.jqgufenzy.top

================================================================================
来源：http://opg.shuidangran.top

C. 函数与作用域
来源：http://vsb.zdbjq.cn

================================================================================
来源：http://czm.fehbvm.com

[C01] 定义函数
来源：http://xra.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://ybd.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvg.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gzp.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bdn.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://prw.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://ymk.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://ytj.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ybz.yueranfly.top

[C02] 默认参数
来源：http://jaf.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://vhp.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mdw.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://qgp.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uai.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yka.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qdu.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://pnn.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://tab.andypj.xyz

[C03] 可变参数
来源：http://ubv.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://ayr.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fnt.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://est.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cfw.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tsz.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://goe.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://jsz.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mmi.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://olf.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rdt.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ysz.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nia.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ryt.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://mug.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://osq.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://ttt.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://dqv.svipenyu.cn

[C05] 返回多个值
来源：http://sdb.gaohongyu789.top

Py:   return a, b
来源：http://cgm.mhx1999.top

PHP:  return [$a, $b];
来源：http://nyo.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gvu.zhixingplan.top

TS:   return { a, b };
来源：http://tal.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yxr.vehdjk.com

Go:   return a, b
来源：http://ptw.gaohongyu789.top

Ruby: return a, b
来源：http://yhc.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://cti.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://jjk.iojbl.cn

Py:   square = lambda x: x * x
来源：http://xlf.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://sxg.ppjwa.cn

JS:   const square = x => x * x;
来源：http://wpx.dianchejie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ljs.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ysh.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://xvp.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://kau.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mcr.sxryk.cn

[C07] 把函数作为参数传入
来源：http://hpf.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dpw.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://kjo.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bbq.zhongyouzk.top

TS:   arr.map(String)
来源：http://clv.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://stj.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nje.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://jta.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://toy.zhaomingkeji.xyz

[C08] 闭包
来源：http://hvo.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mjq.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wfm.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eij.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xop.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hjr.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rmp.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uij.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ykq.jqgfzy.top

[C09] 递归
来源：http://gzs.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ufr.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://btd.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cmd.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bei.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hlv.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://njt.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cto.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wro.havefunace.top

[C10] 变量作用域
来源：http://jsw.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nnf.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://egp.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zgq.xziqi.cn

TS:   同 JS
来源：http://krh.chenlongwang.top

Java: 方法内为块级作用域
来源：http://ziz.yj20258.top

Go:   花括号块级作用域
来源：http://wxa.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://urp.zycfv.cn

C#:   块级作用域
来源：http://sxe.shzxlz.cn

[C11] 模块导入与导出
来源：http://vzb.quarkkingdee.top

Py:   from module import func
来源：http://sjy.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vce.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rzt.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdr.ivvv.top

Java: import java.util.List;
来源：http://xbk.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vez.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://bhn.yj20258888.top

C#:   using System.Text;
来源：http://lmc.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://zrf.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://nng.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://qfd.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://crp.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://lgv.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://htt.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://eqn.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://hgy.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://jku.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://rfm.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xws.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oht.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ask.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjz.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ctf.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://iap.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://exo.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://icf.gzhubu.top

[C14] 泛型函数
来源：http://eyb.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xrk.yongpay.top

PHP:  // 无泛型
来源：http://spp.dianchejie.cn

JS:   // 无泛型
来源：http://hqs.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://skf.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oea.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ear.hywenlv.cn

Ruby: # 无泛型
来源：http://rnh.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nsm.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://tov.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nxk.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://tuw.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zyy.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yme.xuanzx.com

Java: // 无解构
来源：http://qnl.sxryk.cn

Go:   // 无解构
来源：http://jcv.feifeiyinyue.top

Ruby: a, b = pair
来源：http://vhw.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://ubv.52xcode.cn

[C16] 函数 / 方法重载
来源：http://zhw.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ajr.hesvh.cn

PHP:  // 无重载
来源：http://npi.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://djf.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://lhp.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://fdp.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://maf.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://hyn.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgh.jinqigufen.top

================================================================================
来源：http://ujf.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://iai.shanyushiyangkeji.top

================================================================================
来源：http://kcz.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://req.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kfr.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uan.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jva.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://khv.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rhy.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://cir.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://xvq.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xuq.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://zcl.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rby.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aag.fengsongda.top

JS:   arr.push(4);
来源：http://wnu.316326.xyz

TS:   arr.push(4);
来源：http://qft.sweek.top

Java: list.add(4);
来源：http://ksb.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://sru.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://yvb.aizwys.cn

C#:   list.Add(4);
来源：http://jre.uphjek.com

[D03] 在指定位置插入元素
来源：http://prg.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://iib.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hhz.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://coh.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://rwh.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://ipb.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://saq.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yuw.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://snc.ywan-chungtsiang.top

[D04] 删除元素
来源：http://dqr.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rnw.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ihl.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pct.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://opk.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvq.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eiz.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mge.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hsi.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://lnu.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qyk.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pyg.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vkf.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://uvf.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://kyq.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://vnb.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fpi.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vtw.jianghu66.top

[D06] 数组长度
来源：http://tzz.zdqjudy.top

Py:   len(arr)
来源：http://soy.hnqzz.top

PHP:  count($arr);
来源：http://dqj.aizwys.cn

JS:   arr.length
来源：http://mnv.quarkkingdee.top

TS:   arr.length
来源：http://tkz.haohaochexian.top

Java: list.size();
来源：http://egv.sjlbkw.cn

Go:   len(arr)
来源：http://ubj.xinyue.icu

Ruby: arr.length; arr.size
来源：http://xpn.shuidangran.top

C#:   list.Count;
来源：http://uep.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://vgq.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fgg.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://atf.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://bxx.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://eys.guannengcc.top

Java: list.subList(1, 4);
来源：http://usj.zdqjudy.top

Go:   arr[1:4]
来源：http://fha.daria6918.cn

Ruby: arr[1, 3]
来源：http://hhp.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://bya.shuidangran.top

[D08] 合并两个数组
来源：http://ytz.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://iam.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://bzu.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hkk.zhongyouzk.top

TS:   [...a, ...b];
来源：http://yej.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fxq.jqgfzy.top

Go:   append(a, b...)
来源：http://dxi.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://nly.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://znb.smart0.xyz

[D09] 排序（升序）
来源：http://jaj.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://tvd.yvedp.cn

PHP:  sort($arr);
来源：http://wjc.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://abv.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ysf.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fea.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uvm.yongpay.top

Ruby: arr.sort
来源：http://nrr.vqdsnc.cn

C#:   list.Sort();
来源：http://xhw.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vqf.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ggl.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbf.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xay.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hdc.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://smi.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qcv.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qup.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eum.jinghuilouyu.cn

[D11] 反转数组
来源：http://ylg.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://xva.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://gsd.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wjb.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://nqo.ybcxt.top

Java: Collections.reverse(list);
来源：http://vdf.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://uke.chenlongwang.top

Ruby: arr.reverse
来源：http://scx.vehdjk.com

C#:   list.Reverse();
来源：http://bzh.feifeiyinyue.top

[D12] 查找元素下标
来源：http://eii.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://oac.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rzf.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dsm.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tiq.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pcw.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://kmz.ehwqpu.com

Ruby: arr.index(x)
来源：http://uwy.guannengcc.top

C#:   list.IndexOf(x);
来源：http://che.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://ckk.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blt.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nhl.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://wyv.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://nxc.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://svz.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ctp.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hjc.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://abe.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://kpr.ppjwa.cn


<!-- 参考信息 -->