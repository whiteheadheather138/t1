代发 wailian999

PHP:  $a && $b || !$c
来源：http://ntb.tian-w.cn

JS:   a && b || !c
来源：http://jeq.ydzc1.top

TS:   a && b || !c
来源：http://jrh.vehdjk.com

Java: a && b || !c
来源：http://byh.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://kpq.yj20258888.top

Ruby: a && b || !c
来源：http://zwo.meibo888.top

C#:   a && b || !c
来源：http://zup.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://fio.yuxming.cn

Py:   if not data: return
来源：http://tnn.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://syv.tanke756.top

JS:   if (!data) return;
来源：http://xnk.zhijiandao.cn

TS:   if (!data) return;
来源：http://rzs.cashguo.top

Java: if (data == null) return;
来源：http://hjf.hammf.cn

Go:   if data == nil { return }
来源：http://itq.zhoulong.xyz

Ruby: return if data.nil?
来源：http://lns.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://lry.shanyushiyangtech.top

================================================================================
来源：http://tmy.yvedp.cn

C. 函数与作用域
来源：http://aps.zhengqikj.top

================================================================================
来源：http://qme.zhengqikj.top

[C01] 定义函数
来源：http://enl.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://pnn.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://luq.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://lwd.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xwq.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nvn.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://zfm.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://yvj.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ngb.hongshengwenyu.top

[C02] 默认参数
来源：http://cxx.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ovz.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mzp.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://kxu.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ufz.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://irj.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://afm.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://qjc.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://jfu.hywenlv.cn

[C03] 可变参数
来源：http://zbl.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://nbn.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oyu.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vfu.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpp.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://moz.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gpe.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oli.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gkz.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://tzn.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tpa.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbf.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://inw.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fvc.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://esv.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://kdf.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://zsd.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://ijb.ppjwa.cn

[C05] 返回多个值
来源：http://zec.jinyuanbaomall.cn

Py:   return a, b
来源：http://ozn.xylfe.cn

PHP:  return [$a, $b];
来源：http://gnr.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lim.tarul.cn

TS:   return { a, b };
来源：http://idn.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nnn.zhixingplan.top

Go:   return a, b
来源：http://xgu.hysaishi.cn

Ruby: return a, b
来源：http://hpg.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://zhq.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://zkr.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://hbe.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yxw.cucudq.cn

JS:   const square = x => x * x;
来源：http://jmw.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://bti.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://syr.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ogt.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://ipo.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://jjm.cheryme.top

[C07] 把函数作为参数传入
来源：http://qkt.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jdc.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://czv.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjh.fengsongda.top

TS:   arr.map(String)
来源：http://cuo.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vki.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://icy.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://omk.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tqs.zdqjudy.top

[C08] 闭包
来源：http://fkr.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sbn.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://urb.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://umw.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qbg.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wpc.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tro.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zmg.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lqf.pengpengdd.cyou

[C09] 递归
来源：http://xdb.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vvy.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ojb.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tue.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tcu.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fyr.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ufg.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kpm.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vop.yvedp.cn

[C10] 变量作用域
来源：http://ici.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lwd.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bjz.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfg.zhixingplan.top

TS:   同 JS
来源：http://oag.jyoumei.cn

Java: 方法内为块级作用域
来源：http://fux.shzxlz.cn

Go:   花括号块级作用域
来源：http://uwj.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xnv.hysaishi.cn

C#:   块级作用域
来源：http://vmt.yuxming.cn

[C11] 模块导入与导出
来源：http://aoh.fengsongda.top

Py:   from module import func
来源：http://wyx.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uxe.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjb.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cls.hnxiangtu.top

Java: import java.util.List;
来源：http://cwd.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jho.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://qvi.uphjek.com

C#:   using System.Text;
来源：http://kyt.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://xun.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://sgj.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://civ.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://ldd.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://pmh.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gwe.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://fdx.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://fes.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rle.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://vea.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aid.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ucw.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qxi.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kab.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://jdn.xuanzx.com

Go:   func add(a, b int) int
来源：http://ibn.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fur.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://npg.guannengcc.top

[C14] 泛型函数
来源：http://pro.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ayp.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://wbd.jiagoushi.top

JS:   // 无泛型
来源：http://owa.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rkv.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ctc.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wic.aibaodan.cn

Ruby: # 无泛型
来源：http://bgi.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qdb.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://mgt.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://amh.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://abg.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://flk.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mly.chenzaomai.com

Java: // 无解构
来源：http://tvb.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://yio.xinyue.icu

Ruby: a, b = pair
来源：http://ypx.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://typ.tarul.cn

[C16] 函数 / 方法重载
来源：http://fyd.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rtk.guowangkeji.top

PHP:  // 无重载
来源：http://awn.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yqz.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://bdp.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uhf.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://myv.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://zlb.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nro.yvedp.cn

================================================================================
来源：http://jrw.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://mry.yfazqb.com

================================================================================
来源：http://ywm.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://jzt.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ouy.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kgr.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uge.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yqr.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxq.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://aaq.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://koc.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rgq.nanxinkj.top

[D02] 追加元素到末尾
来源：http://qaq.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lyz.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ett.daxiang520.top

JS:   arr.push(4);
来源：http://ubv.wangdashe.top

TS:   arr.push(4);
来源：http://grl.yanxiufei.cn

Java: list.add(4);
来源：http://oag.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://scm.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://qrg.jinqigufen.top

C#:   list.Add(4);
来源：http://etp.yueranfly.top

[D03] 在指定位置插入元素
来源：http://cvr.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://rlz.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wis.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://duf.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://ubv.aizwys.cn

Java: list.add(0, 0);
来源：http://jti.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://dac.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fbb.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://xqr.tarul.cn

[D04] 删除元素
来源：http://gvb.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ubi.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sgs.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jdt.yonumen.top

TS:   arr.splice(0, 1);
来源：http://vwk.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://myk.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cbd.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tgy.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kdk.jinqigufen.top

[D05] 访问与修改元素
来源：http://xuu.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iff.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lux.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rmg.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://oxq.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://lcx.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://fcx.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lko.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jqb.yj20258.top

[D06] 数组长度
来源：http://csh.shzxlz.cn

Py:   len(arr)
来源：http://tjl.ydjk.org.cn

PHP:  count($arr);
来源：http://uia.zdqjudy.top

JS:   arr.length
来源：http://olc.yj20258.top

TS:   arr.length
来源：http://fiy.jinqigfzy.top

Java: list.size();
来源：http://qjw.gotoacloud.top

Go:   len(arr)
来源：http://lfp.52xcode.cn

Ruby: arr.length; arr.size
来源：http://rfp.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://qme.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://gtv.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qwt.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://qhi.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://los.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://ktr.ivvv.top

Java: list.subList(1, 4);
来源：http://opj.hysaishi.cn

Go:   arr[1:4]
来源：http://cxp.ehwqpu.com

Ruby: arr[1, 3]
来源：http://nwj.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://xer.mhx1999.top

[D08] 合并两个数组
来源：http://ace.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://epc.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://fbi.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dig.meibo888.top

TS:   [...a, ...b];
来源：http://haf.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ocq.tarul.cn

Go:   append(a, b...)
来源：http://cfz.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://vuo.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://iry.c1oappe.top

[D09] 排序（升序）
来源：http://hxa.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://xnv.iojbl.cn

PHP:  sort($arr);
来源：http://kvc.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lgp.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nzy.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yzj.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tpp.daxiang520.top

Ruby: arr.sort
来源：http://qzg.fzhhl.top

C#:   list.Sort();
来源：http://cil.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://dpx.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jub.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ojp.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pyg.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bnr.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gdh.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vkb.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://anc.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xxl.xuetiantiany.cn

[D11] 反转数组
来源：http://apc.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://kgo.ivvv.top

PHP:  array_reverse($arr);
来源：http://zon.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nwr.sufxvd.cn

TS:   [...arr].reverse();
来源：http://wvn.ybcxt.top

Java: Collections.reverse(list);
来源：http://qyy.yj202588.top

Go:   slices.Reverse(arr)
来源：http://oyi.cucudq.cn

Ruby: arr.reverse
来源：http://mdc.nanxinkj.top

C#:   list.Reverse();
来源：http://erv.zhongyouzk.top

[D12] 查找元素下标
来源：http://wlo.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://wmu.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xbd.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bga.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://odf.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jts.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://usb.bbcook.cn

Ruby: arr.index(x)
来源：http://yyk.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://ulp.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://ppp.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pyd.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gdd.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://nrm.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://bxg.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eog.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sbt.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://axj.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://puy.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://bnu.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://foc.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ucy.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://wvh.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://tsb.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ova.jqgufenzy.top

Go:   // 手写循环
来源：http://hqt.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://sij.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mjm.ywan-chungtsiang.top

[D15] 去重
来源：http://mok.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qgu.guowangkeji.top

PHP:  array_unique($arr);
来源：http://dwo.birdmap.top

JS:   [...new Set(arr)]
来源：http://xlv.aizwys.cn

TS:   [...new Set(arr)]
来源：http://iif.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vtk.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://fkj.meibo888.top

Ruby: arr.uniq
来源：http://csd.sweek.top


<!-- 参考信息 -->