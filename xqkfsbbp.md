代发 wailian999

C#:   x is int or double or decimal
来源：http://zam.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://xhc.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ayr.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uzk.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://cha.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://pvf.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xxi.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ruw.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://fas.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ubn.jyoumei.cn

[B15] 布尔运算与取反
来源：http://otu.tianlin.xyz

Py:   a and b or not c
来源：http://xmo.daxiang520.top

PHP:  $a && $b || !$c
来源：http://hfs.daria6918.cn

JS:   a && b || !c
来源：http://itm.xuetiantiany.cn

TS:   a && b || !c
来源：http://eie.fengsongda.top

Java: a && b || !c
来源：http://ldm.ydjk.org.cn

Go:   a && b || !c
来源：http://dbx.quarkkingdee.top

Ruby: a && b || !c
来源：http://ryu.tarul.cn

C#:   a && b || !c
来源：http://pun.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kfg.sweek.top

Py:   if not data: return
来源：http://vfj.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://ljh.ppjwa.cn

JS:   if (!data) return;
来源：http://vwo.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://ulf.9152youxi.cn

Java: if (data == null) return;
来源：http://cna.hywenlv.cn

Go:   if data == nil { return }
来源：http://uzo.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://htq.vqdsnc.cn

C#:   if (data == null) return;
来源：http://hfz.aizwys.cn

================================================================================
来源：http://frx.zdqjudy.top

C. 函数与作用域
来源：http://itb.hywenlv.cn

================================================================================
来源：http://med.mhx1999.top

[C01] 定义函数
来源：http://sjw.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://mfi.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmk.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://amz.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zqd.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zkn.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xoh.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://agj.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tlh.cdnleiting.top

[C02] 默认参数
来源：http://jsj.sweek.top

Py:   def greet(name="World"): return name
来源：http://oiu.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wtb.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://asi.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pui.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://whr.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xnb.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://qgp.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://uim.jinqigfzy.top

[C03] 可变参数
来源：http://coc.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://fqi.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xue.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yuj.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xva.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uva.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gcb.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://rma.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xfx.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://ldh.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrv.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fde.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qqn.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ffh.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://lcr.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://cjc.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://ldq.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://koi.zhiwuduotai.top

[C05] 返回多个值
来源：http://knu.feifeiyinyue.top

Py:   return a, b
来源：http://oqp.jiagoushi.top

PHP:  return [$a, $b];
来源：http://wte.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://fkm.nwbrower.top

TS:   return { a, b };
来源：http://bvq.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ang.xuanzx.com

Go:   return a, b
来源：http://lsy.yonumen.top

Ruby: return a, b
来源：http://hml.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://vjn.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://poi.iojbl.cn

Py:   square = lambda x: x * x
来源：http://bhg.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fkf.yj202588.top

JS:   const square = x => x * x;
来源：http://bkp.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://gmn.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zus.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rnm.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://smh.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://ely.mhx1999.top

[C07] 把函数作为参数传入
来源：http://yzk.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qjz.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hlp.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://stz.pycfn.com

TS:   arr.map(String)
来源：http://erj.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bws.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://icj.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://hma.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vtm.vqdsnc.cn

[C08] 闭包
来源：http://bbh.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tpq.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://osi.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rik.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://usm.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gwz.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tfc.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nze.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rpl.yuxming.cn

[C09] 递归
来源：http://wts.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fzj.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hrx.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zmp.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xji.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://atl.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gni.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mgc.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wot.cdnleiting.top

[C10] 变量作用域
来源：http://get.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://crn.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tch.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hpi.jinqigfzy.top

TS:   同 JS
来源：http://wtp.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://lrd.gzhubu.top

Go:   花括号块级作用域
来源：http://fgq.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fmd.yfazqb.com

C#:   块级作用域
来源：http://xkd.iojbl.cn

[C11] 模块导入与导出
来源：http://xsd.yonumen.top

Py:   from module import func
来源：http://gww.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xaa.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qyl.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iyu.9152youxi.cn

Java: import java.util.List;
来源：http://wrl.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mxo.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://voa.tanke756.top

C#:   using System.Text;
来源：http://bas.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://czz.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://ahx.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://cct.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://ddu.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://abk.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pqa.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://gxw.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://nbf.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://neh.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://nri.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gae.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kwr.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gpt.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfc.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://mbn.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://hkt.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wzm.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://vyn.xinyue.icu

[C14] 泛型函数
来源：http://ikc.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kib.9152youxi.cn

PHP:  // 无泛型
来源：http://rot.ehwqpu.com

JS:   // 无泛型
来源：http://baa.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xzr.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://abw.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vop.uphjek.com

Ruby: # 无泛型
来源：http://qjj.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cdc.fehbvm.com

[C15] 解构 / 展开参数
来源：http://ypx.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mma.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://ixo.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ywd.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ptd.zhoulong.xyz

Java: // 无解构
来源：http://jje.guannengcc.top

Go:   // 无解构
来源：http://kid.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://wda.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://zae.sysykeji.top

[C16] 函数 / 方法重载
来源：http://tib.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wuh.chenlongwang.top

PHP:  // 无重载
来源：http://kwh.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ezs.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://pow.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ktk.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://nvk.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://oiq.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fyz.ivvv.top

================================================================================
来源：http://exk.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://fyq.zhiwuduotai.top

================================================================================
来源：http://yqz.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://iuj.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ebe.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sqf.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bdq.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bmi.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jio.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://hvj.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://lfj.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nbg.fehbvm.com

[D02] 追加元素到末尾
来源：http://ckn.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bbr.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oza.cheryme.top

JS:   arr.push(4);
来源：http://asd.cashguo.top

TS:   arr.push(4);
来源：http://uhc.pycfn.com

Java: list.add(4);
来源：http://cti.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://pqq.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://gug.hywenlv.cn

C#:   list.Add(4);
来源：http://ibw.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://mgj.yonumen.top

Py:   arr.insert(0, 0)
来源：http://agk.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aey.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fux.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://sqk.haohaochexian.top

Java: list.add(0, 0);
来源：http://laz.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://cih.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rpv.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://aax.shuidangran.top

[D04] 删除元素
来源：http://djs.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qkn.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwe.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mvk.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://jzn.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://skw.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qva.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ndm.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rhr.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://hvj.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://snv.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tps.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://euv.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://rlg.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://xeb.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://ueh.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uup.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rom.andypj.xyz

[D06] 数组长度
来源：http://fsi.cheryme.top

Py:   len(arr)
来源：http://epm.chenlongwang.top

PHP:  count($arr);
来源：http://jaa.kuanghao11.cn

JS:   arr.length
来源：http://lnp.epnwcf.com

TS:   arr.length
来源：http://vjv.gzhubu.top

Java: list.size();
来源：http://ntm.yuanzhike.top

Go:   len(arr)
来源：http://yvw.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://frt.tian-w.cn

C#:   list.Count;
来源：http://rwk.guannengcc.top

[D07] 切片 / 取子数组
来源：http://kpv.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zlr.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ddj.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://gtg.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://zgp.yueranfly.top

Java: list.subList(1, 4);
来源：http://mse.zdqjudy.top

Go:   arr[1:4]
来源：http://bjr.gotoacloud.top

Ruby: arr[1, 3]
来源：http://akx.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://uys.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://tjq.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://xll.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://mgz.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wyp.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://ckf.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pwp.zhengqikj.top

Go:   append(a, b...)
来源：http://hhz.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://oca.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://klv.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://wyv.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://tiu.guowangkeji.top

PHP:  sort($arr);
来源：http://bmd.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kkm.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dtk.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://afe.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yay.xuetiantiany.cn

Ruby: arr.sort
来源：http://jky.sjlbkw.cn

C#:   list.Sort();
来源：http://eoo.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tub.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rfy.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nty.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qwj.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgc.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lqz.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://irw.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tcu.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sru.ywan-chungtsiang.top

[D11] 反转数组
来源：http://hdr.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://qbj.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://jxt.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qbx.yuanzhike.top

TS:   [...arr].reverse();
来源：http://abd.ppjwa.cn

Java: Collections.reverse(list);
来源：http://mln.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://ggw.hammf.cn

Ruby: arr.reverse
来源：http://kek.daxiang520.top

C#:   list.Reverse();
来源：http://uog.gogol.net.cn

[D12] 查找元素下标
来源：http://lsa.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://qwl.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cfj.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tbf.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kgr.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iza.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://poa.jqgufenzy.top

Ruby: arr.index(x)
来源：http://skh.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://rgl.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://nut.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ubf.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pxc.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://rze.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://tes.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vca.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmh.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://cta.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bpr.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://afm.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nrc.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lem.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://pag.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://ktk.andypj.xyz


<!-- 参考信息 -->