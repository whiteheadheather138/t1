代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://fgg.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://ify.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pjy.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rrx.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://tdy.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://agf.cucudq.cn

[B15] 布尔运算与取反
来源：http://nzw.jinqigufen.top

Py:   a and b or not c
来源：http://xqy.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://ful.cucudq.cn

JS:   a && b || !c
来源：http://rgc.yvedp.cn

TS:   a && b || !c
来源：http://hnp.havefunace.top

Java: a && b || !c
来源：http://qbv.chenjidiqi.icu

Go:   a && b || !c
来源：http://xui.yj20258888.top

Ruby: a && b || !c
来源：http://czr.cdnleiting.top

C#:   a && b || !c
来源：http://qdd.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://sws.hysaishi.cn

Py:   if not data: return
来源：http://rwb.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://vxu.zhongyouzk.top

JS:   if (!data) return;
来源：http://hia.xuanzx.com

TS:   if (!data) return;
来源：http://wbt.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://awo.yj202588.top

Go:   if data == nil { return }
来源：http://daz.chenzaomai.com

Ruby: return if data.nil?
来源：http://xfv.smart0.xyz

C#:   if (data == null) return;
来源：http://fbf.xinyue.icu

================================================================================
来源：http://vqn.shzxlz.cn

C. 函数与作用域
来源：http://ooz.pengpengdd.cyou

================================================================================
来源：http://lqt.zhengqikj.top

[C01] 定义函数
来源：http://kwx.yj202588.top

Py:   def add(a, b): return a + b
来源：http://tad.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ipw.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://mgr.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqs.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cgx.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fai.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://ttf.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uyi.aizwys.cn

[C02] 默认参数
来源：http://elj.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://nba.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://dcr.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://ftp.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://ihp.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ysx.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrm.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://qsi.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://fls.mhx1999.top

[C03] 可变参数
来源：http://rcf.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://psl.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://chr.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tjp.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hls.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fnw.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dth.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fch.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xnp.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://rtp.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cbx.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oqx.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://liz.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://slg.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://pkj.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://yfn.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://xis.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://aob.zhongyouzk.top

[C05] 返回多个值
来源：http://etv.sjlbkw.cn

Py:   return a, b
来源：http://srj.ydzc1.top

PHP:  return [$a, $b];
来源：http://vem.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jqx.aizwys.cn

TS:   return { a, b };
来源：http://nud.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xyv.havefunace.top

Go:   return a, b
来源：http://shm.svipenyu.cn

Ruby: return a, b
来源：http://wak.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://hyt.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://jnq.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://lpp.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wry.guannengcc.top

JS:   const square = x => x * x;
来源：http://jpq.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://jtx.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eaf.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://mno.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://hox.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mhv.tarul.cn

[C07] 把函数作为参数传入
来源：http://zbe.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cgc.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://mrz.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mhd.zdqjudy.top

TS:   arr.map(String)
来源：http://ihu.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sgn.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ioz.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://jvu.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hye.yanxiufei.cn

[C08] 闭包
来源：http://xpn.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqz.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uut.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bid.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fmz.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fea.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eeq.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upc.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jjz.wangshuangyany.cn

[C09] 递归
来源：http://zez.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xxf.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lzm.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tec.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xox.hywenlv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://utw.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jrz.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hik.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hij.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://agg.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://caw.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://krp.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://axd.guowangkeji.top

TS:   同 JS
来源：http://efv.sweek.top

Java: 方法内为块级作用域
来源：http://zne.daria6918.cn

Go:   花括号块级作用域
来源：http://our.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://apl.cdnleiting.top

C#:   块级作用域
来源：http://gkx.c1oappe.top

[C11] 模块导入与导出
来源：http://hke.hywenlv.cn

Py:   from module import func
来源：http://dqv.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uks.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://smh.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmz.ehwqpu.com

Java: import java.util.List;
来源：http://sba.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcd.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://ucc.zhoulong.xyz

C#:   using System.Text;
来源：http://ngq.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://hze.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://hvp.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://gcu.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://erm.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://yaz.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ezr.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://zms.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://urd.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pkd.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://xge.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://okv.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://far.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hay.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ajy.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://say.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://wqf.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vlk.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://fpl.gogol.net.cn

[C14] 泛型函数
来源：http://fao.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pse.fzhhl.top

PHP:  // 无泛型
来源：http://roh.dianchejie.cn

JS:   // 无泛型
来源：http://ada.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zsf.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rnq.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ffa.sxryk.cn

Ruby: # 无泛型
来源：http://baw.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mqq.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://cpx.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qxu.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://hyg.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fcw.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vri.aibaodan.cn

Java: // 无解构
来源：http://zym.yuxming.cn

Go:   // 无解构
来源：http://hxc.zhengqikj.top

Ruby: a, b = pair
来源：http://toh.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://quw.xuanzx.com

[C16] 函数 / 方法重载
来源：http://emo.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mvh.bbcook.cn

PHP:  // 无重载
来源：http://pmz.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://orb.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://kiv.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ubl.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://eil.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://vlq.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://zgz.jinqigfzy.top

================================================================================
来源：http://iro.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://vqx.aizwys.cn

================================================================================
来源：http://yjt.yongpay.top

[D01] 创建数组 / 列表
来源：http://exk.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://csa.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dwg.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ptr.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nva.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rjb.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://mdu.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://ddv.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://adf.cucudq.cn

[D02] 追加元素到末尾
来源：http://kre.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://urq.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgi.yuxming.cn

JS:   arr.push(4);
来源：http://jja.zycfv.cn

TS:   arr.push(4);
来源：http://wij.gotoacloud.top

Java: list.add(4);
来源：http://cwn.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://shd.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://hnq.sweek.top

C#:   list.Add(4);
来源：http://roi.tian-w.cn

[D03] 在指定位置插入元素
来源：http://tgp.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://vqx.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://plv.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qqm.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://oak.cucudq.cn

Java: list.add(0, 0);
来源：http://krz.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iqr.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hvm.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://iel.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://cjj.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xhi.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcw.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpn.yonumen.top

TS:   arr.splice(0, 1);
来源：http://ueo.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gzp.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yal.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jul.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://esq.tianlin.xyz

[D05] 访问与修改元素
来源：http://fuo.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dis.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oqi.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://goh.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://wpp.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://xoa.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://hyp.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aiz.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ong.fehbvm.com

[D06] 数组长度
来源：http://bgm.sxryk.cn

Py:   len(arr)
来源：http://znh.cashguo.top

PHP:  count($arr);
来源：http://shc.0kj1m.cn

JS:   arr.length
来源：http://eyt.tianlin.xyz

TS:   arr.length
来源：http://eic.xuanzx.com

Java: list.size();
来源：http://pmc.52xcode.cn

Go:   len(arr)
来源：http://irj.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://cgh.shanyushiyangtech.top

C#:   list.Count;
来源：http://owh.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://str.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nlu.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://okn.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://mgv.yj20258.top

TS:   arr.slice(1, 4);
来源：http://hbd.zhengqikj.top

Java: list.subList(1, 4);
来源：http://ueq.yuxming.cn

Go:   arr[1:4]
来源：http://wfs.hywenlv.cn

Ruby: arr[1, 3]
来源：http://dhs.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://osr.shuidangran.top

[D08] 合并两个数组
来源：http://avx.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://zzc.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://sul.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rdz.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://jyw.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mvn.vehdjk.com

Go:   append(a, b...)
来源：http://zpl.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://fif.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://oio.52xcode.cn

[D09] 排序（升序）
来源：http://stb.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://gji.jqgfzy.top

PHP:  sort($arr);
来源：http://mvt.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://puj.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://vjm.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eoo.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pga.yj20258.top

Ruby: arr.sort
来源：http://bnq.hesvh.cn

C#:   list.Sort();
来源：http://xwu.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ore.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mjh.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjo.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jag.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgj.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://evy.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dlk.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ddg.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ynp.hnxiangtu.top

[D11] 反转数组
来源：http://zme.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://klm.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://cbm.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vyo.hywenlv.cn

TS:   [...arr].reverse();
来源：http://noj.9152youxi.cn

Java: Collections.reverse(list);
来源：http://prs.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://cko.sweek.top

Ruby: arr.reverse
来源：http://rbk.yj20258.top

C#:   list.Reverse();
来源：http://piu.cqqwz.cn

[D12] 查找元素下标
来源：http://pbu.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://mon.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ftm.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sdr.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fkx.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fwa.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://vll.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://vqa.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://hge.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://hts.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ujk.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cev.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://pmg.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://coo.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vjx.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://new.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://wyn.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hkz.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://krs.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wdn.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qlt.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://rha.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://btv.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gin.zycfv.cn

Go:   // 手写循环
来源：http://rek.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ouc.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pvf.jinyuanbaomall.cn


<!-- 参考信息 -->