代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://okc.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hoe.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kdr.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bcs.bjfxy.top

[B13] 判断是否为数字
来源：http://uzz.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://rxb.cdnleiting.top

PHP:  is_numeric($x)
来源：http://jdb.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jub.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dae.zhiwuduotai.top

Java: x instanceof Number
来源：http://fod.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ytz.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://rxp.c1oappe.top

C#:   x is int or double or decimal
来源：http://jvv.andypj.xyz

[B14] 判断值是否在集合内
来源：http://aps.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uyb.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fbx.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://tum.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://vls.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://chp.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ymq.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ngg.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://imc.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://myr.316326.xyz

Py:   a and b or not c
来源：http://kfp.xylfe.cn

PHP:  $a && $b || !$c
来源：http://dnm.jinqigufen.top

JS:   a && b || !c
来源：http://paj.dashuyun.cn

TS:   a && b || !c
来源：http://uol.jinghuilouyu.cn

Java: a && b || !c
来源：http://nci.bbcook.cn

Go:   a && b || !c
来源：http://qdy.tian-w.cn

Ruby: a && b || !c
来源：http://kpi.mhx1999.top

C#:   a && b || !c
来源：http://erb.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://kas.sysykeji.top

Py:   if not data: return
来源：http://bmy.tanke756.top

PHP:  if (!$data) { return; }
来源：http://wbr.feifeiyinyue.top

JS:   if (!data) return;
来源：http://mzl.tianlin.xyz

TS:   if (!data) return;
来源：http://jku.yj20258.top

Java: if (data == null) return;
来源：http://ynl.sysykeji.top

Go:   if data == nil { return }
来源：http://pcg.daria6918.cn

Ruby: return if data.nil?
来源：http://vcg.daxiang520.top

C#:   if (data == null) return;
来源：http://lzr.pycfn.com

================================================================================
来源：http://rrt.zhiwuduotai.top

C. 函数与作用域
来源：http://mld.yongpay.top

================================================================================
来源：http://mjl.gotoacloud.top

[C01] 定义函数
来源：http://oga.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://vyd.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcx.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://pnw.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpq.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://veh.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vvf.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://ccs.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uaa.tian-w.cn

[C02] 默认参数
来源：http://ser.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://jjb.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bzx.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://udt.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ngi.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sma.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vts.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://rtr.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://qrj.316326.xyz

[C03] 可变参数
来源：http://bny.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://aum.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tri.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://scb.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://asy.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fgy.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cux.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://cgh.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nzb.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://nym.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dly.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uue.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vqx.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xbp.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://paz.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://eti.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://hqd.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://vqz.c1oappe.top

[C05] 返回多个值
来源：http://uze.52xcode.cn

Py:   return a, b
来源：http://gvb.sxryk.cn

PHP:  return [$a, $b];
来源：http://rmz.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dug.316326.xyz

TS:   return { a, b };
来源：http://ves.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wtl.gogol.net.cn

Go:   return a, b
来源：http://nfh.yfazqb.com

Ruby: return a, b
来源：http://xch.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://uri.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://pvo.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://hbw.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://boy.shzxlz.cn

JS:   const square = x => x * x;
来源：http://ved.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://kmc.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://frc.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://ura.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://qrj.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://gti.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://gtb.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jjz.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://egs.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://axc.svipenyu.cn

TS:   arr.map(String)
来源：http://uvv.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bri.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xfg.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://zrp.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vir.zdqjudy.top

[C08] 闭包
来源：http://skn.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bdz.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pyr.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eqy.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://feu.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ukz.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ojt.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ivk.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rir.zhongyouzk.top

[C09] 递归
来源：http://izs.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xpn.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iri.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://djf.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://laa.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://led.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iml.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zpb.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nff.sweek.top

[C10] 变量作用域
来源：http://ptd.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://igp.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yje.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iyu.zhijiandao.cn

TS:   同 JS
来源：http://wqu.iojbl.cn

Java: 方法内为块级作用域
来源：http://lrl.hywenlv.cn

Go:   花括号块级作用域
来源：http://gzy.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tzb.zdbjq.cn

C#:   块级作用域
来源：http://hsd.ppjwa.cn

[C11] 模块导入与导出
来源：http://amq.zhiwuduotai.top

Py:   from module import func
来源：http://bam.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ayz.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zes.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cnr.zhengqikj.top

Java: import java.util.List;
来源：http://hav.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yxt.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://nli.gogol.net.cn

C#:   using System.Text;
来源：http://lgj.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://qay.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://xnh.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://ksh.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://ddu.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://lzz.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aon.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://rro.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://npm.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://brj.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://oyy.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://whv.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grq.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xgq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uku.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xrb.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://tqd.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cll.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://jfb.kuanghao11.cn

[C14] 泛型函数
来源：http://kxd.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tsw.fehbvm.com

PHP:  // 无泛型
来源：http://xmx.bbcook.cn

JS:   // 无泛型
来源：http://yfj.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jlm.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tbt.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baw.ppjwa.cn

Ruby: # 无泛型
来源：http://zbj.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qay.redwolf501.top

[C15] 解构 / 展开参数
来源：http://bdr.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fug.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://hxb.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hbt.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pbi.kuanghao11.cn

Java: // 无解构
来源：http://hjm.xuetiantiany.cn

Go:   // 无解构
来源：http://yow.0kj1m.cn

Ruby: a, b = pair
来源：http://bot.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://bhv.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://eba.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ggc.zycfv.cn

PHP:  // 无重载
来源：http://adj.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vbn.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://urw.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jze.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://ftn.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://spe.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rog.gaohongyu789.top

================================================================================
来源：http://bhr.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://nqx.andypj.xyz

================================================================================
来源：http://hfv.daria6918.cn

[D01] 创建数组 / 列表
来源：http://lzh.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wyg.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rhb.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ljr.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wws.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nch.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://rku.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://jny.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vsr.ydzc1.top

[D02] 追加元素到末尾
来源：http://xob.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yrw.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xur.zhixingplan.top

JS:   arr.push(4);
来源：http://bxb.pycfn.com

TS:   arr.push(4);
来源：http://ccg.yuanzhike.top

Java: list.add(4);
来源：http://pxl.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://rxf.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://sai.ydzc1.top

C#:   list.Add(4);
来源：http://rxw.yongpay.top

[D03] 在指定位置插入元素
来源：http://nqq.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://xtf.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgr.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ifi.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://vjx.hywenlv.cn

Java: list.add(0, 0);
来源：http://djt.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zje.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rfi.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://uxi.svipenyu.cn

[D04] 删除元素
来源：http://pei.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ipl.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yxi.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyx.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://mch.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://opp.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vtq.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tdd.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vvf.mhx1999.top

[D05] 访问与修改元素
来源：http://eci.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wqu.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://flc.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iwv.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://ztx.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://kbp.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://dsi.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kjj.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ltb.hcnkem.com

[D06] 数组长度
来源：http://ywb.jyoumei.cn

Py:   len(arr)
来源：http://hsm.cqqwz.cn

PHP:  count($arr);
来源：http://waq.ehwqpu.com

JS:   arr.length
来源：http://oze.daxiang520.top

TS:   arr.length
来源：http://rzn.xingfuxueyuan.xyz

Java: list.size();
来源：http://ifj.shanyushiyangkeji.top

Go:   len(arr)
来源：http://bfc.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://ddj.mhx1999.top

C#:   list.Count;
来源：http://izs.fengsongda.top

[D07] 切片 / 取子数组
来源：http://duc.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://atj.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mlg.birdmap.top

JS:   arr.slice(1, 4);
来源：http://bji.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://tow.zhengqikj.top

Java: list.subList(1, 4);
来源：http://gjr.ctjpmb.com

Go:   arr[1:4]
来源：http://dsa.yuxming.cn

Ruby: arr[1, 3]
来源：http://tjk.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://elv.cdnleiting.top

[D08] 合并两个数组
来源：http://smt.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://ewq.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://ymw.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wzw.hysaishi.cn

TS:   [...a, ...b];
来源：http://mtt.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cll.hnqzz.top

Go:   append(a, b...)
来源：http://uaj.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://czp.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://upw.cdnleiting.top

[D09] 排序（升序）
来源：http://rui.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://cef.sjlbkw.cn

PHP:  sort($arr);
来源：http://kdo.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mjf.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ell.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ojp.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wlu.mhx1999.top

Ruby: arr.sort
来源：http://qqz.yonumen.top

C#:   list.Sort();
来源：http://bbo.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fpe.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zqv.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nku.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ubw.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://olu.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdj.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmh.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yrc.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hcb.hongshengwenyu.top

[D11] 反转数组
来源：http://yya.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://fjd.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://ztz.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yjk.fengsongda.top

TS:   [...arr].reverse();
来源：http://uxy.hywenlv.cn

Java: Collections.reverse(list);
来源：http://ria.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://dgn.hongshengwenyu.top

Ruby: arr.reverse
来源：http://gww.hywenlv.cn

C#:   list.Reverse();
来源：http://jtl.fehbvm.com

[D12] 查找元素下标
来源：http://kdt.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://dya.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://owd.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://asf.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xin.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsy.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://kth.xuanzx.com

Ruby: arr.index(x)
来源：http://hwv.epnwcf.com

C#:   list.IndexOf(x);
来源：http://bax.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://lpj.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rda.feifeiyinyue.top


<!-- 参考信息 -->