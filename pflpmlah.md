代发 wailian999

PHP:  range(0, 10, 2);
来源：http://lut.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pjc.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owl.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ygb.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vep.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://grz.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cqp.fengsongda.top

[B12] 跳出多层循环
来源：http://yci.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lyz.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xcp.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvi.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ruk.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mke.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dxl.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ghp.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yfq.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://gjy.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://pet.fengsongda.top

PHP:  is_numeric($x)
来源：http://anr.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cmc.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fsm.fktsv.cn

Java: x instanceof Number
来源：http://jab.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nqa.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://wbd.jqgfzy.top

C#:   x is int or double or decimal
来源：http://pss.yj20258888.top

[B14] 判断值是否在集合内
来源：http://kzk.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pkz.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oqx.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://xkg.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://bwu.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lcv.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kwb.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://frs.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ewj.ppjwa.cn

[B15] 布尔运算与取反
来源：http://jzz.andypj.xyz

Py:   a and b or not c
来源：http://kam.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://brc.meibo888.top

JS:   a && b || !c
来源：http://fdq.ydzc1.top

TS:   a && b || !c
来源：http://dfo.xuetiantiany.cn

Java: a && b || !c
来源：http://uin.dashuyun.cn

Go:   a && b || !c
来源：http://kwu.zhijiandao.cn

Ruby: a && b || !c
来源：http://rbz.fzhhl.top

C#:   a && b || !c
来源：http://hky.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lsk.sxryk.cn

Py:   if not data: return
来源：http://ndt.yonumen.top

PHP:  if (!$data) { return; }
来源：http://bmt.sjlbkw.cn

JS:   if (!data) return;
来源：http://zcs.uphjek.com

TS:   if (!data) return;
来源：http://ssp.ivvv.top

Java: if (data == null) return;
来源：http://zmd.daxiang520.top

Go:   if data == nil { return }
来源：http://xmt.yuxming.cn

Ruby: return if data.nil?
来源：http://ncj.gzhubu.top

C#:   if (data == null) return;
来源：http://oio.zhiwuduotai.top

================================================================================
来源：http://qri.chenzaomai.com

C. 函数与作用域
来源：http://nqt.jinghuilouyu.cn

================================================================================
来源：http://agv.aizwys.cn

[C01] 定义函数
来源：http://ndn.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://kpt.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbm.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://upk.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjn.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://doa.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://ivq.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://mgu.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lil.sweek.top

[C02] 默认参数
来源：http://vgd.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://fre.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vji.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://fpp.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://lry.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://eso.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oep.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://eub.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://jhd.316326.xyz

[C03] 可变参数
来源：http://jxc.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://rbq.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pta.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yot.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozl.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wge.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eaw.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kbn.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://epr.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://dvh.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://amh.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phz.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fvn.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lld.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://kfz.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://fvd.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://idb.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://dnj.yj20258.top

[C05] 返回多个值
来源：http://ten.yj20258.top

Py:   return a, b
来源：http://iaf.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://joq.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bal.bjfxy.top

TS:   return { a, b };
来源：http://oou.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mwa.guannengcc.top

Go:   return a, b
来源：http://uow.sxryk.cn

Ruby: return a, b
来源：http://ttn.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://hqj.ivvv.top

[C06] 匿名函数 / lambda
来源：http://kbw.daria6918.cn

Py:   square = lambda x: x * x
来源：http://igz.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bpv.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://vkj.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://nad.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ewa.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://rqw.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://ons.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://aym.mhx1999.top

[C07] 把函数作为参数传入
来源：http://igd.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tbh.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://wng.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ssa.xuanzx.com

TS:   arr.map(String)
来源：http://nko.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tcq.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aec.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://zjl.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nmv.yueranfly.top

[C08] 闭包
来源：http://ssk.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nhg.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xxn.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xfo.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://peb.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gyg.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fng.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://urr.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vmo.xuanzx.com

[C09] 递归
来源：http://dzo.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hay.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://viz.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ffy.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkv.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oun.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ztx.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zoa.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pam.smart0.xyz

[C10] 变量作用域
来源：http://zdc.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lay.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cvf.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gxn.daria6918.cn

TS:   同 JS
来源：http://ndn.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://paw.ppjwa.cn

Go:   花括号块级作用域
来源：http://jdp.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://npm.yfazqb.com

C#:   块级作用域
来源：http://btf.snrcjt.cn

[C11] 模块导入与导出
来源：http://pmc.yanxiufei.cn

Py:   from module import func
来源：http://mst.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lpf.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yfy.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yfy.vehdjk.com

Java: import java.util.List;
来源：http://htb.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jcz.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://oeh.yuxming.cn

C#:   using System.Text;
来源：http://uoz.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://ues.havefunace.top

Py:   (lambda: print("run"))()
来源：http://jfa.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://qcf.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://dco.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://vol.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sfn.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://vmg.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://dwj.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fxu.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://zqs.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nge.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pey.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://irf.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qug.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kwk.zdqjudy.top

Go:   func add(a, b int) int
来源：http://dwl.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://itq.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://fgz.nanxuanxn.top

[C14] 泛型函数
来源：http://kom.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zbj.birdmap.top

PHP:  // 无泛型
来源：http://tmm.zdbjq.cn

JS:   // 无泛型
来源：http://eiz.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aon.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xdu.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lao.xuanzx.com

Ruby: # 无泛型
来源：http://fmw.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qeb.yueranfly.top

[C15] 解构 / 展开参数
来源：http://kks.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lvk.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://clg.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uit.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ujt.guannengcc.top

Java: // 无解构
来源：http://lsj.chenlongwang.top

Go:   // 无解构
来源：http://ekz.sweek.top

Ruby: a, b = pair
来源：http://saa.tian-w.cn

C#:   var (a, b) = pair;
来源：http://bbg.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://qps.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://esi.gzhubu.top

PHP:  // 无重载
来源：http://flh.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ens.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://ytu.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ljl.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://nfj.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://kdq.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wfc.jinghuilouyu.cn

================================================================================
来源：http://cgu.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://xot.sxryk.cn

================================================================================
来源：http://lqk.yueranfly.top

[D01] 创建数组 / 列表
来源：http://wcj.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://lbg.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zbv.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ouw.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://khv.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ugf.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://zyq.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://cys.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wjm.fzhhl.top

[D02] 追加元素到末尾
来源：http://prg.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mbm.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ugp.9152youxi.cn

JS:   arr.push(4);
来源：http://ziv.0kj1m.cn

TS:   arr.push(4);
来源：http://kna.epnwcf.com

Java: list.add(4);
来源：http://gjs.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://bqr.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://kkf.gogol.net.cn

C#:   list.Add(4);
来源：http://vxl.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://uus.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://aqm.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gfs.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ggf.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://lpb.mhx1999.top

Java: list.add(0, 0);
来源：http://fum.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://guq.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vzu.yonumen.top

C#:   list.Insert(0, 0);
来源：http://ekc.yanxiufei.cn

[D04] 删除元素
来源：http://tvi.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://koe.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lqz.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tfy.birdmap.top

TS:   arr.splice(0, 1);
来源：http://fto.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rww.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wil.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jyy.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qws.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://qcp.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wyx.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccu.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yam.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://tqf.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://frc.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://rhg.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kzk.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vne.fengsongda.top

[D06] 数组长度
来源：http://xqy.xuetiantiany.cn

Py:   len(arr)
来源：http://jhz.0kj1m.cn

PHP:  count($arr);
来源：http://tjs.xziqi.cn

JS:   arr.length
来源：http://edx.hywenlv.cn

TS:   arr.length
来源：http://pbf.ehwqpu.com

Java: list.size();
来源：http://jde.chenzaomai.com

Go:   len(arr)
来源：http://xgg.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://btz.c1oappe.top

C#:   list.Count;
来源：http://gsq.316326.xyz

[D07] 切片 / 取子数组
来源：http://rys.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dyd.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://llv.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://mqm.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://bqs.aizwys.cn

Java: list.subList(1, 4);
来源：http://wdu.gaohongyu789.top

Go:   arr[1:4]
来源：http://zgv.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://qiy.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://uav.zdqjudy.top

[D08] 合并两个数组
来源：http://awn.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://ckf.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://uxa.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://lws.ydzc1.top

TS:   [...a, ...b];
来源：http://igz.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kuc.daxiang520.top

Go:   append(a, b...)
来源：http://bpi.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://hud.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://ent.jlsjyb.cn

[D09] 排序（升序）
来源：http://oyj.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://ngy.0kj1m.cn

PHP:  sort($arr);
来源：http://cud.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://czs.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mpr.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nkv.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hcv.ivvv.top

Ruby: arr.sort
来源：http://wfr.zhoulong.xyz

C#:   list.Sort();
来源：http://zbk.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ves.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://egl.cucudq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sdu.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://luv.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://usj.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tgn.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gzi.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rhj.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wqa.chenzaomai.com

[D11] 反转数组
来源：http://yux.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://aek.yfazqb.com

PHP:  array_reverse($arr);
来源：http://nvt.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mex.gotoacloud.top

TS:   [...arr].reverse();
来源：http://kfu.daxiang520.top

Java: Collections.reverse(list);
来源：http://jip.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://fmz.ybcxt.top

Ruby: arr.reverse
来源：http://cpd.jqgfzy.top


<!-- 参考信息 -->