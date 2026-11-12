代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlo.yanxiufei.cn

Java: x instanceof Number
来源：http://vdy.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kfz.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://ugp.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://lrx.cashguo.top

[B14] 判断值是否在集合内
来源：http://ndz.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iqk.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://txp.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://etx.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://ret.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://moc.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hug.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lfx.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://izu.jiagoushi.top

[B15] 布尔运算与取反
来源：http://fcq.yangfankeji.com

Py:   a and b or not c
来源：http://iue.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://dgj.nwbrower.top

JS:   a && b || !c
来源：http://uux.uphjek.com

TS:   a && b || !c
来源：http://fdi.hnxiangtu.top

Java: a && b || !c
来源：http://aot.nanxinkj.top

Go:   a && b || !c
来源：http://uef.nanxuanxn.top

Ruby: a && b || !c
来源：http://ivm.ppjwa.cn

C#:   a && b || !c
来源：http://eif.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ijg.jqgufenzy.top

Py:   if not data: return
来源：http://kzg.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://gxd.tian-w.cn

JS:   if (!data) return;
来源：http://fwc.zycfv.cn

TS:   if (!data) return;
来源：http://ltv.hcnkem.com

Java: if (data == null) return;
来源：http://byw.hnxiangtu.top

Go:   if data == nil { return }
来源：http://zgn.zhixingplan.top

Ruby: return if data.nil?
来源：http://vbu.snrcjt.cn

C#:   if (data == null) return;
来源：http://gdk.fktsv.cn

================================================================================
来源：http://ego.cheryme.top

C. 函数与作用域
来源：http://shv.nanxuanxn.top

================================================================================
来源：http://dvl.yj202588.top

[C01] 定义函数
来源：http://ueo.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://ihp.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aaz.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://rja.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lab.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bot.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hfp.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://mkr.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jen.guannengcc.top

[C02] 默认参数
来源：http://avc.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://ink.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qdu.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://raw.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://imc.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdz.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dui.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://oaa.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://ykq.dianchejie.cn

[C03] 可变参数
来源：http://mrt.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://wws.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vnx.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vjr.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mtt.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ttr.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cok.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dbw.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://whh.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://ifi.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ubj.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xuq.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bol.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uot.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://dyb.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://xvb.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://rgd.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://lez.tarul.cn

[C05] 返回多个值
来源：http://lez.xuetiantiany.cn

Py:   return a, b
来源：http://ohv.hywenlv.cn

PHP:  return [$a, $b];
来源：http://exp.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hlq.zycfv.cn

TS:   return { a, b };
来源：http://bpr.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sse.jinqigufen.top

Go:   return a, b
来源：http://awe.chenzaomai.com

Ruby: return a, b
来源：http://bxc.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://fuw.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://uha.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://aiv.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bzc.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://ooc.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://slv.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mtx.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://erv.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://hgd.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://qyx.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://ggh.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcr.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://wxh.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qyn.pengpengdd.cyou

TS:   arr.map(String)
来源：http://ohb.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ojd.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nih.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://ccx.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eqz.nwbrower.top

[C08] 闭包
来源：http://zjn.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vhu.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vcv.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ioh.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nzl.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://piq.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vul.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mmn.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tca.meibo888.top

[C09] 递归
来源：http://jca.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fbs.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sjn.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nnb.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wtu.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gnn.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oer.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tcx.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lra.smart0.xyz

[C10] 变量作用域
来源：http://jqc.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zzk.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gqh.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mic.hesvh.cn

TS:   同 JS
来源：http://ooq.zhixingplan.top

Java: 方法内为块级作用域
来源：http://fhf.wangdashe.top

Go:   花括号块级作用域
来源：http://jcj.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ebb.redwolf501.top

C#:   块级作用域
来源：http://uoy.gaohongyu789.top

[C11] 模块导入与导出
来源：http://edv.ctjpmb.com

Py:   from module import func
来源：http://vce.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gjp.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://liz.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://glc.cheryme.top

Java: import java.util.List;
来源：http://hiw.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bex.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://clk.sysykeji.top

C#:   using System.Text;
来源：http://wuj.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://ier.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://qhy.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://feu.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://fcj.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://jbp.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjg.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://zuj.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://dai.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vxa.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://hgv.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xhv.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nrr.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iaz.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwq.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://uiq.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://xvp.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eyw.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://woi.yueranfly.top

[C14] 泛型函数
来源：http://ajl.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mfo.snrcjt.cn

PHP:  // 无泛型
来源：http://ric.cheryme.top

JS:   // 无泛型
来源：http://hsk.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yoe.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ruk.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxm.ppjwa.cn

Ruby: # 无泛型
来源：http://mxc.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ghr.yj20258.top

[C15] 解构 / 展开参数
来源：http://jav.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jim.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://srs.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgk.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://das.xylfe.cn

Java: // 无解构
来源：http://klk.hammf.cn

Go:   // 无解构
来源：http://yza.0kj1m.cn

Ruby: a, b = pair
来源：http://srs.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://xwj.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://lpg.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://msx.tianlin.xyz

PHP:  // 无重载
来源：http://dzu.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fcd.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://jep.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dsz.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://cjm.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://apq.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hcj.daxiang520.top

================================================================================
来源：http://tul.birdmap.top

D. 数组 / 列表 / 集合
来源：http://hrv.cashguo.top

================================================================================
来源：http://hlz.daria6918.cn

[D01] 创建数组 / 列表
来源：http://jmq.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cao.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ujv.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://amq.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ynp.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rcj.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://tsg.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://ndl.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ors.hfpthk.cn

[D02] 追加元素到末尾
来源：http://rhg.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pvv.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slb.guowangkeji.top

JS:   arr.push(4);
来源：http://gcf.ehwqpu.com

TS:   arr.push(4);
来源：http://sgu.cashguo.top

Java: list.add(4);
来源：http://dxd.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://ega.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://wsg.guowangkeji.top

C#:   list.Add(4);
来源：http://mij.cucudq.cn

[D03] 在指定位置插入元素
来源：http://jyw.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://hqb.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hqp.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lhx.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://kgj.ctjpmb.com

Java: list.add(0, 0);
来源：http://hfv.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nki.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fmv.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://pvt.hongshengwenyu.top

[D04] 删除元素
来源：http://vul.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kze.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iqu.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bzt.hammf.cn

TS:   arr.splice(0, 1);
来源：http://rtf.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fbi.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zua.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://whx.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lox.nwbrower.top

[D05] 访问与修改元素
来源：http://ash.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lir.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://asl.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kwq.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://ctm.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://qji.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://ijj.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://okb.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lzs.ppjwa.cn

[D06] 数组长度
来源：http://sfv.uphjek.com

Py:   len(arr)
来源：http://fdo.chenzaomai.com

PHP:  count($arr);
来源：http://mfs.zhengqikj.top

JS:   arr.length
来源：http://qhl.ppjwa.cn

TS:   arr.length
来源：http://isp.sjlbkw.cn

Java: list.size();
来源：http://ihv.yj202588.top

Go:   len(arr)
来源：http://ijs.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://svv.meibo888.top

C#:   list.Count;
来源：http://rpe.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://idu.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lsp.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bxt.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://tuf.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://gkt.ehwqpu.com

Java: list.subList(1, 4);
来源：http://yci.cucudq.cn

Go:   arr[1:4]
来源：http://ijd.zhengqikj.top

Ruby: arr[1, 3]
来源：http://xxq.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://zlu.jinqigufen.top

[D08] 合并两个数组
来源：http://vit.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://pjp.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://ljs.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sqa.daria6918.cn

TS:   [...a, ...b];
来源：http://snd.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qbr.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://ipj.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://xnn.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://oyq.zdbjq.cn

[D09] 排序（升序）
来源：http://ojd.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://fqh.dashuyun.cn

PHP:  sort($arr);
来源：http://dzd.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ixu.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eji.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gmz.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yva.fanxiaobao.xyz

Ruby: arr.sort
来源：http://rxq.pengpengdd.cyou

C#:   list.Sort();
来源：http://zmt.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://amv.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zyy.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://omd.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zss.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://brd.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ann.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tfh.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cmm.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hyy.smart0.xyz

[D11] 反转数组
来源：http://iqs.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://gzo.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://uqt.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://prl.cashguo.top

TS:   [...arr].reverse();
来源：http://ija.svipenyu.cn

Java: Collections.reverse(list);
来源：http://tar.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://dnv.ehwqpu.com

Ruby: arr.reverse
来源：http://ais.chenjidiqi.icu

C#:   list.Reverse();
来源：http://nbt.chenlongwang.top

[D12] 查找元素下标
来源：http://scf.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://ecb.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qyz.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pep.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xqp.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://huw.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://cii.xziqi.cn

Ruby: arr.index(x)
来源：http://dwt.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://tkk.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://fma.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hqw.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kqj.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://bcy.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://oiv.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wdp.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nvc.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://ovk.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ngt.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://pqd.dashuyun.cn


<!-- 参考信息 -->