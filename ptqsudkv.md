代发 wailian999

C#:   x is int or double or decimal
来源：http://woo.cheryme.top

[B14] 判断值是否在集合内
来源：http://wsq.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xxq.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fnv.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://irx.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://cya.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vrw.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://udr.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://jgf.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://udz.gotoacloud.top

[B15] 布尔运算与取反
来源：http://uyk.yj20258888.top

Py:   a and b or not c
来源：http://max.smart0.xyz

PHP:  $a && $b || !$c
来源：http://mqf.0kj1m.cn

JS:   a && b || !c
来源：http://rjq.vehdjk.com

TS:   a && b || !c
来源：http://ess.cheryme.top

Java: a && b || !c
来源：http://qln.epnwcf.com

Go:   a && b || !c
来源：http://glp.iojbl.cn

Ruby: a && b || !c
来源：http://rtr.xinyue.icu

C#:   a && b || !c
来源：http://dmw.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dty.yueranfly.top

Py:   if not data: return
来源：http://myb.meibo888.top

PHP:  if (!$data) { return; }
来源：http://bbm.nanxinkj.top

JS:   if (!data) return;
来源：http://eum.nanxinkj.top

TS:   if (!data) return;
来源：http://orq.haohaochexian.top

Java: if (data == null) return;
来源：http://vmf.iojbl.cn

Go:   if data == nil { return }
来源：http://yrm.aizwys.cn

Ruby: return if data.nil?
来源：http://ofm.havefunace.top

C#:   if (data == null) return;
来源：http://pyu.fanxiaobao.xyz

================================================================================
来源：http://vhx.chenjidiqi.icu

C. 函数与作用域
来源：http://rkq.redwolf501.top

================================================================================
来源：http://ukj.shuidangran.top

[C01] 定义函数
来源：http://tgd.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://hwa.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pyv.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://tps.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzg.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://trm.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://ftw.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://omo.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hba.havefunace.top

[C02] 默认参数
来源：http://ijm.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://kym.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tua.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://mtw.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oot.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ths.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yoc.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://cms.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://iep.zhongyouzk.top

[C03] 可变参数
来源：http://njk.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://cqx.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qbi.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uem.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oly.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://glq.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ptv.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gav.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lhz.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://vpw.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rxa.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jqc.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpf.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ttw.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://oft.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://oob.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://lqg.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://iqo.gzhubu.top

[C05] 返回多个值
来源：http://wgl.zdqjudy.top

Py:   return a, b
来源：http://vwk.dashuyun.cn

PHP:  return [$a, $b];
来源：http://coy.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tyd.yj202588.top

TS:   return { a, b };
来源：http://oxn.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mre.tian-w.cn

Go:   return a, b
来源：http://mmk.hcnkem.com

Ruby: return a, b
来源：http://zvk.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://usp.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://guo.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://agi.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iru.zdqjudy.top

JS:   const square = x => x * x;
来源：http://eef.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://xrv.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://owj.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://elc.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://ege.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://mdo.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://qxw.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fef.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://wah.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tqb.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://wmx.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bnu.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yzf.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://xhb.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gjt.hysaishi.cn

[C08] 闭包
来源：http://zrt.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vpe.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vwq.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kgw.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sqb.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qus.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rsb.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://src.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rpq.yvedp.cn

[C09] 递归
来源：http://avs.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pyj.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xco.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qus.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmg.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yza.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ukr.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wtf.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hqj.ctjpmb.com

[C10] 变量作用域
来源：http://azz.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ugz.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ynh.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rod.dianchejie.cn

TS:   同 JS
来源：http://org.cheryme.top

Java: 方法内为块级作用域
来源：http://dcd.guowangkeji.top

Go:   花括号块级作用域
来源：http://tep.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nug.jqgufenzy.top

C#:   块级作用域
来源：http://dys.snrcjt.cn

[C11] 模块导入与导出
来源：http://obh.bjfxy.top

Py:   from module import func
来源：http://myc.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wlr.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://kat.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ogc.tian-w.cn

Java: import java.util.List;
来源：http://dqv.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kre.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://cay.shangyingyoupin.top

C#:   using System.Text;
来源：http://zkk.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://iqz.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://yyh.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://cbb.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://ons.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://cax.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xmr.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://enq.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://mzx.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eux.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://uev.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://llf.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifv.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpz.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cna.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kjl.guowangkeji.top

Go:   func add(a, b int) int
来源：http://aww.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tcr.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://oae.jinqigfzy.top

[C14] 泛型函数
来源：http://cwk.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tku.epnwcf.com

PHP:  // 无泛型
来源：http://wig.bbcook.cn

JS:   // 无泛型
来源：http://jwx.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://abo.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebz.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dbl.cdnleiting.top

Ruby: # 无泛型
来源：http://qnp.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jfb.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://ahr.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mun.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://tgl.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ogw.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://con.xuetiantiany.cn

Java: // 无解构
来源：http://rzq.zhiwuduotai.top

Go:   // 无解构
来源：http://gnb.vehdjk.com

Ruby: a, b = pair
来源：http://dtt.yj20258.top

C#:   var (a, b) = pair;
来源：http://qlf.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://tzi.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vsu.guannengcc.top

PHP:  // 无重载
来源：http://vmd.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://skd.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://kzt.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://szx.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://qmf.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://wvq.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ghk.gaohongyu789.top

================================================================================
来源：http://kmz.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://pyx.havefunace.top

================================================================================
来源：http://gom.c1oappe.top

[D01] 创建数组 / 列表
来源：http://rrc.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gxy.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://boa.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://itu.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bfi.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rrp.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://des.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://yyn.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://spc.cqqwz.cn

[D02] 追加元素到末尾
来源：http://puc.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ayb.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tbc.vqdsnc.cn

JS:   arr.push(4);
来源：http://nvb.cdnleiting.top

TS:   arr.push(4);
来源：http://bcn.cashguo.top

Java: list.add(4);
来源：http://cio.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://ofo.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://fyo.nwbrower.top

C#:   list.Add(4);
来源：http://utu.yongpay.top

[D03] 在指定位置插入元素
来源：http://xsx.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://zgd.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kuq.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://onl.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://yex.52xcode.cn

Java: list.add(0, 0);
来源：http://tkw.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uzn.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dmg.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://wgg.xuetiantiany.cn

[D04] 删除元素
来源：http://cni.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jpm.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oeu.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qrd.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://myj.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rnm.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ljy.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ubf.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rvh.xylfe.cn

[D05] 访问与修改元素
来源：http://ttu.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zif.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://euu.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yzi.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cof.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://mvl.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://bnh.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wxn.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iqd.quarkkingdee.top

[D06] 数组长度
来源：http://pzf.ybcxt.top

Py:   len(arr)
来源：http://qgi.yongpay.top

PHP:  count($arr);
来源：http://bqu.zhengqikj.top

JS:   arr.length
来源：http://ffi.zhixingplan.top

TS:   arr.length
来源：http://bbh.zdbjq.cn

Java: list.size();
来源：http://obo.pycfn.com

Go:   len(arr)
来源：http://cjm.xuanzx.com

Ruby: arr.length; arr.size
来源：http://heu.fengsongda.top

C#:   list.Count;
来源：http://vki.hnqzz.top

[D07] 切片 / 取子数组
来源：http://mjk.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cfy.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ute.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://oej.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://tpr.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://kcv.iojbl.cn

Go:   arr[1:4]
来源：http://vtm.cucudq.cn

Ruby: arr[1, 3]
来源：http://hmo.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://sbw.pengpengdd.cyou

[D08] 合并两个数组
来源：http://dqy.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://mfv.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://reu.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zxy.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://enh.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrk.gaohongyu789.top

Go:   append(a, b...)
来源：http://xoz.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://amm.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://flv.zycfv.cn

[D09] 排序（升序）
来源：http://oci.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://ehv.aibaodan.cn

PHP:  sort($arr);
来源：http://ujt.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fyv.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ffl.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xee.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nqg.aibaodan.cn

Ruby: arr.sort
来源：http://icj.gotoacloud.top

C#:   list.Sort();
来源：http://rzw.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wds.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hmv.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yaw.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://opf.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zpy.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fje.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmo.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cds.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qpo.meibo888.top

[D11] 反转数组
来源：http://prg.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://fcn.ivvv.top

PHP:  array_reverse($arr);
来源：http://thz.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vxe.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://qte.yj20258888.top

Java: Collections.reverse(list);
来源：http://oep.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://egb.cdnleiting.top

Ruby: arr.reverse
来源：http://zrw.yangfankeji.com

C#:   list.Reverse();
来源：http://usc.xylfe.cn

[D12] 查找元素下标
来源：http://jcd.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://fhj.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbp.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnv.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ppg.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://irk.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://tfg.hammf.cn

Ruby: arr.index(x)
来源：http://bsq.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://uao.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://tlp.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://odr.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://phd.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://hyq.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://qgg.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jof.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dsp.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oih.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zsx.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://kvi.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vvn.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vej.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://pfn.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://zdw.yanxiufei.cn


<!-- 参考信息 -->