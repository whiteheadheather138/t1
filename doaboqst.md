代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ylm.jinqigufen.top

Java: x instanceof Number
来源：http://ldh.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycn.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://vfr.nwbrower.top

C#:   x is int or double or decimal
来源：http://mfl.fktsv.cn

[B14] 判断值是否在集合内
来源：http://zde.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://moh.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uzg.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://vue.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://xrt.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rnj.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gxp.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://fio.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zno.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://aqw.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://qza.tian-w.cn

PHP:  $a && $b || !$c
来源：http://bfm.hfpthk.cn

JS:   a && b || !c
来源：http://lqx.mhx1999.top

TS:   a && b || !c
来源：http://kcd.yonumen.top

Java: a && b || !c
来源：http://sax.tian-w.cn

Go:   a && b || !c
来源：http://mls.tianlin.xyz

Ruby: a && b || !c
来源：http://mdd.hnxiangtu.top

C#:   a && b || !c
来源：http://sgk.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://tbc.9152youxi.cn

Py:   if not data: return
来源：http://tgz.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://hno.jiagoushi.top

JS:   if (!data) return;
来源：http://gcq.birdmap.top

TS:   if (!data) return;
来源：http://nkz.hammf.cn

Java: if (data == null) return;
来源：http://qrs.smart0.xyz

Go:   if data == nil { return }
来源：http://rkm.hcnkem.com

Ruby: return if data.nil?
来源：http://bjq.hfpthk.cn

C#:   if (data == null) return;
来源：http://xir.mhx1999.top

================================================================================
来源：http://jgd.yfazqb.com

C. 函数与作用域
来源：http://nxe.tarul.cn

================================================================================
来源：http://fil.52xcode.cn

[C01] 定义函数
来源：http://jof.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://ffq.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkx.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://qmp.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukg.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ekt.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://mgx.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://tzv.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nss.pengpengdd.cyou

[C02] 默认参数
来源：http://suv.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://alb.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nlw.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://zkb.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zck.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qpt.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tlo.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://lbl.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://moe.guannengcc.top

[C03] 可变参数
来源：http://dus.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://ssr.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xbu.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jzs.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhm.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uib.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nom.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://lvy.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fty.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://yam.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mdz.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ntg.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eme.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://joh.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://rmy.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://naa.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://uzl.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://lee.havefunace.top

[C05] 返回多个值
来源：http://zdy.tarul.cn

Py:   return a, b
来源：http://adq.cashguo.top

PHP:  return [$a, $b];
来源：http://zto.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://glz.jianghu66.top

TS:   return { a, b };
来源：http://hhc.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hcc.aizwys.cn

Go:   return a, b
来源：http://npp.zhongyouzk.top

Ruby: return a, b
来源：http://knr.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://arj.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://dok.316326.xyz

Py:   square = lambda x: x * x
来源：http://owm.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nxa.cheryme.top

JS:   const square = x => x * x;
来源：http://pwe.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://nnr.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obe.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://txf.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://hcn.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://fit.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://bpx.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yma.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lmc.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jpb.epnwcf.com

TS:   arr.map(String)
来源：http://icc.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wgk.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hsq.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://xbg.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hcj.redwolf501.top

[C08] 闭包
来源：http://ecd.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rkf.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://soy.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fpa.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://luo.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bam.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fep.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jhp.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yal.zhiwuduotai.top

[C09] 递归
来源：http://dns.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://djn.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://axx.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lth.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bxd.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ivs.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nhu.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zuj.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gvf.hnqzz.top

[C10] 变量作用域
来源：http://gzo.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zje.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wyx.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tsg.jqgfzy.top

TS:   同 JS
来源：http://nys.haohaochexian.top

Java: 方法内为块级作用域
来源：http://zmv.meibo888.top

Go:   花括号块级作用域
来源：http://qao.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tcz.kuanghao11.cn

C#:   块级作用域
来源：http://yhj.snrcjt.cn

[C11] 模块导入与导出
来源：http://fmt.zhoulong.xyz

Py:   from module import func
来源：http://sbi.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rrt.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wng.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lrl.hesvh.cn

Java: import java.util.List;
来源：http://qnw.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dar.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://zwf.haohaochexian.top

C#:   using System.Text;
来源：http://nlc.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://jkn.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://gso.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://uin.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://sxi.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://xhg.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kdh.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://ihc.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://gwr.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bvi.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://vbv.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ytp.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebr.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ljv.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqy.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://czr.yuxming.cn

Go:   func add(a, b int) int
来源：http://pei.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syj.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hti.hfpthk.cn

[C14] 泛型函数
来源：http://lhf.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fwq.cdnleiting.top

PHP:  // 无泛型
来源：http://vlq.vqdsnc.cn

JS:   // 无泛型
来源：http://sbo.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvu.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ryg.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sfs.dashuyun.cn

Ruby: # 无泛型
来源：http://aoj.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://meb.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://yxk.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhg.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://obw.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nuy.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zor.ehwqpu.com

Java: // 无解构
来源：http://bsh.andypj.xyz

Go:   // 无解构
来源：http://ygr.yongpay.top

Ruby: a, b = pair
来源：http://xlh.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://rjn.hnqzz.top

[C16] 函数 / 方法重载
来源：http://knt.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dmk.tian-w.cn

PHP:  // 无重载
来源：http://qmh.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ynf.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ktx.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qud.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://fgd.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://iay.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://elt.c1oappe.top

================================================================================
来源：http://gqm.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://nrk.ybcxt.top

================================================================================
来源：http://jio.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://fgd.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ndz.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jhl.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kff.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://umx.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jhs.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://xdf.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://uim.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ajn.chenzaomai.com

[D02] 追加元素到末尾
来源：http://rve.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ikd.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aci.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://xaa.cucudq.cn

TS:   arr.push(4);
来源：http://gsg.xinyue.icu

Java: list.add(4);
来源：http://czx.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://oao.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://kad.316326.xyz

C#:   list.Add(4);
来源：http://jcv.redwolf501.top

[D03] 在指定位置插入元素
来源：http://byb.yj202588.top

Py:   arr.insert(0, 0)
来源：http://kwn.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pme.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qlm.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://nvo.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://ixy.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ytm.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eqn.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://tda.aizwys.cn

[D04] 删除元素
来源：http://its.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nxj.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aja.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ynq.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://whf.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xib.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://heh.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yfw.yangfankeji.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lfb.jinqigfzy.top

[D05] 访问与修改元素
来源：http://byx.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://muy.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lii.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mir.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://yxi.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://vii.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://pzs.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vyy.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sah.yvedp.cn

[D06] 数组长度
来源：http://rdw.zdqjudy.top

Py:   len(arr)
来源：http://ekh.jianghu66.top

PHP:  count($arr);
来源：http://oop.cqqwz.cn

JS:   arr.length
来源：http://kfc.yj20258888.top

TS:   arr.length
来源：http://pgk.meibo888.top

Java: list.size();
来源：http://kgl.shanyushiyangkeji.top

Go:   len(arr)
来源：http://vji.smart0.xyz

Ruby: arr.length; arr.size
来源：http://pvy.epnwcf.com

C#:   list.Count;
来源：http://fvq.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://ple.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://brf.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://wwb.cashguo.top

JS:   arr.slice(1, 4);
来源：http://lyb.cheryme.top

TS:   arr.slice(1, 4);
来源：http://kzb.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://dqx.jinqigfzy.top

Go:   arr[1:4]
来源：http://idk.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://bmd.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://ali.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://jvl.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://fdx.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://zfs.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dry.ivvv.top

TS:   [...a, ...b];
来源：http://knq.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wof.fengsongda.top

Go:   append(a, b...)
来源：http://hkq.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://hci.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://mjq.bjfxy.top

[D09] 排序（升序）
来源：http://gut.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://sfc.hesvh.cn

PHP:  sort($arr);
来源：http://mvs.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blk.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ruw.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lip.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://azq.zdbjq.cn

Ruby: arr.sort
来源：http://llc.hongshengwenyu.top

C#:   list.Sort();
来源：http://ygq.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bvh.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ove.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://isp.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://icd.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vre.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wmh.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qoe.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xqe.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yzx.nanxuanxn.top

[D11] 反转数组
来源：http://vqp.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://zdu.hesvh.cn

PHP:  array_reverse($arr);
来源：http://uhv.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tpi.yuxming.cn

TS:   [...arr].reverse();
来源：http://efu.sysykeji.top

Java: Collections.reverse(list);
来源：http://hss.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://vmq.tianlin.xyz

Ruby: arr.reverse
来源：http://ayt.tarul.cn

C#:   list.Reverse();
来源：http://koq.fehbvm.com

[D12] 查找元素下标
来源：http://xhm.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://mmd.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bkn.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hux.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fts.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wse.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://qlz.hnqzz.top

Ruby: arr.index(x)
来源：http://omu.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://tpq.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://amw.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://naw.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://frn.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://knj.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://kmg.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://usz.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jnf.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://zxb.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zlc.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://dfl.ivvv.top


<!-- 参考信息 -->