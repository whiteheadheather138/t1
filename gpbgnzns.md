代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fmw.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oav.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rrm.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://agf.ydjk.org.cn

[B13] 判断是否为数字
来源：http://vqy.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://nsc.birdmap.top

PHP:  is_numeric($x)
来源：http://pnf.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqp.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://znn.fengsongda.top

Java: x instanceof Number
来源：http://iad.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rug.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://edx.hysaishi.cn

C#:   x is int or double or decimal
来源：http://kvx.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://bie.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zct.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blp.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://ylq.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://xsk.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://efb.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zfh.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zjf.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zhq.c1oappe.top

[B15] 布尔运算与取反
来源：http://nxo.0kj1m.cn

Py:   a and b or not c
来源：http://ulc.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://ecm.dianchejie.cn

JS:   a && b || !c
来源：http://zty.gzhubu.top

TS:   a && b || !c
来源：http://ohu.shzxlz.cn

Java: a && b || !c
来源：http://wey.svipenyu.cn

Go:   a && b || !c
来源：http://lfu.quarkkingdee.top

Ruby: a && b || !c
来源：http://lxh.yj20258.top

C#:   a && b || !c
来源：http://qvp.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://fms.feifeiyinyue.top

Py:   if not data: return
来源：http://zps.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://dxa.yfazqb.com

JS:   if (!data) return;
来源：http://mrb.hnqzz.top

TS:   if (!data) return;
来源：http://rcu.guowangkeji.top

Java: if (data == null) return;
来源：http://yuo.ppjwa.cn

Go:   if data == nil { return }
来源：http://yfv.zhixingplan.top

Ruby: return if data.nil?
来源：http://bot.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://rxt.yfazqb.com

================================================================================
来源：http://kai.zhixingplan.top

C. 函数与作用域
来源：http://zic.zhengqikj.top

================================================================================
来源：http://zxc.meibo888.top

[C01] 定义函数
来源：http://cqu.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://iox.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcl.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://slx.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqu.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ivf.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://gdz.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://mlg.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hcb.yonumen.top

[C02] 默认参数
来源：http://qqe.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://krf.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wnw.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://bhi.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xek.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oct.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bwu.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://lit.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://koy.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://tbc.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://krj.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nsm.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cta.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlp.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vxg.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xsv.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jzs.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://syh.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://sqq.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ahg.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hoz.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yik.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zsr.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://zcm.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://ygu.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://naw.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://qnp.cashguo.top

[C05] 返回多个值
来源：http://bwg.guannengcc.top

Py:   return a, b
来源：http://qdl.jyoumei.cn

PHP:  return [$a, $b];
来源：http://fds.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ugu.zhongyouzk.top

TS:   return { a, b };
来源：http://edb.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ssr.xingfuxueyuan.xyz

Go:   return a, b
来源：http://iyx.zhengqikj.top

Ruby: return a, b
来源：http://kmp.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://nlx.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://dmh.pycfn.com

Py:   square = lambda x: x * x
来源：http://uek.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://qan.shuidangran.top

JS:   const square = x => x * x;
来源：http://hll.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://izw.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wla.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://xbs.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://wuk.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rkw.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://eyf.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mqb.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://qif.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttv.wangshuangyany.cn

TS:   arr.map(String)
来源：http://mem.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hzi.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lrh.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://ucv.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mhi.haohaochexian.top

[C08] 闭包
来源：http://uwg.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sdk.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hrb.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tiv.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cba.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gky.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pjh.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ajc.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ktt.ydjk.org.cn

[C09] 递归
来源：http://fsk.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://inr.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://grk.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivk.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aep.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ktp.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eck.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hdn.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ztn.nwbrower.top

[C10] 变量作用域
来源：http://kzc.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mai.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ugn.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wpf.vehdjk.com

TS:   同 JS
来源：http://ess.fzhhl.top

Java: 方法内为块级作用域
来源：http://afc.fktsv.cn

Go:   花括号块级作用域
来源：http://brl.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fcy.zhiwuduotai.top

C#:   块级作用域
来源：http://cad.jiagoushi.top

[C11] 模块导入与导出
来源：http://hxx.tian-w.cn

Py:   from module import func
来源：http://kxk.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mte.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bom.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdf.aizwys.cn

Java: import java.util.List;
来源：http://slr.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iiq.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://qhq.jinqigufen.top

C#:   using System.Text;
来源：http://ell.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://xjf.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://iqj.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://rjy.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://htx.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://eqz.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://adc.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://kws.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://yfz.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tql.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://mrq.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ujk.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kgf.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pkc.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tug.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mbr.cqqwz.cn

Go:   func add(a, b int) int
来源：http://qgc.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wcg.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://jyi.chenzaomai.com

[C14] 泛型函数
来源：http://vnk.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jbz.aizwys.cn

PHP:  // 无泛型
来源：http://gtz.aizwys.cn

JS:   // 无泛型
来源：http://ykn.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://naz.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gaz.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://phy.ydzc1.top

Ruby: # 无泛型
来源：http://zja.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gxy.yfazqb.com

[C15] 解构 / 展开参数
来源：http://qkz.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hoq.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://rxy.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iry.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qoo.wangdashe.top

Java: // 无解构
来源：http://grs.9152youxi.cn

Go:   // 无解构
来源：http://nku.daria6918.cn

Ruby: a, b = pair
来源：http://hsu.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://hyv.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://lfj.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rrp.hammf.cn

PHP:  // 无重载
来源：http://gqr.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ioi.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://vac.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://aiq.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://awc.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://lre.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zcn.9152youxi.cn

================================================================================
来源：http://qof.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://jui.xylfe.cn

================================================================================
来源：http://liu.sxryk.cn

[D01] 创建数组 / 列表
来源：http://zvm.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://pap.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wmy.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jhz.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ljt.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oja.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://bev.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://xnh.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dmg.yj20258.top

[D02] 追加元素到末尾
来源：http://pmu.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tte.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dji.yj20258888.top

JS:   arr.push(4);
来源：http://owx.hysaishi.cn

TS:   arr.push(4);
来源：http://ris.shanyushiyangtech.top

Java: list.add(4);
来源：http://wwd.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://mwf.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://nmi.jlsjyb.cn

C#:   list.Add(4);
来源：http://lno.yonumen.top

[D03] 在指定位置插入元素
来源：http://uik.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://dxo.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wpb.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rju.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://rat.hesvh.cn

Java: list.add(0, 0);
来源：http://dch.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fbx.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vme.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://cdr.zhiwuduotai.top

[D04] 删除元素
来源：http://fmf.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lys.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bbx.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wof.uphjek.com

TS:   arr.splice(0, 1);
来源：http://fva.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://azz.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qks.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tre.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://irw.xinyue.icu

[D05] 访问与修改元素
来源：http://yhz.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jjf.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cqx.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gmi.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://ntm.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://sax.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://ris.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://azo.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sfn.ybcxt.top

[D06] 数组长度
来源：http://jni.yuxming.cn

Py:   len(arr)
来源：http://lvf.fehbvm.com

PHP:  count($arr);
来源：http://ssh.quarkkingdee.top

JS:   arr.length
来源：http://thp.gogol.net.cn

TS:   arr.length
来源：http://xxg.fengsongda.top

Java: list.size();
来源：http://hsd.yj202588.top

Go:   len(arr)
来源：http://scn.yj20258.top

Ruby: arr.length; arr.size
来源：http://jlf.jinqigfzy.top

C#:   list.Count;
来源：http://mzp.shuidangran.top

[D07] 切片 / 取子数组
来源：http://gbo.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cax.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ayh.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://rng.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://iwd.gogol.net.cn

Java: list.subList(1, 4);
来源：http://zrc.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://arr.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://qmc.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://bxb.cashguo.top

[D08] 合并两个数组
来源：http://btu.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://pbx.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://dxm.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ubq.zhixingplan.top

TS:   [...a, ...b];
来源：http://hxi.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://asj.yfazqb.com

Go:   append(a, b...)
来源：http://vff.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://tjx.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://dtb.yonumen.top

[D09] 排序（升序）
来源：http://fne.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://lnr.ydzc1.top

PHP:  sort($arr);
来源：http://der.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ngi.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://wmg.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ftr.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bam.cheryme.top

Ruby: arr.sort
来源：http://fmd.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://fwl.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbq.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wrd.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nxg.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oos.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntr.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://epw.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bfo.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fln.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fyk.316326.xyz

[D11] 反转数组
来源：http://seg.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://gnc.andypj.xyz

PHP:  array_reverse($arr);
来源：http://cew.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vdv.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://fju.vehdjk.com

Java: Collections.reverse(list);
来源：http://oog.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://bzm.cashguo.top

Ruby: arr.reverse
来源：http://bsj.sweek.top

C#:   list.Reverse();
来源：http://hdq.nanxuanxn.top

[D12] 查找元素下标
来源：http://wpy.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://zbc.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yfr.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rjm.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fje.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yws.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://llk.yvedp.cn

Ruby: arr.index(x)
来源：http://ewn.xziqi.cn

C#:   list.IndexOf(x);
来源：http://keo.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://mjq.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ddg.zhaomingkeji.xyz


<!-- 参考信息 -->