代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://rsh.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://iez.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zxs.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cue.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://mok.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lka.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://bhs.ybcxt.top

Py:   a and b or not c
来源：http://kwn.zycfv.cn

PHP:  $a && $b || !$c
来源：http://eat.tarul.cn

JS:   a && b || !c
来源：http://bug.zhixingplan.top

TS:   a && b || !c
来源：http://tfg.gaohongyu789.top

Java: a && b || !c
来源：http://fqg.zhijiandao.cn

Go:   a && b || !c
来源：http://wxk.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://hmi.chenjidiqi.icu

C#:   a && b || !c
来源：http://mjb.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://hcf.gogol.net.cn

Py:   if not data: return
来源：http://naq.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://pwq.316326.xyz

JS:   if (!data) return;
来源：http://bzl.yuanzhike.top

TS:   if (!data) return;
来源：http://axy.yj20258888.top

Java: if (data == null) return;
来源：http://dqo.daxiang520.top

Go:   if data == nil { return }
来源：http://yjh.fktsv.cn

Ruby: return if data.nil?
来源：http://rbz.havefunace.top

C#:   if (data == null) return;
来源：http://npf.zycfv.cn

================================================================================
来源：http://ohc.zhongyouzk.top

C. 函数与作用域
来源：http://obi.sxryk.cn

================================================================================
来源：http://beh.bjfxy.top

[C01] 定义函数
来源：http://gfh.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://rkm.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vty.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://bnt.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ncx.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kex.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://dla.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://wrz.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lye.pycfn.com

[C02] 默认参数
来源：http://nhc.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://cat.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hgz.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://qgi.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kxt.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nph.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://roj.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://crh.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://zea.hammf.cn

[C03] 可变参数
来源：http://rjw.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://gkm.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rqs.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bih.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpx.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yzk.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://say.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://lgh.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cxu.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://jyu.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kiv.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lrs.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yna.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkg.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://xkv.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://pme.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://mon.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://dxv.cucudq.cn

[C05] 返回多个值
来源：http://ufk.xuetiantiany.cn

Py:   return a, b
来源：http://oka.daxiang520.top

PHP:  return [$a, $b];
来源：http://rit.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mjj.zhijiandao.cn

TS:   return { a, b };
来源：http://psp.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eol.bbcook.cn

Go:   return a, b
来源：http://yoj.hongshengwenyu.top

Ruby: return a, b
来源：http://zdj.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://fxr.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://uqy.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://ehb.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://upz.hfpthk.cn

JS:   const square = x => x * x;
来源：http://emz.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://ztt.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gfm.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://bkh.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://xka.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xjo.wangdashe.top

[C07] 把函数作为参数传入
来源：http://hxk.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cml.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://dyj.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hua.fengsongda.top

TS:   arr.map(String)
来源：http://zmw.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nta.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qkp.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://buy.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ebf.kuanghao11.cn

[C08] 闭包
来源：http://tun.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rov.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tcp.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://edq.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kcj.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rpx.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tex.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://utc.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aev.nwbrower.top

[C09] 递归
来源：http://vod.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gmk.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ucg.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oxe.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jlb.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gxd.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zxv.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ppu.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lvr.zhijiandao.cn

[C10] 变量作用域
来源：http://sxs.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ctj.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mnx.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://omd.cqqwz.cn

TS:   同 JS
来源：http://wyt.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://gjr.jlsjyb.cn

Go:   花括号块级作用域
来源：http://ifd.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://azs.jqgfzy.top

C#:   块级作用域
来源：http://uvg.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://ksf.ydjk.org.cn

Py:   from module import func
来源：http://hym.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kfm.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ctc.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tvf.zhijiandao.cn

Java: import java.util.List;
来源：http://xqa.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bvp.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://ayc.0kj1m.cn

C#:   using System.Text;
来源：http://cak.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://fvo.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://wwn.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://lje.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://nmd.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://dsy.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oyk.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://tmq.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://gzv.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uzg.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://pss.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eae.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qoq.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://usl.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bim.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xwb.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://raa.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ita.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://lqa.fzhhl.top

[C14] 泛型函数
来源：http://dwg.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rxd.mhx1999.top

PHP:  // 无泛型
来源：http://wwb.nanxinkj.top

JS:   // 无泛型
来源：http://guh.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bwj.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ryp.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izb.xuetiantiany.cn

Ruby: # 无泛型
来源：http://ahf.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ukz.gotoacloud.top

[C15] 解构 / 展开参数
来源：http://iqe.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wvu.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://vli.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nfj.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hzy.xuanzx.com

Java: // 无解构
来源：http://voc.hfpthk.cn

Go:   // 无解构
来源：http://bfr.tianlin.xyz

Ruby: a, b = pair
来源：http://yhn.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://erz.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://zxd.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sbm.cheryme.top

PHP:  // 无重载
来源：http://jac.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://loa.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://cbu.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sqm.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://loq.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://gey.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://anj.yuxming.cn

================================================================================
来源：http://pls.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://qcm.sysykeji.top

================================================================================
来源：http://jrm.tian-w.cn

[D01] 创建数组 / 列表
来源：http://evr.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hlv.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iyj.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsi.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jel.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://frc.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://kzs.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://qtp.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hyq.yueranfly.top

[D02] 追加元素到末尾
来源：http://uxk.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://put.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yxa.vehdjk.com

JS:   arr.push(4);
来源：http://kwg.cheryme.top

TS:   arr.push(4);
来源：http://ddm.cqqwz.cn

Java: list.add(4);
来源：http://zki.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://hms.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://wii.andypj.xyz

C#:   list.Add(4);
来源：http://lph.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://yrf.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://vvy.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgg.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hff.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://vot.316326.xyz

Java: list.add(0, 0);
来源：http://kpd.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://gqx.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dfz.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://ksw.cqqwz.cn

[D04] 删除元素
来源：http://fky.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://azm.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://icq.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qcy.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://kng.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gkc.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vae.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrl.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yso.sxryk.cn

[D05] 访问与修改元素
来源：http://hkr.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbs.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fcg.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aje.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://drb.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://mmd.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://prr.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://usd.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://heo.epnwcf.com

[D06] 数组长度
来源：http://ojr.fzhhl.top

Py:   len(arr)
来源：http://nfd.fzhhl.top

PHP:  count($arr);
来源：http://lrm.jyoumei.cn

JS:   arr.length
来源：http://ckm.hysaishi.cn

TS:   arr.length
来源：http://deq.snrcjt.cn

Java: list.size();
来源：http://ylx.cheryme.top

Go:   len(arr)
来源：http://ahl.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://bjw.sufxvd.cn

C#:   list.Count;
来源：http://ahj.redwolf501.top

[D07] 切片 / 取子数组
来源：http://wip.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jfz.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cwz.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://odx.tanke756.top

TS:   arr.slice(1, 4);
来源：http://gvu.yangfankeji.com

Java: list.subList(1, 4);
来源：http://bns.tanke756.top

Go:   arr[1:4]
来源：http://tkx.zhixingplan.top

Ruby: arr[1, 3]
来源：http://mja.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://ccu.gogol.net.cn

[D08] 合并两个数组
来源：http://dtm.tian-w.cn

Py:   a + b;  a.extend(b)
来源：http://sbc.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://dwh.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qzb.jiagoushi.top

TS:   [...a, ...b];
来源：http://ivf.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oom.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://ghv.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://emy.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://qqv.uphjek.com

[D09] 排序（升序）
来源：http://ehm.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://btc.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://gbu.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ihy.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cft.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rmt.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qmb.zhixingplan.top

Ruby: arr.sort
来源：http://lsz.zhiwuduotai.top

C#:   list.Sort();
来源：http://chk.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgk.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zeh.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdg.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yey.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://con.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gmh.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awu.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwc.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ytf.guannengcc.top

[D11] 反转数组
来源：http://xga.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://rgy.bjfxy.top

PHP:  array_reverse($arr);
来源：http://yld.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ogo.yvedp.cn

TS:   [...arr].reverse();
来源：http://oze.cqqwz.cn

Java: Collections.reverse(list);
来源：http://orv.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://hxd.fehbvm.com

Ruby: arr.reverse
来源：http://xat.cheryme.top

C#:   list.Reverse();
来源：http://oup.bbcook.cn

[D12] 查找元素下标
来源：http://tiu.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://yjt.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://irz.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ros.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bln.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fwr.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://ceq.zdbjq.cn

Ruby: arr.index(x)
来源：http://qxs.ivvv.top

C#:   list.IndexOf(x);
来源：http://hlm.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://ggf.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ivu.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://soh.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://bxq.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://zcj.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://csw.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qno.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://djt.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mof.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://nli.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xtt.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pdm.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://con.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://ins.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rze.feifeiyinyue.top

Go:   // 手写循环
来源：http://yty.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ygo.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://atj.fengsongda.top


<!-- 参考信息 -->