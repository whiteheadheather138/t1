代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://qap.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qbj.fktsv.cn

[B15] 布尔运算与取反
来源：http://mxx.jinghuilouyu.cn

Py:   a and b or not c
来源：http://wza.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://pcq.jinghuilouyu.cn

JS:   a && b || !c
来源：http://dpl.kuanghao11.cn

TS:   a && b || !c
来源：http://ojw.kuanghao11.cn

Java: a && b || !c
来源：http://fmk.jianghu66.top

Go:   a && b || !c
来源：http://uhc.gotoacloud.top

Ruby: a && b || !c
来源：http://djc.jinghuilouyu.cn

C#:   a && b || !c
来源：http://nih.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ypb.9152youxi.cn

Py:   if not data: return
来源：http://ytg.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://dgc.iojbl.cn

JS:   if (!data) return;
来源：http://rlv.feifeiyinyue.top

TS:   if (!data) return;
来源：http://uop.nanxinkj.top

Java: if (data == null) return;
来源：http://qlg.cheryme.top

Go:   if data == nil { return }
来源：http://atj.hcnkem.com

Ruby: return if data.nil?
来源：http://mfx.zdbjq.cn

C#:   if (data == null) return;
来源：http://xgt.sysykeji.top

================================================================================
来源：http://btc.xziqi.cn

C. 函数与作用域
来源：http://fhm.zhiwuduotai.top

================================================================================
来源：http://zcu.zhengqikj.top

[C01] 定义函数
来源：http://kzo.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://hvo.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ptp.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://tvo.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnm.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pat.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jvu.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://obo.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://opr.yuanzhike.top

[C02] 默认参数
来源：http://mqf.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://xhx.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zgx.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://ykn.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rrk.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ldd.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nbm.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://vpm.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://kew.jyoumei.cn

[C03] 可变参数
来源：http://ctb.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://dvi.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gbj.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhn.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tod.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fxo.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yna.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xlo.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xse.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://qrp.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owm.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://atf.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mhv.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ruv.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://hkm.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://krr.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://byg.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://ztu.yonumen.top

[C05] 返回多个值
来源：http://lzq.fktsv.cn

Py:   return a, b
来源：http://wby.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://wyx.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://mca.andypj.xyz

TS:   return { a, b };
来源：http://msm.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ywc.zdbjq.cn

Go:   return a, b
来源：http://dqt.ybcxt.top

Ruby: return a, b
来源：http://vzj.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://sno.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://swx.nwbrower.top

Py:   square = lambda x: x * x
来源：http://bqg.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yti.tian-w.cn

JS:   const square = x => x * x;
来源：http://lxo.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://whj.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ovr.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://kot.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://tun.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://dax.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://ecq.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lqy.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://nxa.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://por.ydzc1.top

TS:   arr.map(String)
来源：http://bcj.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://khn.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://esj.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://daq.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://owh.birdmap.top

[C08] 闭包
来源：http://nhp.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lic.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qga.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sac.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ioy.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vst.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://akx.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hfe.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qjq.zhoulong.xyz

[C09] 递归
来源：http://cby.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gey.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pxy.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ntu.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gfx.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tgr.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wot.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iub.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vrf.chenlongwang.top

[C10] 变量作用域
来源：http://pyg.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gjx.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryz.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jac.yangfankeji.com

TS:   同 JS
来源：http://yia.tian-w.cn

Java: 方法内为块级作用域
来源：http://glh.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://xux.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ile.tianlin.xyz

C#:   块级作用域
来源：http://nim.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://opl.fktsv.cn

Py:   from module import func
来源：http://zwz.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zro.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kdt.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cwm.shzxlz.cn

Java: import java.util.List;
来源：http://ktm.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hqb.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://ixx.jinghuilouyu.cn

C#:   using System.Text;
来源：http://qwy.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://rje.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://hnx.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://ydd.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://sia.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://lae.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mnx.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://uwi.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://bat.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fud.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://fom.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pud.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://exw.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vkz.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fie.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://lvx.tanke756.top

Go:   func add(a, b int) int
来源：http://gov.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lvj.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://mjd.xuetiantiany.cn

[C14] 泛型函数
来源：http://mwn.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://skv.bbcook.cn

PHP:  // 无泛型
来源：http://ctd.ppjwa.cn

JS:   // 无泛型
来源：http://hmd.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iry.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ytf.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://muo.jiagoushi.top

Ruby: # 无泛型
来源：http://jvr.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvq.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://eyf.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hdo.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://nrk.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://noq.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eiv.jinqigfzy.top

Java: // 无解构
来源：http://jqe.sxryk.cn

Go:   // 无解构
来源：http://yqq.nanxinkj.top

Ruby: a, b = pair
来源：http://jub.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://vcg.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://jpg.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uvg.tanke756.top

PHP:  // 无重载
来源：http://fus.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://dtg.tarul.cn

TS:   // 用联合类型或重载签名声明
来源：http://ssq.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bfu.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://ior.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://pja.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kwq.quarkkingdee.top

================================================================================
来源：http://bik.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://pnr.52xcode.cn

================================================================================
来源：http://ipf.shuidangran.top

[D01] 创建数组 / 列表
来源：http://mvk.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pym.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://koe.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nrm.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ivh.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://smd.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://roy.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://vdd.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jqq.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://fwd.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zzi.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vse.zhoulong.xyz

JS:   arr.push(4);
来源：http://kdt.tianlin.xyz

TS:   arr.push(4);
来源：http://hbh.tianlin.xyz

Java: list.add(4);
来源：http://jxy.pycfn.com

Go:   arr = append(arr, 4)
来源：http://qjd.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://wza.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://vbl.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://opb.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://ivb.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umo.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nty.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://oli.quarkkingdee.top

Java: list.add(0, 0);
来源：http://xtt.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mjf.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qbb.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://rhu.yanxiufei.cn

[D04] 删除元素
来源：http://lav.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ijh.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xwx.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hiu.cashguo.top

TS:   arr.splice(0, 1);
来源：http://isq.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tup.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wzz.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aqs.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://asq.fehbvm.com

[D05] 访问与修改元素
来源：http://myt.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kdi.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qua.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://atz.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://evv.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://grj.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://yki.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kpa.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fex.fengsongda.top

[D06] 数组长度
来源：http://jcw.9152youxi.cn

Py:   len(arr)
来源：http://sug.nwbrower.top

PHP:  count($arr);
来源：http://jjr.shuidangran.top

JS:   arr.length
来源：http://uia.sysykeji.top

TS:   arr.length
来源：http://hvp.fehbvm.com

Java: list.size();
来源：http://ybe.gogol.net.cn

Go:   len(arr)
来源：http://tjq.iojbl.cn

Ruby: arr.length; arr.size
来源：http://cxy.aibaodan.cn

C#:   list.Count;
来源：http://tnq.redwolf501.top

[D07] 切片 / 取子数组
来源：http://rxq.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sct.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jka.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://mtp.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://mbj.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://mpw.ehwqpu.com

Go:   arr[1:4]
来源：http://fyr.ppjwa.cn

Ruby: arr[1, 3]
来源：http://exj.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://hjr.uphjek.com

[D08] 合并两个数组
来源：http://dbi.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://eqk.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://klz.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ugp.zhengqikj.top

TS:   [...a, ...b];
来源：http://gpi.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wgx.zdqjudy.top

Go:   append(a, b...)
来源：http://gjj.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://lvb.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://mmh.cucudq.cn

[D09] 排序（升序）
来源：http://rju.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://iyw.ehwqpu.com

PHP:  sort($arr);
来源：http://buf.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mqg.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mkt.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hdh.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iub.yfazqb.com

Ruby: arr.sort
来源：http://ldh.zhengqikj.top

C#:   list.Sort();
来源：http://iyn.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zrd.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uqk.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tzw.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjs.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lww.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zmg.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opp.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zso.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://enu.haohaochexian.top

[D11] 反转数组
来源：http://ehe.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://chk.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://tww.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pos.fktsv.cn

TS:   [...arr].reverse();
来源：http://xya.cucudq.cn

Java: Collections.reverse(list);
来源：http://bes.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://gzu.meibo888.top

Ruby: arr.reverse
来源：http://yms.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://ywi.fehbvm.com

[D12] 查找元素下标
来源：http://vhs.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://nri.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ghc.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qyl.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://scx.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pns.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://ewc.snrcjt.cn

Ruby: arr.index(x)
来源：http://enm.wangdashe.top

C#:   list.IndexOf(x);
来源：http://sjz.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://jhr.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://brh.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rqi.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://aca.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://kkt.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gey.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hlp.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://rvd.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wqp.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://mzd.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vwp.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mif.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://xvy.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://zvo.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://amz.zycfv.cn

Go:   // 手写循环
来源：http://txe.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://llx.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sla.jyoumei.cn

[D15] 去重
来源：http://kdt.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hwm.cheryme.top

PHP:  array_unique($arr);
来源：http://blg.hammf.cn

JS:   [...new Set(arr)]
来源：http://fmm.dashuyun.cn


<!-- 参考信息 -->