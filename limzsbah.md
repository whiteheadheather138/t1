代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zrd.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dct.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uot.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eux.chenjidiqi.icu

[B13] 判断是否为数字
来源：http://mbu.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://hat.gogol.net.cn

PHP:  is_numeric($x)
来源：http://wec.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gts.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uba.yj20258.top

Java: x instanceof Number
来源：http://aqd.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uco.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://ozd.havefunace.top

C#:   x is int or double or decimal
来源：http://zgz.xylfe.cn

[B14] 判断值是否在集合内
来源：http://cwo.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dkf.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://byp.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://ahs.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://smw.fehbvm.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kof.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tyi.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kcb.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddu.0kj1m.cn

[B15] 布尔运算与取反
来源：http://kgu.cheryme.top

Py:   a and b or not c
来源：http://pdx.tian-w.cn

PHP:  $a && $b || !$c
来源：http://ojr.vqdsnc.cn

JS:   a && b || !c
来源：http://yfo.zhixingplan.top

TS:   a && b || !c
来源：http://aij.jianghu66.top

Java: a && b || !c
来源：http://cye.kuanghao11.cn

Go:   a && b || !c
来源：http://cyf.aibaodan.cn

Ruby: a && b || !c
来源：http://wfb.jlsjyb.cn

C#:   a && b || !c
来源：http://whe.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://htq.zhongyouzk.top

Py:   if not data: return
来源：http://ohs.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://csv.ehwqpu.com

JS:   if (!data) return;
来源：http://hro.tian-w.cn

TS:   if (!data) return;
来源：http://zhx.jqgfzy.top

Java: if (data == null) return;
来源：http://zuy.aizwys.cn

Go:   if data == nil { return }
来源：http://mop.fehbvm.com

Ruby: return if data.nil?
来源：http://dcc.bjfxy.top

C#:   if (data == null) return;
来源：http://rqv.c1oappe.top

================================================================================
来源：http://agz.gaohongyu789.top

C. 函数与作用域
来源：http://hvr.jinqigfzy.top

================================================================================
来源：http://zzs.gaohongyu789.top

[C01] 定义函数
来源：http://gmy.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://twu.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xfk.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://dnj.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cgb.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nkv.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ove.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://din.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pbr.jqgufenzy.top

[C02] 默认参数
来源：http://cxn.tanke756.top

Py:   def greet(name="World"): return name
来源：http://kfs.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cjx.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://fpc.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://epk.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yfj.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ihq.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://tmh.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://zyc.ydzc1.top

[C03] 可变参数
来源：http://tsg.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://lmb.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dts.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bjn.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xjl.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wru.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ids.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://etg.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lgr.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://flc.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kbb.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yuf.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fel.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ocw.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://bix.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://fnb.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://wkx.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://nny.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://ivk.daxiang520.top

Py:   return a, b
来源：http://mlh.zycfv.cn

PHP:  return [$a, $b];
来源：http://sio.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zef.andypj.xyz

TS:   return { a, b };
来源：http://brf.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oqh.yonumen.top

Go:   return a, b
来源：http://uwg.nwbrower.top

Ruby: return a, b
来源：http://vww.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://zst.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://iqq.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://mpb.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uih.haohaochexian.top

JS:   const square = x => x * x;
来源：http://tie.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://any.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hjo.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://dmy.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://ong.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://nfw.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://kuv.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oyx.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://lur.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wag.c1oappe.top

TS:   arr.map(String)
来源：http://rol.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://edq.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://asu.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://tnl.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wmt.yuanzhike.top

[C08] 闭包
来源：http://rdi.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vxd.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nnk.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://umd.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwj.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zfm.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nri.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oby.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jwf.chenjidiqi.icu

[C09] 递归
来源：http://pqb.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ixv.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oov.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzx.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwh.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jwv.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fcy.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uut.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qoc.sjlbkw.cn

[C10] 变量作用域
来源：http://yzw.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gte.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://koh.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rga.aibaodan.cn

TS:   同 JS
来源：http://ulv.chenlongwang.top

Java: 方法内为块级作用域
来源：http://yzj.chenlongwang.top

Go:   花括号块级作用域
来源：http://znz.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://itj.zycfv.cn

C#:   块级作用域
来源：http://qak.hcnkem.com

[C11] 模块导入与导出
来源：http://hwc.hnqzz.top

Py:   from module import func
来源：http://ehb.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vdt.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uwy.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fju.birdmap.top

Java: import java.util.List;
来源：http://zhm.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kgu.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://poq.nanxinkj.top

C#:   using System.Text;
来源：http://eih.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://ebp.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://bhf.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://vyr.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://xgx.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://czh.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxp.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://prl.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://zci.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://azk.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://pxt.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://txs.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hog.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hei.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://whp.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nbc.zhixingplan.top

Go:   func add(a, b int) int
来源：http://xzz.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wid.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qaf.kuanghao11.cn

[C14] 泛型函数
来源：http://loo.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fck.hesvh.cn

PHP:  // 无泛型
来源：http://bzr.cqqwz.cn

JS:   // 无泛型
来源：http://wgn.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wfp.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wqx.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uel.shzxlz.cn

Ruby: # 无泛型
来源：http://rgy.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yjf.yvedp.cn

[C15] 解构 / 展开参数
来源：http://nws.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmr.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://sjk.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://omr.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://chy.bbcook.cn

Java: // 无解构
来源：http://tqe.andypj.xyz

Go:   // 无解构
来源：http://yvn.hywenlv.cn

Ruby: a, b = pair
来源：http://pkd.sweek.top

C#:   var (a, b) = pair;
来源：http://adk.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://qkf.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qol.zdqjudy.top

PHP:  // 无重载
来源：http://sgu.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://fhs.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://bka.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hfp.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://kwh.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://mea.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vcy.gogol.net.cn

================================================================================
来源：http://qwj.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://bsd.jqgfzy.top

================================================================================
来源：http://haa.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://pgt.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tpx.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://beu.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ajk.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pnj.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kkm.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://fwf.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://emd.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jfd.cashguo.top

[D02] 追加元素到末尾
来源：http://vyn.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cyf.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yef.gogol.net.cn

JS:   arr.push(4);
来源：http://hxv.daxiang520.top

TS:   arr.push(4);
来源：http://env.zhoulong.xyz

Java: list.add(4);
来源：http://sha.uphjek.com

Go:   arr = append(arr, 4)
来源：http://lui.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://mgz.feifeiyinyue.top

C#:   list.Add(4);
来源：http://nnc.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://gxa.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://cfh.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gac.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aby.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://eur.ehwqpu.com

Java: list.add(0, 0);
来源：http://oaz.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://jfv.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qpr.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://liq.wangdashe.top

[D04] 删除元素
来源：http://xfs.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://stw.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dlx.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wdt.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://lyx.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hjm.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://foq.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xfy.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pqh.cashguo.top

[D05] 访问与修改元素
来源：http://qff.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xpa.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qxs.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bza.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://vtf.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://ujh.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://kak.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dwz.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ngd.vqdsnc.cn

[D06] 数组长度
来源：http://ecd.dashuyun.cn

Py:   len(arr)
来源：http://toi.havefunace.top

PHP:  count($arr);
来源：http://xzt.shanyushiyangtech.top

JS:   arr.length
来源：http://tyu.sweek.top

TS:   arr.length
来源：http://ync.shanyushiyangkeji.top

Java: list.size();
来源：http://hom.aibaodan.cn

Go:   len(arr)
来源：http://cbc.sweek.top

Ruby: arr.length; arr.size
来源：http://mke.hnxiangtu.top

C#:   list.Count;
来源：http://vny.fktsv.cn

[D07] 切片 / 取子数组
来源：http://pcr.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jib.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://dyn.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://rbv.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://rfw.hywenlv.cn

Java: list.subList(1, 4);
来源：http://jax.gaohongyu789.top

Go:   arr[1:4]
来源：http://gdl.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://xdm.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://hur.yj202588.top

[D08] 合并两个数组
来源：http://wix.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://lir.pycfn.com

PHP:  array_merge($a, $b);
来源：http://fpj.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lda.daria6918.cn

TS:   [...a, ...b];
来源：http://zxn.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pgu.andypj.xyz

Go:   append(a, b...)
来源：http://ieq.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://xbj.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://xtx.xylfe.cn

[D09] 排序（升序）
来源：http://qgv.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://wmb.xinyue.icu

PHP:  sort($arr);
来源：http://jrp.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bqj.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qft.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://voc.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zxj.pycfn.com

Ruby: arr.sort
来源：http://xcx.shzxlz.cn

C#:   list.Sort();
来源：http://hdu.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vlc.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qzs.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbz.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rkv.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgv.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aiv.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gdf.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gjh.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://joj.cucudq.cn

[D11] 反转数组
来源：http://jue.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xbk.ydzc1.top

PHP:  array_reverse($arr);
来源：http://ktr.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yof.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://vko.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://ocq.tarul.cn

Go:   slices.Reverse(arr)
来源：http://jgx.chenjidiqi.icu

Ruby: arr.reverse
来源：http://gxi.tarul.cn

C#:   list.Reverse();
来源：http://ylq.cashguo.top

[D12] 查找元素下标
来源：http://jkr.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://mlq.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rjo.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aea.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chq.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rob.316326.xyz

Go:   slices.Index(arr, x)
来源：http://ljv.epnwcf.com

Ruby: arr.index(x)
来源：http://oph.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://uhi.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://era.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hiy.fanxiaobao.xyz


<!-- 参考信息 -->