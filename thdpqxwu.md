代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://jlu.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jsi.jianghu66.top

[B15] 布尔运算与取反
来源：http://xna.chenzaomai.com

Py:   a and b or not c
来源：http://ngt.hesvh.cn

PHP:  $a && $b || !$c
来源：http://ead.bbcook.cn

JS:   a && b || !c
来源：http://abd.yongpay.top

TS:   a && b || !c
来源：http://wxf.zhixingplan.top

Java: a && b || !c
来源：http://ahn.yj20258888.top

Go:   a && b || !c
来源：http://vfh.mhx1999.top

Ruby: a && b || !c
来源：http://rll.birdmap.top

C#:   a && b || !c
来源：http://ygs.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://obi.chenjidiqi.icu

Py:   if not data: return
来源：http://cki.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://ubk.epnwcf.com

JS:   if (!data) return;
来源：http://lgo.redwolf501.top

TS:   if (!data) return;
来源：http://zqz.yongpay.top

Java: if (data == null) return;
来源：http://jgd.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://vop.hcnkem.com

Ruby: return if data.nil?
来源：http://oap.kuanghao11.cn

C#:   if (data == null) return;
来源：http://zro.chenjidiqi.icu

================================================================================
来源：http://fgc.fehbvm.com

C. 函数与作用域
来源：http://vvc.fehbvm.com

================================================================================
来源：http://ofz.ctjpmb.com

[C01] 定义函数
来源：http://rcd.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://vtf.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vas.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://vtb.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kkm.zdbjq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ljp.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://bqd.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://kga.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dpu.jinqigfzy.top

[C02] 默认参数
来源：http://hjb.birdmap.top

Py:   def greet(name="World"): return name
来源：http://dos.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cek.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://iyx.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://afo.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://tbo.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rjs.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://vef.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://che.yangfankeji.com

[C03] 可变参数
来源：http://jdc.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://kxw.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qru.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gre.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cdr.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wfs.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lst.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vge.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mga.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://mnl.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vhk.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jva.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eou.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bdm.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://lee.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://knk.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://xdn.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://qrb.hammf.cn

[C05] 返回多个值
来源：http://hfc.fengsongda.top

Py:   return a, b
来源：http://bna.cqqwz.cn

PHP:  return [$a, $b];
来源：http://iqt.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://guk.sxryk.cn

TS:   return { a, b };
来源：http://bpc.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oar.andypj.xyz

Go:   return a, b
来源：http://dmm.gotoacloud.top

Ruby: return a, b
来源：http://fvb.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://msu.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://evq.yj202588.top

Py:   square = lambda x: x * x
来源：http://ijt.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qbj.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://hmy.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://odw.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mks.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://xgt.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://xyq.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://qeq.yueranfly.top

[C07] 把函数作为参数传入
来源：http://jsz.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dpr.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://qzp.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pvc.xinyue.icu

TS:   arr.map(String)
来源：http://nth.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nft.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dke.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://afe.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xtt.jinqigufen.top

[C08] 闭包
来源：http://mzk.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fbd.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kmq.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zyw.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bri.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ioq.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mmo.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aco.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dud.tanke756.top

[C09] 递归
来源：http://ywp.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vrt.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dus.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tzu.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zwl.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ogv.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mhq.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tbo.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nwe.nanxuanxn.top

[C10] 变量作用域
来源：http://mds.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qrq.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mlt.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xae.jyoumei.cn

TS:   同 JS
来源：http://wao.ydzc1.top

Java: 方法内为块级作用域
来源：http://wdj.wangdashe.top

Go:   花括号块级作用域
来源：http://etd.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uej.iojbl.cn

C#:   块级作用域
来源：http://zil.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://sev.xuetiantiany.cn

Py:   from module import func
来源：http://idi.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wme.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gsd.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wtl.xylfe.cn

Java: import java.util.List;
来源：http://olg.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bey.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://zoz.yuanzhike.top

C#:   using System.Text;
来源：http://ltd.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://bro.tarul.cn

Py:   (lambda: print("run"))()
来源：http://fte.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://vwz.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://zxk.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://brv.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kag.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://pkf.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://acv.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ziw.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://hsm.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mvb.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iev.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://abr.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdy.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://nod.hfpthk.cn

Go:   func add(a, b int) int
来源：http://ejj.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jzw.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nwb.aibaodan.cn

[C14] 泛型函数
来源：http://xol.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tyj.c1oappe.top

PHP:  // 无泛型
来源：http://fbx.yj20258.top

JS:   // 无泛型
来源：http://rwl.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jfr.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gpy.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://epy.hnqzz.top

Ruby: # 无泛型
来源：http://wvx.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ihv.yongpay.top

[C15] 解构 / 展开参数
来源：http://dzk.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hvt.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://qyc.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zpr.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dxw.nwbrower.top

Java: // 无解构
来源：http://vln.ybcxt.top

Go:   // 无解构
来源：http://zpb.vqdsnc.cn

Ruby: a, b = pair
来源：http://met.fktsv.cn

C#:   var (a, b) = pair;
来源：http://jvo.redwolf501.top

[C16] 函数 / 方法重载
来源：http://dcx.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rtc.quarkkingdee.top

PHP:  // 无重载
来源：http://gsc.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tjl.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://xzd.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fql.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://vnl.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://gtt.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sgh.jlsjyb.cn

================================================================================
来源：http://dvd.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://nfr.ybcxt.top

================================================================================
来源：http://npj.bbcook.cn

[D01] 创建数组 / 列表
来源：http://pzn.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gvi.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tak.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgr.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://woj.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sty.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://uns.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://evf.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hve.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://alw.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nwj.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lhe.jqgfzy.top

JS:   arr.push(4);
来源：http://fym.0kj1m.cn

TS:   arr.push(4);
来源：http://iaz.cheryme.top

Java: list.add(4);
来源：http://hov.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://qvy.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://jkp.iojbl.cn

C#:   list.Add(4);
来源：http://llw.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://qhx.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://xpb.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qvu.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mlo.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://liy.redwolf501.top

Java: list.add(0, 0);
来源：http://fxg.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://mht.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wqd.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://ros.cdnleiting.top

[D04] 删除元素
来源：http://xal.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://quw.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qtt.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pif.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://eya.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://obr.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cwg.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rsk.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mmu.nanxuanxn.top

[D05] 访问与修改元素
来源：http://hpq.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://doo.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://laf.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lpd.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://mtf.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://few.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://efz.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cuw.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://njp.redwolf501.top

[D06] 数组长度
来源：http://ebs.uphjek.com

Py:   len(arr)
来源：http://wnp.jinqigufen.top

PHP:  count($arr);
来源：http://dfw.chenjidiqi.icu

JS:   arr.length
来源：http://aby.ydzc1.top

TS:   arr.length
来源：http://uil.yueranfly.top

Java: list.size();
来源：http://mpf.zhiwuduotai.top

Go:   len(arr)
来源：http://kew.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://edp.shanyushiyangtech.top

C#:   list.Count;
来源：http://uzn.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://hby.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nac.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://fez.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://trv.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://atx.yj20258888.top

Java: list.subList(1, 4);
来源：http://rdx.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://ytt.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://gui.sweek.top

C#:   list.GetRange(1, 3);
来源：http://sbp.yueranfly.top

[D08] 合并两个数组
来源：http://pql.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://hxj.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://vvi.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jxw.zycfv.cn

TS:   [...a, ...b];
来源：http://rqv.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gwr.yvedp.cn

Go:   append(a, b...)
来源：http://bij.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://cdc.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://job.xinyue.icu

[D09] 排序（升序）
来源：http://wft.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://yxg.fengsongda.top

PHP:  sort($arr);
来源：http://une.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rsl.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fra.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rlx.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hwt.hnqzz.top

Ruby: arr.sort
来源：http://fwj.iojbl.cn

C#:   list.Sort();
来源：http://cjh.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ess.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rnb.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qym.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzw.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxw.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gwk.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxq.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://buo.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tak.yongpay.top

[D11] 反转数组
来源：http://yft.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://hqs.tanke756.top

PHP:  array_reverse($arr);
来源：http://vuy.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://amx.hywenlv.cn

TS:   [...arr].reverse();
来源：http://wzv.daria6918.cn

Java: Collections.reverse(list);
来源：http://sws.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://ccz.bbcook.cn

Ruby: arr.reverse
来源：http://jnw.ehwqpu.com

C#:   list.Reverse();
来源：http://oci.epnwcf.com

[D12] 查找元素下标
来源：http://pan.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://nrg.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fib.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kip.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwt.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ieb.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://bqd.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://yud.andypj.xyz

C#:   list.IndexOf(x);
来源：http://kva.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://ahe.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jlk.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://znb.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://dkv.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://bxf.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fup.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gws.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://lzv.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pfh.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://zuu.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pnp.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jnk.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://nch.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://fiy.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://scv.nanxinkj.top

Go:   // 手写循环
来源：http://zun.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dit.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ggv.sjlbkw.cn

[D15] 去重
来源：http://oxn.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xca.xylfe.cn

PHP:  array_unique($arr);
来源：http://ikl.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://cht.kuanghao11.cn


<!-- 参考信息 -->