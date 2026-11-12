代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbf.fzhhl.top

Java: x instanceof Number
来源：http://hks.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xzr.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://gle.daria6918.cn

C#:   x is int or double or decimal
来源：http://dmk.yuxming.cn

[B14] 判断值是否在集合内
来源：http://nza.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mcp.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://crz.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://mqt.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://lxn.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yjh.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oeq.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pui.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uci.ydzc1.top

[B15] 布尔运算与取反
来源：http://fbi.guannengcc.top

Py:   a and b or not c
来源：http://dng.sysykeji.top

PHP:  $a && $b || !$c
来源：http://xoj.tian-w.cn

JS:   a && b || !c
来源：http://rpb.hesvh.cn

TS:   a && b || !c
来源：http://ipx.hesvh.cn

Java: a && b || !c
来源：http://nah.yfazqb.com

Go:   a && b || !c
来源：http://gwf.tanke756.top

Ruby: a && b || !c
来源：http://imk.fanxiaobao.xyz

C#:   a && b || !c
来源：http://hnt.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://ibu.hnxiangtu.top

Py:   if not data: return
来源：http://esl.hammf.cn

PHP:  if (!$data) { return; }
来源：http://pcl.shangyingyoupin.top

JS:   if (!data) return;
来源：http://wgb.zhengqikj.top

TS:   if (!data) return;
来源：http://efw.gogol.net.cn

Java: if (data == null) return;
来源：http://ikw.tarul.cn

Go:   if data == nil { return }
来源：http://rzf.sysykeji.top

Ruby: return if data.nil?
来源：http://qms.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://thj.mhx1999.top

================================================================================
来源：http://okd.yueranfly.top

C. 函数与作用域
来源：http://djl.jlsjyb.cn

================================================================================
来源：http://cso.shzxlz.cn

[C01] 定义函数
来源：http://faz.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://tmy.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aay.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://kmk.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xro.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zaq.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xzc.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://trt.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vxg.yj20258888.top

[C02] 默认参数
来源：http://qhb.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://yhy.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://its.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://atr.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zui.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fev.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://trj.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://vtl.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://jpj.0kj1m.cn

[C03] 可变参数
来源：http://byr.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://tqq.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vkc.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkg.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xux.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ibd.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wpy.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://lkv.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zfc.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://lll.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ojx.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fgm.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://slh.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jrd.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://jgp.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://aal.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://cnl.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://uxb.gzhubu.top

[C05] 返回多个值
来源：http://bfe.guowangkeji.top

Py:   return a, b
来源：http://sxj.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://jyr.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kjd.chenjidiqi.icu

TS:   return { a, b };
来源：http://gov.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pud.tarul.cn

Go:   return a, b
来源：http://gle.gzhubu.top

Ruby: return a, b
来源：http://kim.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://vfk.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://bbi.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://abc.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pqi.bbcook.cn

JS:   const square = x => x * x;
来源：http://rbt.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://gtt.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://urf.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://swi.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://nkk.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fux.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://cfl.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mob.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://fiv.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oil.yuxming.cn

TS:   arr.map(String)
来源：http://edp.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rza.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rrs.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://wak.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dun.316326.xyz

[C08] 闭包
来源：http://oec.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dlu.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fbs.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cup.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://drl.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dqh.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mcq.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jdv.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uav.pycfn.com

[C09] 递归
来源：http://xwt.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwm.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bwd.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdn.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cub.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fqb.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayo.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ieg.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vdw.kuanghao11.cn

[C10] 变量作用域
来源：http://zii.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dgq.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ebn.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dwc.wangdashe.top

TS:   同 JS
来源：http://qgl.yvedp.cn

Java: 方法内为块级作用域
来源：http://xpr.yangfankeji.com

Go:   花括号块级作用域
来源：http://val.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fzm.hnxiangtu.top

C#:   块级作用域
来源：http://bsl.xuanzx.com

[C11] 模块导入与导出
来源：http://lks.ywan-chungtsiang.top

Py:   from module import func
来源：http://clw.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cef.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ult.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://acb.xylfe.cn

Java: import java.util.List;
来源：http://dde.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://myj.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://yck.aibaodan.cn

C#:   using System.Text;
来源：http://lgt.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://lzz.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://xdd.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://vge.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://xvm.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://hgf.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jke.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://diz.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://puj.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ncu.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://zxm.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fpc.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uuz.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wmx.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zzb.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hec.cucudq.cn

Go:   func add(a, b int) int
来源：http://yhg.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zzq.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://rgc.hnxiangtu.top

[C14] 泛型函数
来源：http://els.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nty.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://hjl.nwbrower.top

JS:   // 无泛型
来源：http://ezl.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://apl.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pjs.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jgv.jyoumei.cn

Ruby: # 无泛型
来源：http://cfk.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://psz.ivvv.top

[C15] 解构 / 展开参数
来源：http://uvi.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ciy.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://rkb.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyg.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dnb.cheryme.top

Java: // 无解构
来源：http://yry.316326.xyz

Go:   // 无解构
来源：http://hfw.tian-w.cn

Ruby: a, b = pair
来源：http://buh.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://qes.daxiang520.top

[C16] 函数 / 方法重载
来源：http://yge.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mwg.316326.xyz

PHP:  // 无重载
来源：http://wxu.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zfr.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://gtn.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wkt.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://per.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://ivi.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ppy.meibo888.top

================================================================================
来源：http://rut.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://dwx.ywan-chungtsiang.top

================================================================================
来源：http://lwm.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://dkw.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tvo.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mar.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jbv.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://let.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lit.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://rzo.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://buz.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ilu.cashguo.top

[D02] 追加元素到末尾
来源：http://wkx.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lpe.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nap.gzhubu.top

JS:   arr.push(4);
来源：http://khz.yvedp.cn

TS:   arr.push(4);
来源：http://ozy.daxiang520.top

Java: list.add(4);
来源：http://txy.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://nkm.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://dbr.pycfn.com

C#:   list.Add(4);
来源：http://bgg.cucudq.cn

[D03] 在指定位置插入元素
来源：http://pcf.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://lbc.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ybz.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nxd.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://qxa.kuanghao11.cn

Java: list.add(0, 0);
来源：http://xhq.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://vfd.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzj.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://gce.vehdjk.com

[D04] 删除元素
来源：http://dne.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uug.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://okf.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpu.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://kfr.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nle.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sxg.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rgc.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ugt.gotoacloud.top

[D05] 访问与修改元素
来源：http://hnu.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://upu.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ebf.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jwg.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://ioj.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://pvf.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://srs.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tqq.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bao.fktsv.cn

[D06] 数组长度
来源：http://ier.tarul.cn

Py:   len(arr)
来源：http://gsn.mhx1999.top

PHP:  count($arr);
来源：http://rvc.jqgufenzy.top

JS:   arr.length
来源：http://okt.ppjwa.cn

TS:   arr.length
来源：http://jdo.cdnleiting.top

Java: list.size();
来源：http://afr.jlsjyb.cn

Go:   len(arr)
来源：http://ksy.sxryk.cn

Ruby: arr.length; arr.size
来源：http://kkj.tian-w.cn

C#:   list.Count;
来源：http://azr.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://nyg.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vct.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://aav.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://rnx.havefunace.top

TS:   arr.slice(1, 4);
来源：http://gli.tian-w.cn

Java: list.subList(1, 4);
来源：http://cih.bjfxy.top

Go:   arr[1:4]
来源：http://ckq.hfpthk.cn

Ruby: arr[1, 3]
来源：http://kfp.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://dhb.guowangkeji.top

[D08] 合并两个数组
来源：http://wtz.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://oxu.uphjek.com

PHP:  array_merge($a, $b);
来源：http://ayf.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kse.shzxlz.cn

TS:   [...a, ...b];
来源：http://jrc.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ohx.jianghu66.top

Go:   append(a, b...)
来源：http://ier.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://hik.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://had.andypj.xyz

[D09] 排序（升序）
来源：http://djv.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://ojs.nanxuanxn.top

PHP:  sort($arr);
来源：http://who.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://okg.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jyh.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mur.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aiu.cdnleiting.top

Ruby: arr.sort
来源：http://dlx.fengsongda.top

C#:   list.Sort();
来源：http://urz.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://frf.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vfk.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eir.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wvx.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fja.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yma.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awx.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cws.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ajg.yfazqb.com

[D11] 反转数组
来源：http://hlv.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://khj.gzhubu.top

PHP:  array_reverse($arr);
来源：http://pot.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cgv.xylfe.cn

TS:   [...arr].reverse();
来源：http://plx.9152youxi.cn

Java: Collections.reverse(list);
来源：http://kay.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://lbq.zhixingplan.top

Ruby: arr.reverse
来源：http://qsj.hnqzz.top

C#:   list.Reverse();
来源：http://gsj.ivvv.top

[D12] 查找元素下标
来源：http://mgi.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://tyg.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://weo.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xyr.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lct.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dar.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://wys.pycfn.com

Ruby: arr.index(x)
来源：http://qmv.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://fxr.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://xgz.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fum.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayc.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://job.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://zah.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cgy.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xhe.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cwn.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wcm.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://piw.andypj.xyz


<!-- 参考信息 -->