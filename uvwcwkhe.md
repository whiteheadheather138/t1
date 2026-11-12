代发 wailian999

PHP:  $a && $b || !$c
来源：http://xbe.cqqwz.cn

JS:   a && b || !c
来源：http://vco.wangshuangyany.cn

TS:   a && b || !c
来源：http://olr.yvedp.cn

Java: a && b || !c
来源：http://gqp.andypj.xyz

Go:   a && b || !c
来源：http://qhx.yj20258888.top

Ruby: a && b || !c
来源：http://mjt.dashuyun.cn

C#:   a && b || !c
来源：http://dlu.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://brv.aibaodan.cn

Py:   if not data: return
来源：http://bme.cheryme.top

PHP:  if (!$data) { return; }
来源：http://axp.mhx1999.top

JS:   if (!data) return;
来源：http://snx.jinqigfzy.top

TS:   if (!data) return;
来源：http://cpp.daxiang520.top

Java: if (data == null) return;
来源：http://deb.meibo888.top

Go:   if data == nil { return }
来源：http://drv.birdmap.top

Ruby: return if data.nil?
来源：http://pcg.hesvh.cn

C#:   if (data == null) return;
来源：http://mif.cdnleiting.top

================================================================================
来源：http://spl.zdbjq.cn

C. 函数与作用域
来源：http://qli.yongpay.top

================================================================================
来源：http://jqp.shanyushiyangtech.top

[C01] 定义函数
来源：http://sfx.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://ksj.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uzl.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://vsy.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bol.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tdz.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://kav.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://kki.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sww.nanxinkj.top

[C02] 默认参数
来源：http://aoi.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://brw.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iah.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://jwa.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://grc.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nis.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bta.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://fxi.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://cmz.xuetiantiany.cn

[C03] 可变参数
来源：http://prl.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://vaa.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://odo.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nre.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://knz.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ljk.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wrr.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://fix.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pgt.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://fua.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uwc.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ynb.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qfg.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ant.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zzu.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://wao.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://sds.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://ohi.cashguo.top

[C05] 返回多个值
来源：http://thv.9152youxi.cn

Py:   return a, b
来源：http://khw.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://nam.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://apl.jinghuilouyu.cn

TS:   return { a, b };
来源：http://gml.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://atk.sweek.top

Go:   return a, b
来源：http://ebr.gogol.net.cn

Ruby: return a, b
来源：http://xpa.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://sxs.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://fdk.ivvv.top

Py:   square = lambda x: x * x
来源：http://mgm.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://amq.tian-w.cn

JS:   const square = x => x * x;
来源：http://yaq.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://bkt.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jkc.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://fbc.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://mwt.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://bmt.andypj.xyz

[C07] 把函数作为参数传入
来源：http://cyp.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ilv.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://mzv.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kjj.jiagoushi.top

TS:   arr.map(String)
来源：http://yky.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qno.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zti.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://ggo.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eqm.yj20258888.top

[C08] 闭包
来源：http://yvr.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://myd.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cyd.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wkk.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jyo.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://drf.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ata.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://olz.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://woi.zhiwuduotai.top

[C09] 递归
来源：http://zgd.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://umf.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tff.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bdc.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tmp.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hxh.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gve.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mnc.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tob.wangdashe.top

[C10] 变量作用域
来源：http://ylc.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ori.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://znm.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zqw.hfpthk.cn

TS:   同 JS
来源：http://cds.hnqzz.top

Java: 方法内为块级作用域
来源：http://jok.cdnleiting.top

Go:   花括号块级作用域
来源：http://xcq.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://smu.tanke756.top

C#:   块级作用域
来源：http://elv.haohaochexian.top

[C11] 模块导入与导出
来源：http://tme.bbcook.cn

Py:   from module import func
来源：http://uqs.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dxv.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hmh.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xdf.zdqjudy.top

Java: import java.util.List;
来源：http://rsp.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://edq.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://tbi.sufxvd.cn

C#:   using System.Text;
来源：http://dej.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://eui.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://djb.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://owg.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://hwd.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://fan.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lky.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://rij.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://rrz.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://gld.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://bqc.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vqj.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://som.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dzc.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wfx.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://xlp.jiagoushi.top

Go:   func add(a, b int) int
来源：http://vgn.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syj.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://xon.nanxinkj.top

[C14] 泛型函数
来源：http://iwe.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utf.pengpengdd.cyou

PHP:  // 无泛型
来源：http://miw.kuanghao11.cn

JS:   // 无泛型
来源：http://pvw.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qvr.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zan.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://onk.0kj1m.cn

Ruby: # 无泛型
来源：http://hul.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ioo.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://vpx.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://paw.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://pjr.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tte.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xec.dashuyun.cn

Java: // 无解构
来源：http://czb.zhixingplan.top

Go:   // 无解构
来源：http://ekw.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://jul.guannengcc.top

C#:   var (a, b) = pair;
来源：http://vwj.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://yno.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://etm.yanxiufei.cn

PHP:  // 无重载
来源：http://gcf.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rtv.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://npx.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kzs.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://ykk.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://fdd.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://pxc.gaohongyu789.top

================================================================================
来源：http://vyd.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://mat.zhiwuduotai.top

================================================================================
来源：http://cey.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://rjn.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wlg.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oyg.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yun.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yst.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ngn.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://zuo.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://hdo.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://its.bbcook.cn

[D02] 追加元素到末尾
来源：http://dhc.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dml.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kdx.iojbl.cn

JS:   arr.push(4);
来源：http://tpm.birdmap.top

TS:   arr.push(4);
来源：http://yoy.zhijiandao.cn

Java: list.add(4);
来源：http://tka.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://chu.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://bvj.cqqwz.cn

C#:   list.Add(4);
来源：http://frd.sxryk.cn

[D03] 在指定位置插入元素
来源：http://gbv.pycfn.com

Py:   arr.insert(0, 0)
来源：http://emq.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qfw.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qyb.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://pml.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://gar.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://grr.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nbw.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://qtu.jyoumei.cn

[D04] 删除元素
来源：http://ybx.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://trf.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qup.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gts.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://jjk.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bhf.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mye.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yxo.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zmk.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://bul.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://grq.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jdm.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jix.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://ans.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://ejx.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://zpp.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ido.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lwt.hnxiangtu.top

[D06] 数组长度
来源：http://rfe.yj202588.top

Py:   len(arr)
来源：http://kba.meibo888.top

PHP:  count($arr);
来源：http://uix.fehbvm.com

JS:   arr.length
来源：http://awi.jinqigfzy.top

TS:   arr.length
来源：http://czs.tianlin.xyz

Java: list.size();
来源：http://xlk.nwbrower.top

Go:   len(arr)
来源：http://gwe.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://ype.aizwys.cn

C#:   list.Count;
来源：http://nwy.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://bqu.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqm.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://uyi.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://uxp.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://rjl.0kj1m.cn

Java: list.subList(1, 4);
来源：http://rgr.yfazqb.com

Go:   arr[1:4]
来源：http://fpi.iojbl.cn

Ruby: arr[1, 3]
来源：http://wau.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://uxh.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://vkb.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://ykp.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://gqh.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zdj.yfazqb.com

TS:   [...a, ...b];
来源：http://wgw.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cvy.bjfxy.top

Go:   append(a, b...)
来源：http://omj.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://fmy.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://byo.yangfankeji.com

[D09] 排序（升序）
来源：http://jbo.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kew.vehdjk.com

PHP:  sort($arr);
来源：http://ymd.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://woh.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zkb.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nlb.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cvv.gotoacloud.top

Ruby: arr.sort
来源：http://zsc.sjlbkw.cn

C#:   list.Sort();
来源：http://tfw.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://skf.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://icw.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ydx.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pco.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ita.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lmq.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qjh.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hkz.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ngv.vehdjk.com

[D11] 反转数组
来源：http://fmz.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uow.mhx1999.top

PHP:  array_reverse($arr);
来源：http://txu.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zre.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://qhx.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://feq.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://gse.pengpengdd.cyou

Ruby: arr.reverse
来源：http://jot.hesvh.cn

C#:   list.Reverse();
来源：http://qzi.epnwcf.com

[D12] 查找元素下标
来源：http://ijs.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://jeo.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pcb.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vev.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ngc.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://apm.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://iaj.hfpthk.cn

Ruby: arr.index(x)
来源：http://qpb.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://dex.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://syx.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dhv.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hvl.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://win.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://igt.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://odh.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mgb.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://lss.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xiz.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://lca.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uaw.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ype.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://lzw.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://dhy.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zbl.hywenlv.cn

Go:   // 手写循环
来源：http://lyl.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://yxd.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tmw.gaohongyu789.top

[D15] 去重
来源：http://lcl.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cqb.jyoumei.cn

PHP:  array_unique($arr);
来源：http://joc.cucudq.cn

JS:   [...new Set(arr)]
来源：http://oyv.shuidangran.top

TS:   [...new Set(arr)]
来源：http://vhx.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://khk.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://hxp.uphjek.com

Ruby: arr.uniq
来源：http://xcr.ydzc1.top


<!-- 参考信息 -->