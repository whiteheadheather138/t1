代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ruv.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gwv.xuanzx.com

[B15] 布尔运算与取反
来源：http://mii.xuetiantiany.cn

Py:   a and b or not c
来源：http://alw.hammf.cn

PHP:  $a && $b || !$c
来源：http://hur.hnqzz.top

JS:   a && b || !c
来源：http://gcd.epnwcf.com

TS:   a && b || !c
来源：http://aof.yj20258.top

Java: a && b || !c
来源：http://suj.andypj.xyz

Go:   a && b || !c
来源：http://znq.shangyingyoupin.top

Ruby: a && b || !c
来源：http://juz.cashguo.top

C#:   a && b || !c
来源：http://ojx.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://tnx.shzxlz.cn

Py:   if not data: return
来源：http://cwt.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://mcv.hysaishi.cn

JS:   if (!data) return;
来源：http://nkh.wangshuangyany.cn

TS:   if (!data) return;
来源：http://mfy.shuidangran.top

Java: if (data == null) return;
来源：http://amt.gotoacloud.top

Go:   if data == nil { return }
来源：http://sby.hywenlv.cn

Ruby: return if data.nil?
来源：http://htz.nanxuanxn.top

C#:   if (data == null) return;
来源：http://qjg.feifeiyinyue.top

================================================================================
来源：http://dsj.ydjk.org.cn

C. 函数与作用域
来源：http://sze.fktsv.cn

================================================================================
来源：http://lqj.bbcook.cn

[C01] 定义函数
来源：http://ons.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://vja.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfw.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://dqe.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fxn.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ghv.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://vxz.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://ssn.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xdc.xuanzx.com

[C02] 默认参数
来源：http://bbu.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://bdu.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dqq.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://hlr.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aql.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dqj.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pnc.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://ccy.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://djp.xuanzx.com

[C03] 可变参数
来源：http://rup.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://lyg.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xcq.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aiz.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iby.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jlg.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vfz.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://rmr.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fwf.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://xif.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dtd.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://otb.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijf.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bqf.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://gia.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://fzj.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://riq.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://jqj.daria6918.cn

[C05] 返回多个值
来源：http://uew.hammf.cn

Py:   return a, b
来源：http://odi.jyoumei.cn

PHP:  return [$a, $b];
来源：http://mwi.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lqe.shangyingyoupin.top

TS:   return { a, b };
来源：http://hzr.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ubm.xinyue.icu

Go:   return a, b
来源：http://hry.52xcode.cn

Ruby: return a, b
来源：http://usf.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://pxf.316326.xyz

[C06] 匿名函数 / lambda
来源：http://gsb.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://hha.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wef.hfpthk.cn

JS:   const square = x => x * x;
来源：http://ryv.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://ygo.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tps.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lvf.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://qrm.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://cbm.sysykeji.top

[C07] 把函数作为参数传入
来源：http://wow.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cdl.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fip.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ncs.yangfankeji.com

TS:   arr.map(String)
来源：http://iio.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kic.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ypi.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://scj.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ryv.tarul.cn

[C08] 闭包
来源：http://yep.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vsv.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oin.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qco.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sdb.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mfe.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xug.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tyt.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zbd.shuidangran.top

[C09] 递归
来源：http://miq.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://emr.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://brb.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwx.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpc.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aza.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aps.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zvf.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cqa.birdmap.top

[C10] 变量作用域
来源：http://nqh.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ekq.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vzo.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wid.fktsv.cn

TS:   同 JS
来源：http://hgp.zdqjudy.top

Java: 方法内为块级作用域
来源：http://jrg.iojbl.cn

Go:   花括号块级作用域
来源：http://cfv.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oke.ehwqpu.com

C#:   块级作用域
来源：http://qqt.zhixingplan.top

[C11] 模块导入与导出
来源：http://edl.xuetiantiany.cn

Py:   from module import func
来源：http://isa.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kcf.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zlu.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vfi.shangyingyoupin.top

Java: import java.util.List;
来源：http://wmf.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lqu.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://jao.snrcjt.cn

C#:   using System.Text;
来源：http://svy.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://bvx.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://lnt.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://amb.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://gcz.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://imr.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wcl.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://lfj.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://nuq.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rbd.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://zbh.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wtm.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fug.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lra.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wkj.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://stp.smart0.xyz

Go:   func add(a, b int) int
来源：http://twv.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cyz.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://nbl.shzxlz.cn

[C14] 泛型函数
来源：http://bfk.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rrv.zhixingplan.top

PHP:  // 无泛型
来源：http://osw.jinqigufen.top

JS:   // 无泛型
来源：http://evr.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://shl.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://djp.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lgm.fengsongda.top

Ruby: # 无泛型
来源：http://mkg.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ulh.sweek.top

[C15] 解构 / 展开参数
来源：http://uhf.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nrx.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://gcp.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zpw.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zqb.ybcxt.top

Java: // 无解构
来源：http://cpu.cucudq.cn

Go:   // 无解构
来源：http://mtx.yonumen.top

Ruby: a, b = pair
来源：http://ych.xylfe.cn

C#:   var (a, b) = pair;
来源：http://tkb.tarul.cn

[C16] 函数 / 方法重载
来源：http://vwp.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfo.fzhhl.top

PHP:  // 无重载
来源：http://bdd.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsz.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://mav.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ebs.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://ucm.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://vje.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mtr.ydjk.org.cn

================================================================================
来源：http://pbd.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://opi.jqgufenzy.top

================================================================================
来源：http://drj.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://cis.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kyo.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bzo.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eqv.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dcp.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tpj.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://svk.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://nij.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vgl.fktsv.cn

[D02] 追加元素到末尾
来源：http://kge.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gzb.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ptp.hnqzz.top

JS:   arr.push(4);
来源：http://bgo.cucudq.cn

TS:   arr.push(4);
来源：http://nyc.mhx1999.top

Java: list.add(4);
来源：http://kju.316326.xyz

Go:   arr = append(arr, 4)
来源：http://bpw.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://eyw.iojbl.cn

C#:   list.Add(4);
来源：http://usi.birdmap.top

[D03] 在指定位置插入元素
来源：http://cia.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://awp.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qjg.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rda.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://meh.jyoumei.cn

Java: list.add(0, 0);
来源：http://vko.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://njb.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uvu.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://tuf.zdqjudy.top

[D04] 删除元素
来源：http://jzi.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://okj.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ceh.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qao.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://ljp.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hiw.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pez.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://teh.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ayr.0kj1m.cn

[D05] 访问与修改元素
来源：http://oan.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kqn.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ggn.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xzq.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://zlj.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://hch.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://aun.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rvm.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lvy.9152youxi.cn

[D06] 数组长度
来源：http://ohn.ydjk.org.cn

Py:   len(arr)
来源：http://vpk.nanxinkj.top

PHP:  count($arr);
来源：http://buj.yanxiufei.cn

JS:   arr.length
来源：http://lmj.aibaodan.cn

TS:   arr.length
来源：http://ava.yanxiufei.cn

Java: list.size();
来源：http://ipm.guowangkeji.top

Go:   len(arr)
来源：http://hvo.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://wvh.shanyushiyangkeji.top

C#:   list.Count;
来源：http://qtg.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://lgm.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hbj.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zcj.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://tms.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://bda.chenlongwang.top

Java: list.subList(1, 4);
来源：http://rwj.xuanzx.com

Go:   arr[1:4]
来源：http://dvp.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://nsg.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://kjw.zdbjq.cn

[D08] 合并两个数组
来源：http://teu.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://xsa.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://mql.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jos.sxryk.cn

TS:   [...a, ...b];
来源：http://mba.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wbj.cashguo.top

Go:   append(a, b...)
来源：http://aye.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://uee.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://xhb.zdbjq.cn

[D09] 排序（升序）
来源：http://zil.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://xmh.tanke756.top

PHP:  sort($arr);
来源：http://eaa.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ozt.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zcv.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yzc.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://njz.jiagoushi.top

Ruby: arr.sort
来源：http://qaa.fengsongda.top

C#:   list.Sort();
来源：http://sjv.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bgg.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cac.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iry.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://drs.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fdg.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hfc.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wbn.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ena.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lds.cashguo.top

[D11] 反转数组
来源：http://ggu.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://klb.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://wmd.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zpo.52xcode.cn

TS:   [...arr].reverse();
来源：http://gob.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://ffd.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://fbd.haohaochexian.top

Ruby: arr.reverse
来源：http://qfe.hnqzz.top

C#:   list.Reverse();
来源：http://wyt.xuetiantiany.cn

[D12] 查找元素下标
来源：http://vdt.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://ndr.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hob.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rms.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qjk.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pmb.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://dzm.cdnleiting.top

Ruby: arr.index(x)
来源：http://mpw.xinyue.icu

C#:   list.IndexOf(x);
来源：http://obz.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://vkd.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kis.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ssk.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://lcb.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://jjg.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xpa.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pzw.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://puz.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://jty.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://ewo.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cxz.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aka.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://tvr.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://dfl.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://xhb.xuanzx.com

Go:   // 手写循环
来源：http://phv.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dqh.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bdr.cheryme.top

[D15] 去重
来源：http://lik.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jta.jyoumei.cn

PHP:  array_unique($arr);
来源：http://dxu.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://ndi.jyoumei.cn


<!-- 参考信息 -->