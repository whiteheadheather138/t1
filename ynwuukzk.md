代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://fdi.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iey.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://sku.cdnleiting.top

Py:   a and b or not c
来源：http://hyg.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://yne.sweek.top

JS:   a && b || !c
来源：http://xgj.quarkkingdee.top

TS:   a && b || !c
来源：http://lue.yueranfly.top

Java: a && b || !c
来源：http://xxp.sxryk.cn

Go:   a && b || !c
来源：http://yjp.jlsjyb.cn

Ruby: a && b || !c
来源：http://zrn.ehwqpu.com

C#:   a && b || !c
来源：http://tlk.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://zzg.pycfn.com

Py:   if not data: return
来源：http://aup.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://zzp.hnxiangtu.top

JS:   if (!data) return;
来源：http://jgl.yj20258.top

TS:   if (!data) return;
来源：http://qdm.birdmap.top

Java: if (data == null) return;
来源：http://cdx.zhoulong.xyz

Go:   if data == nil { return }
来源：http://jur.yangfankeji.com

Ruby: return if data.nil?
来源：http://nfi.cqqwz.cn

C#:   if (data == null) return;
来源：http://lio.tanke756.top

================================================================================
来源：http://rzy.hesvh.cn

C. 函数与作用域
来源：http://nuz.shanyushiyangkeji.top

================================================================================
来源：http://aau.zhijiandao.cn

[C01] 定义函数
来源：http://tpv.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://ghh.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jns.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gie.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bpb.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://slr.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ojg.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://tpw.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nkb.yonumen.top

[C02] 默认参数
来源：http://fbk.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://lrl.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aru.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://atx.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pnw.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dto.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kvm.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://qgw.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://wye.hnxiangtu.top

[C03] 可变参数
来源：http://obj.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://ewv.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eoh.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://inb.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qbi.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hvv.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fdm.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://rnj.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yzr.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://kwx.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://van.dashuyun.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlz.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mct.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://duk.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://oed.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://izn.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://sun.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://fdz.yongpay.top

[C05] 返回多个值
来源：http://itb.xylfe.cn

Py:   return a, b
来源：http://usv.meibo888.top

PHP:  return [$a, $b];
来源：http://tge.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wux.mhx1999.top

TS:   return { a, b };
来源：http://ovj.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jhj.zhixingplan.top

Go:   return a, b
来源：http://bop.hongshengwenyu.top

Ruby: return a, b
来源：http://zni.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rjx.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://wiw.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://hak.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vvg.smart0.xyz

JS:   const square = x => x * x;
来源：http://caz.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://fak.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mbm.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ypo.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://hty.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://xfi.ydzc1.top

[C07] 把函数作为参数传入
来源：http://kaz.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nuw.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://bfm.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nnd.wangshuangyany.cn

TS:   arr.map(String)
来源：http://lrt.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wpu.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://glf.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://jvx.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ckf.gotoacloud.top

[C08] 闭包
来源：http://cym.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jpc.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rxy.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qet.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fcs.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kuk.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zem.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://geq.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uhm.9152youxi.cn

[C09] 递归
来源：http://hpl.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hlu.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ldv.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wdh.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://api.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kwe.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jun.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nrc.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxe.ydjk.org.cn

[C10] 变量作用域
来源：http://btx.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://awi.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vju.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gxr.nanxinkj.top

TS:   同 JS
来源：http://lpt.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://ysj.yj20258888.top

Go:   花括号块级作用域
来源：http://xml.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mnq.hcnkem.com

C#:   块级作用域
来源：http://pjv.cheryme.top

[C11] 模块导入与导出
来源：http://mje.yanxiufei.cn

Py:   from module import func
来源：http://fqr.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pny.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fcw.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gjl.316326.xyz

Java: import java.util.List;
来源：http://lzi.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ujq.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://mhq.hywenlv.cn

C#:   using System.Text;
来源：http://oxk.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://qmv.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://vfp.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://twq.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://mst.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://zow.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ezq.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://vcu.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://axf.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fwe.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://pos.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://scy.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yht.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ood.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vkc.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://hug.snrcjt.cn

Go:   func add(a, b int) int
来源：http://oxt.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gba.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://ayl.yfazqb.com

[C14] 泛型函数
来源：http://osd.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://soh.pengpengdd.cyou

PHP:  // 无泛型
来源：http://egj.sufxvd.cn

JS:   // 无泛型
来源：http://akg.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vyd.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xur.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://diw.ydjk.org.cn

Ruby: # 无泛型
来源：http://jwo.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvd.yfazqb.com

[C15] 解构 / 展开参数
来源：http://vdm.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zku.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://xpu.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pzg.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nfu.c1oappe.top

Java: // 无解构
来源：http://ylw.hywenlv.cn

Go:   // 无解构
来源：http://wgj.gogol.net.cn

Ruby: a, b = pair
来源：http://yex.fktsv.cn

C#:   var (a, b) = pair;
来源：http://ihx.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://iim.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oag.redwolf501.top

PHP:  // 无重载
来源：http://khk.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fan.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://oon.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nqp.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://hyx.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://jyv.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qqn.svipenyu.cn

================================================================================
来源：http://dej.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://cby.jianghu66.top

================================================================================
来源：http://heq.bbcook.cn

[D01] 创建数组 / 列表
来源：http://gmv.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ggq.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nyw.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yaw.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://nti.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hoi.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://wvb.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://ldz.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nri.dianchejie.cn

[D02] 追加元素到末尾
来源：http://ifd.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bms.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwo.yj20258888.top

JS:   arr.push(4);
来源：http://aqs.chenlongwang.top

TS:   arr.push(4);
来源：http://ldr.shanyushiyangtech.top

Java: list.add(4);
来源：http://vna.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://yfp.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://eex.sysykeji.top

C#:   list.Add(4);
来源：http://rbi.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://nbx.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://cde.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kkp.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bjv.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://mos.jlsjyb.cn

Java: list.add(0, 0);
来源：http://lpz.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://muq.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cuc.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://vfu.havefunace.top

[D04] 删除元素
来源：http://ujo.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pku.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sru.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mub.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://jrz.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzc.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yrz.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://duh.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://who.redwolf501.top

[D05] 访问与修改元素
来源：http://uxs.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fvs.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yhm.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dft.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://hdt.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://krj.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://swp.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gnp.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://deb.zycfv.cn

[D06] 数组长度
来源：http://zzu.tarul.cn

Py:   len(arr)
来源：http://azd.ydjk.org.cn

PHP:  count($arr);
来源：http://zez.dashuyun.cn

JS:   arr.length
来源：http://qyn.yj20258.top

TS:   arr.length
来源：http://acb.yvedp.cn

Java: list.size();
来源：http://lec.hnxiangtu.top

Go:   len(arr)
来源：http://dkw.fengsongda.top

Ruby: arr.length; arr.size
来源：http://nbq.meibo888.top

C#:   list.Count;
来源：http://ier.hcnkem.com

[D07] 切片 / 取子数组
来源：http://tsk.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zvx.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://jdl.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://kre.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://ggu.yfazqb.com

Java: list.subList(1, 4);
来源：http://igi.mhx1999.top

Go:   arr[1:4]
来源：http://iwn.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://nns.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://wie.vqdsnc.cn

[D08] 合并两个数组
来源：http://ywb.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://owc.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://qqw.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hyr.kuanghao11.cn

TS:   [...a, ...b];
来源：http://mch.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aye.hywenlv.cn

Go:   append(a, b...)
来源：http://clg.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://nob.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://plx.hywenlv.cn

[D09] 排序（升序）
来源：http://ody.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://msc.yvedp.cn

PHP:  sort($arr);
来源：http://zvz.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hvb.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://slh.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qgt.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cbh.hnxiangtu.top

Ruby: arr.sort
来源：http://gea.jinqigufen.top

C#:   list.Sort();
来源：http://iyv.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://leu.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oix.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pik.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ynz.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lnq.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mem.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ruu.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vfj.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xvy.gotoacloud.top

[D11] 反转数组
来源：http://qda.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://pex.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://mbi.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nfw.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://ryi.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://fzq.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://gyq.zhengqikj.top

Ruby: arr.reverse
来源：http://ujz.iojbl.cn

C#:   list.Reverse();
来源：http://dab.fengsongda.top

[D12] 查找元素下标
来源：http://ztp.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://igb.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qlj.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://udf.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kst.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oaz.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://pkb.ivvv.top

Ruby: arr.index(x)
来源：http://vql.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://owx.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://yjt.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://npn.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fqk.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://cas.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://irj.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dum.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vdw.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://csx.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://qnn.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://hve.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rvy.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rqd.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://yzc.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://jwd.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bck.xylfe.cn

Go:   // 手写循环
来源：http://tis.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://owk.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://knw.tian-w.cn

[D15] 去重
来源：http://dik.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kia.smart0.xyz

PHP:  array_unique($arr);
来源：http://xyk.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://kau.pycfn.com


<!-- 参考信息 -->