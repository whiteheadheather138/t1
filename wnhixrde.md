代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fqp.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://boe.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ndn.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ynj.yonumen.top

[B13] 判断是否为数字
来源：http://fmp.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://hkm.jqgfzy.top

PHP:  is_numeric($x)
来源：http://zpk.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mcg.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zoa.cdnleiting.top

Java: x instanceof Number
来源：http://zbv.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mha.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://ygs.c1oappe.top

C#:   x is int or double or decimal
来源：http://dbn.sweek.top

[B14] 判断值是否在集合内
来源：http://mjt.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://icv.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://odf.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://sqx.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://jbl.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://uwl.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rcq.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://tmy.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jxp.sufxvd.cn

[B15] 布尔运算与取反
来源：http://jtb.pycfn.com

Py:   a and b or not c
来源：http://npq.c1oappe.top

PHP:  $a && $b || !$c
来源：http://jdl.jlsjyb.cn

JS:   a && b || !c
来源：http://xxe.yanxiufei.cn

TS:   a && b || !c
来源：http://nnl.shanyushiyangtech.top

Java: a && b || !c
来源：http://rxu.yonumen.top

Go:   a && b || !c
来源：http://utb.pycfn.com

Ruby: a && b || !c
来源：http://wmm.aizwys.cn

C#:   a && b || !c
来源：http://fgn.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kgp.ehwqpu.com

Py:   if not data: return
来源：http://spq.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://quq.feifeiyinyue.top

JS:   if (!data) return;
来源：http://wle.aibaodan.cn

TS:   if (!data) return;
来源：http://atn.havefunace.top

Java: if (data == null) return;
来源：http://cqx.cqqwz.cn

Go:   if data == nil { return }
来源：http://ren.yfazqb.com

Ruby: return if data.nil?
来源：http://inv.zdbjq.cn

C#:   if (data == null) return;
来源：http://fuw.sxryk.cn

================================================================================
来源：http://bcx.wangshuangyany.cn

C. 函数与作用域
来源：http://jnu.jinyuanbaomall.cn

================================================================================
来源：http://ajt.aibaodan.cn

[C01] 定义函数
来源：http://uyw.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://lci.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wte.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://amk.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djc.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yxn.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://iqz.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://gxi.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://duy.cashguo.top

[C02] 默认参数
来源：http://sri.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://kxi.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qoj.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://zww.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hls.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://thq.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sjo.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://cne.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://xkl.zhengqikj.top

[C03] 可变参数
来源：http://ejj.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://chw.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vzk.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vks.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgr.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xrx.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wrg.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://kky.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fio.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://qxl.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uvb.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ddw.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://teo.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wrr.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://fjk.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://nvk.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://fvv.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://mda.gogol.net.cn

[C05] 返回多个值
来源：http://jik.jqgufenzy.top

Py:   return a, b
来源：http://yvp.yonumen.top

PHP:  return [$a, $b];
来源：http://egy.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://bbi.pycfn.com

TS:   return { a, b };
来源：http://koy.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jzt.aizwys.cn

Go:   return a, b
来源：http://mhy.gogol.net.cn

Ruby: return a, b
来源：http://ocm.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://usj.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://zyd.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://koy.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jsa.tian-w.cn

JS:   const square = x => x * x;
来源：http://wmu.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://fcn.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://psa.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://oje.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://abf.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://smr.yuxming.cn

[C07] 把函数作为参数传入
来源：http://kob.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tzc.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://orv.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oop.xuanzx.com

TS:   arr.map(String)
来源：http://wgp.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ofu.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gsn.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://xjf.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dfh.ybcxt.top

[C08] 闭包
来源：http://ybi.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dej.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ees.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cvd.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qdf.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rue.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://okp.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xjk.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ygp.zdbjq.cn

[C09] 递归
来源：http://fqf.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cdp.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qyb.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttv.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bre.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vsr.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ieb.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://haq.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eva.cdnleiting.top

[C10] 变量作用域
来源：http://cmk.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zgt.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mzc.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wop.xuanzx.com

TS:   同 JS
来源：http://qwx.mhx1999.top

Java: 方法内为块级作用域
来源：http://sjg.52xcode.cn

Go:   花括号块级作用域
来源：http://xpi.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ehj.fzhhl.top

C#:   块级作用域
来源：http://znr.gotoacloud.top

[C11] 模块导入与导出
来源：http://heo.chenzaomai.com

Py:   from module import func
来源：http://gfn.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ahb.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rbs.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://elo.cashguo.top

Java: import java.util.List;
来源：http://lmu.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nlw.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://pzl.guannengcc.top

C#:   using System.Text;
来源：http://xrg.sweek.top

[C12] 立即执行函数 IIFE
来源：http://qpl.meibo888.top

Py:   (lambda: print("run"))()
来源：http://xql.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://nbz.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://oee.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://fuo.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kaz.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://fef.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://qiq.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dzr.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://gxz.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abx.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pws.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gpz.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://auh.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mza.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://iuv.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xpb.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://pds.fengsongda.top

[C14] 泛型函数
来源：http://dda.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ojj.epnwcf.com

PHP:  // 无泛型
来源：http://cvl.52xcode.cn

JS:   // 无泛型
来源：http://nfe.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xoz.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vys.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iao.pycfn.com

Ruby: # 无泛型
来源：http://kbd.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tce.yfazqb.com

[C15] 解构 / 展开参数
来源：http://aqu.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hwm.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://lms.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gyp.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uzb.meibo888.top

Java: // 无解构
来源：http://xxj.kuanghao11.cn

Go:   // 无解构
来源：http://eta.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://bhb.andypj.xyz

C#:   var (a, b) = pair;
来源：http://jjk.xinyue.icu

[C16] 函数 / 方法重载
来源：http://iar.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bvw.52xcode.cn

PHP:  // 无重载
来源：http://njq.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ein.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://iie.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yei.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://qwr.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://zgt.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gve.fehbvm.com

================================================================================
来源：http://npv.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://tuw.shanyushiyangtech.top

================================================================================
来源：http://sia.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://cdy.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovw.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kgo.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wna.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://azw.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hks.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://gkq.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://nwr.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pzr.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://hsj.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bor.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://spz.quarkkingdee.top

JS:   arr.push(4);
来源：http://mix.cqqwz.cn

TS:   arr.push(4);
来源：http://hgb.ppjwa.cn

Java: list.add(4);
来源：http://psi.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://ksk.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://hbg.wangdashe.top

C#:   list.Add(4);
来源：http://rbn.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://mwc.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://lkk.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bno.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://svk.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://gwx.redwolf501.top

Java: list.add(0, 0);
来源：http://pbu.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://epj.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://edj.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://wcl.yj20258888.top

[D04] 删除元素
来源：http://zmi.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tsf.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://awv.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nmq.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://mai.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tad.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://unj.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gpo.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vwr.zhoulong.xyz

[D05] 访问与修改元素
来源：http://rcn.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iqk.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bya.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kxq.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://hxg.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://edc.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://axt.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zwa.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wib.redwolf501.top

[D06] 数组长度
来源：http://rsg.yuanzhike.top

Py:   len(arr)
来源：http://vtr.tianlin.xyz

PHP:  count($arr);
来源：http://zun.aizwys.cn

JS:   arr.length
来源：http://wrz.vehdjk.com

TS:   arr.length
来源：http://rsj.ydjk.org.cn

Java: list.size();
来源：http://fcg.dashuyun.cn

Go:   len(arr)
来源：http://jet.316326.xyz

Ruby: arr.length; arr.size
来源：http://pkh.bjfxy.top

C#:   list.Count;
来源：http://rxt.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://aun.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bzz.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://axa.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://urr.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://wls.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://tcl.daxiang520.top

Go:   arr[1:4]
来源：http://knv.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://rpv.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://zju.bjfxy.top

[D08] 合并两个数组
来源：http://cpi.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://dzm.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://tiy.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://azh.tarul.cn

TS:   [...a, ...b];
来源：http://lul.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tna.sweek.top

Go:   append(a, b...)
来源：http://mun.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://arw.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://fjm.0kj1m.cn

[D09] 排序（升序）
来源：http://dza.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://clv.hywenlv.cn

PHP:  sort($arr);
来源：http://anq.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vzy.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mbb.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fkl.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mey.ydzc1.top

Ruby: arr.sort
来源：http://bvy.cqqwz.cn

C#:   list.Sort();
来源：http://alx.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://rfi.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://roc.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygr.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uxa.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jos.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tqk.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://adb.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wqy.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qfc.ywan-chungtsiang.top

[D11] 反转数组
来源：http://gmy.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://rhy.hammf.cn

PHP:  array_reverse($arr);
来源：http://ran.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lbo.yangfankeji.com

TS:   [...arr].reverse();
来源：http://fob.hywenlv.cn

Java: Collections.reverse(list);
来源：http://qxp.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://kjk.aibaodan.cn

Ruby: arr.reverse
来源：http://jde.guowangkeji.top

C#:   list.Reverse();
来源：http://hjc.jqgufenzy.top

[D12] 查找元素下标
来源：http://enn.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://uzn.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jaz.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://moq.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uwq.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wti.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://xte.dashuyun.cn

Ruby: arr.index(x)
来源：http://lxt.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://zlv.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://coq.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pdk.dianchejie.cn


<!-- 参考信息 -->