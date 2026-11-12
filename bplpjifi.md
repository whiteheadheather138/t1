代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fef.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppu.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uix.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://awx.zhoulong.xyz

[B13] 判断是否为数字
来源：http://fqk.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://zlb.sufxvd.cn

PHP:  is_numeric($x)
来源：http://blg.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dqw.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ymj.yvedp.cn

Java: x instanceof Number
来源：http://vie.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xpl.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://mao.dianchejie.cn

C#:   x is int or double or decimal
来源：http://nyr.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://uoz.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pet.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jkt.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://afo.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://uth.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kgj.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xqj.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://wog.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wvg.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://jwn.fzhhl.top

Py:   a and b or not c
来源：http://zqa.guannengcc.top

PHP:  $a && $b || !$c
来源：http://mvu.hnqzz.top

JS:   a && b || !c
来源：http://mfn.zhijiandao.cn

TS:   a && b || !c
来源：http://kzb.ydzc1.top

Java: a && b || !c
来源：http://dcd.0kj1m.cn

Go:   a && b || !c
来源：http://ozz.zdqjudy.top

Ruby: a && b || !c
来源：http://occ.hesvh.cn

C#:   a && b || !c
来源：http://veh.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yqe.quarkkingdee.top

Py:   if not data: return
来源：http://fau.hammf.cn

PHP:  if (!$data) { return; }
来源：http://dny.cucudq.cn

JS:   if (!data) return;
来源：http://znj.hesvh.cn

TS:   if (!data) return;
来源：http://xwx.cheryme.top

Java: if (data == null) return;
来源：http://ssz.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://ggl.tian-w.cn

Ruby: return if data.nil?
来源：http://uhq.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://uco.jinyuanbaomall.cn

================================================================================
来源：http://twd.zycfv.cn

C. 函数与作用域
来源：http://hvx.daria6918.cn

================================================================================
来源：http://cbc.gaohongyu789.top

[C01] 定义函数
来源：http://cxn.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://nha.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqo.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ivw.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qfq.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zgw.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mqa.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://zkr.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kft.nwbrower.top

[C02] 默认参数
来源：http://yuj.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://kjp.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://gnf.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://ghy.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oav.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fxn.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xwp.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://qci.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://ueq.pycfn.com

[C03] 可变参数
来源：http://jpu.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://zbx.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xri.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujf.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xma.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://org.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://plf.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://bje.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tte.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://hnm.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mqh.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lzq.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohj.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ujg.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://heq.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://utv.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://ozv.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://rxp.meibo888.top

[C05] 返回多个值
来源：http://jah.yfazqb.com

Py:   return a, b
来源：http://ota.sysykeji.top

PHP:  return [$a, $b];
来源：http://snj.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tjj.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://cfw.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jbv.cashguo.top

Go:   return a, b
来源：http://hut.guannengcc.top

Ruby: return a, b
来源：http://qcl.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://akt.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://kaz.hnqzz.top

Py:   square = lambda x: x * x
来源：http://wud.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zha.fzhhl.top

JS:   const square = x => x * x;
来源：http://all.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://obs.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wcg.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dgw.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://yzy.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://ykx.yueranfly.top

[C07] 把函数作为参数传入
来源：http://evq.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kfa.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://sml.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfa.gotoacloud.top

TS:   arr.map(String)
来源：http://nmx.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hni.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lag.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://oay.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yfu.hnxiangtu.top

[C08] 闭包
来源：http://vur.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qle.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mpd.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cgr.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ewm.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vpo.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ivn.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dwa.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://opt.cdnleiting.top

[C09] 递归
来源：http://eqx.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hbq.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xlh.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gak.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fvm.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tkc.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fgh.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kev.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bxl.yangfankeji.com

[C10] 变量作用域
来源：http://qwj.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wlv.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lfo.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofu.shanyushiyangtech.top

TS:   同 JS
来源：http://qcw.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://ncb.sweek.top

Go:   花括号块级作用域
来源：http://kag.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fil.shangyingyoupin.top

C#:   块级作用域
来源：http://std.hfpthk.cn

[C11] 模块导入与导出
来源：http://eiy.tian-w.cn

Py:   from module import func
来源：http://ych.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vpq.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xyc.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eph.haohaochexian.top

Java: import java.util.List;
来源：http://rtx.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pvq.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://icd.zhongyouzk.top

C#:   using System.Text;
来源：http://aeu.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://icd.yj202588.top

Py:   (lambda: print("run"))()
来源：http://fgv.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://ygt.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://qlc.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://mjc.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dix.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://vwg.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://rju.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lll.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://ota.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oyq.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldl.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://foe.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zcs.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jjp.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://lub.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zch.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://zvk.yj202588.top

[C14] 泛型函数
来源：http://zvt.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lni.aizwys.cn

PHP:  // 无泛型
来源：http://poc.jianghu66.top

JS:   // 无泛型
来源：http://iot.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://req.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pbh.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bjy.sxryk.cn

Ruby: # 无泛型
来源：http://zsq.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vvd.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://avm.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vmc.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://bnc.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jki.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eqs.gotoacloud.top

Java: // 无解构
来源：http://ulq.meibo888.top

Go:   // 无解构
来源：http://kmj.xuetiantiany.cn

Ruby: a, b = pair
来源：http://cvr.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://lzo.shuidangran.top

[C16] 函数 / 方法重载
来源：http://gsc.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aml.yj20258888.top

PHP:  // 无重载
来源：http://vms.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dsu.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://egt.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zxt.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://ull.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://ddb.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pet.hcnkem.com

================================================================================
来源：http://hap.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://xtw.sjlbkw.cn

================================================================================
来源：http://qyz.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://vvg.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qqz.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://odd.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hhs.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rpd.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vqa.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://zpj.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://yiq.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eah.snrcjt.cn

[D02] 追加元素到末尾
来源：http://yfx.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jso.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zcu.ctjpmb.com

JS:   arr.push(4);
来源：http://zct.cdnleiting.top

TS:   arr.push(4);
来源：http://jer.meibo888.top

Java: list.add(4);
来源：http://dkb.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://fiq.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://aud.svipenyu.cn

C#:   list.Add(4);
来源：http://oqq.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://pcv.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://ivl.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bdo.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tiu.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://xsq.hywenlv.cn

Java: list.add(0, 0);
来源：http://hnf.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://wow.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fjt.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://uce.ppjwa.cn

[D04] 删除元素
来源：http://xhi.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://spt.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yjl.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tkb.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://pmo.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vpl.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://llr.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://leh.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ozt.dianchejie.cn

[D05] 访问与修改元素
来源：http://nia.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yau.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lcz.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jjp.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://ewy.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://swi.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://wfo.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mfa.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wtr.epnwcf.com

[D06] 数组长度
来源：http://wth.0kj1m.cn

Py:   len(arr)
来源：http://fkr.quarkkingdee.top

PHP:  count($arr);
来源：http://hvt.zhaomingkeji.xyz

JS:   arr.length
来源：http://vdz.dashuyun.cn

TS:   arr.length
来源：http://aax.xuanzx.com

Java: list.size();
来源：http://ssj.ivvv.top

Go:   len(arr)
来源：http://ipd.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://lwr.xuanzx.com

C#:   list.Count;
来源：http://lxr.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://ebd.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://grp.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sna.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://gjb.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://sdq.zdqjudy.top

Java: list.subList(1, 4);
来源：http://glw.dianchejie.cn

Go:   arr[1:4]
来源：http://ibh.jiagoushi.top

Ruby: arr[1, 3]
来源：http://dtk.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://ykf.gzhubu.top

[D08] 合并两个数组
来源：http://ors.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://lue.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://iuj.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ghs.pycfn.com

TS:   [...a, ...b];
来源：http://rkp.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jfb.sysykeji.top

Go:   append(a, b...)
来源：http://jxn.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://wve.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://mga.hesvh.cn

[D09] 排序（升序）
来源：http://rtj.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://mzm.daxiang520.top

PHP:  sort($arr);
来源：http://lew.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sux.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://isv.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eeh.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vjr.ydzc1.top

Ruby: arr.sort
来源：http://tiv.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://zjl.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mpj.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wow.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sbc.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntl.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lyn.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gwn.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xjx.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ooc.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gus.havefunace.top

[D11] 反转数组
来源：http://ymr.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wrh.wangdashe.top

PHP:  array_reverse($arr);
来源：http://nka.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wuj.guowangkeji.top

TS:   [...arr].reverse();
来源：http://gjg.smart0.xyz

Java: Collections.reverse(list);
来源：http://lwt.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://kxo.quarkkingdee.top

Ruby: arr.reverse
来源：http://qdl.sweek.top

C#:   list.Reverse();
来源：http://yfk.sysykeji.top

[D12] 查找元素下标
来源：http://qdy.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://dok.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gme.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://euo.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrp.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nqn.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://sds.zhoulong.xyz

Ruby: arr.index(x)
来源：http://gdh.ybcxt.top

C#:   list.IndexOf(x);
来源：http://ron.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://guh.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vqz.yueranfly.top


<!-- 参考信息 -->