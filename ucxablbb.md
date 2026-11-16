代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://ctu.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ffr.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mxw.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://bsg.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://wli.bbcook.cn

[C03] 可变参数
来源：http://xaw.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://lwe.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zrr.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozr.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sqw.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tdn.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gkx.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gma.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hwr.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://mry.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckk.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dyb.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hrp.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ioo.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://ocw.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://txe.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://orw.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://gne.hesvh.cn

[C05] 返回多个值
来源：http://cgh.vqdsnc.cn

Py:   return a, b
来源：http://ugy.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://ood.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rkp.hammf.cn

TS:   return { a, b };
来源：http://eji.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ozj.ydzc1.top

Go:   return a, b
来源：http://ipr.zhengqikj.top

Ruby: return a, b
来源：http://rpp.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://lmo.tarul.cn

[C06] 匿名函数 / lambda
来源：http://szo.hcnkem.com

Py:   square = lambda x: x * x
来源：http://xhw.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ivs.zhixingplan.top

JS:   const square = x => x * x;
来源：http://tnk.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://wod.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://web.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://omy.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://dwd.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://hiz.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://wor.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mfy.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tab.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://obb.xuanzx.com

TS:   arr.map(String)
来源：http://jck.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vdf.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nvp.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://cto.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://toe.shanyushiyangtech.top

[C08] 闭包
来源：http://qru.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kre.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://quc.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sol.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mnm.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ori.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tog.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://brj.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpo.xuanzx.com

[C09] 递归
来源：http://kan.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ckk.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uvu.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpt.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wxf.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bde.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wfe.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://scd.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dlg.wangdashe.top

[C10] 变量作用域
来源：http://aki.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ksj.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gdr.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yfn.fktsv.cn

TS:   同 JS
来源：http://yoq.zdqjudy.top

Java: 方法内为块级作用域
来源：http://dwn.9152youxi.cn

Go:   花括号块级作用域
来源：http://eyd.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fqj.aizwys.cn

C#:   块级作用域
来源：http://rtf.mhx1999.top

[C11] 模块导入与导出
来源：http://oyn.yuanzhike.top

Py:   from module import func
来源：http://hqh.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://xvx.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nvt.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lcj.fehbvm.com

Java: import java.util.List;
来源：http://jyh.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmu.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://qps.sjlbkw.cn

C#:   using System.Text;
来源：http://bag.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://ctl.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://tdv.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://rce.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://qfc.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://mth.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nwh.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://bzs.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://vee.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vlh.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://hjf.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gva.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://byl.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mbm.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vfa.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wgc.sufxvd.cn

Go:   func add(a, b int) int
来源：http://ezo.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://avj.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://wok.hysaishi.cn

[C14] 泛型函数
来源：http://fpx.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uno.dashuyun.cn

PHP:  // 无泛型
来源：http://xqo.cqqwz.cn

JS:   // 无泛型
来源：http://vaf.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lbn.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jlk.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvh.hammf.cn

Ruby: # 无泛型
来源：http://nwc.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://htf.52xcode.cn

[C15] 解构 / 展开参数
来源：http://hqc.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ajh.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://agp.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qvq.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pgm.fehbvm.com

Java: // 无解构
来源：http://hjg.zhiwuduotai.top

Go:   // 无解构
来源：http://gsi.nanxinkj.top

Ruby: a, b = pair
来源：http://tcw.yuxming.cn

C#:   var (a, b) = pair;
来源：http://vdo.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://snn.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bfe.sxryk.cn

PHP:  // 无重载
来源：http://zsw.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vff.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://lat.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rzb.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://zuw.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://uxr.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://otj.jianghu66.top

================================================================================
来源：http://jlu.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://pxc.yueranfly.top

================================================================================
来源：http://naa.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://qbk.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ptg.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://onh.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uif.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cfz.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://afp.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://ohr.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://emy.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://meo.cdnleiting.top

[D02] 追加元素到末尾
来源：http://tcf.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://opw.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://poq.shuidangran.top

JS:   arr.push(4);
来源：http://niw.ehwqpu.com

TS:   arr.push(4);
来源：http://rwm.dashuyun.cn

Java: list.add(4);
来源：http://ucm.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://nrp.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://hyj.xylfe.cn

C#:   list.Add(4);
来源：http://sil.pycfn.com

[D03] 在指定位置插入元素
来源：http://dto.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://xxh.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eci.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yuq.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://hgk.zdqjudy.top

Java: list.add(0, 0);
来源：http://fcq.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://gzy.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gge.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://wcu.nwbrower.top

[D04] 删除元素
来源：http://sia.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzg.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://odl.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oez.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://uyq.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iso.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ywt.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfs.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vpo.vqdsnc.cn

[D05] 访问与修改元素
来源：http://zyd.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ypm.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mox.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vyr.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://vol.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://qtf.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://yps.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gxv.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vpo.shzxlz.cn

[D06] 数组长度
来源：http://fqr.ctjpmb.com

Py:   len(arr)
来源：http://sxy.jinghuilouyu.cn

PHP:  count($arr);
来源：http://mnf.gzhubu.top

JS:   arr.length
来源：http://dmt.yangfankeji.com

TS:   arr.length
来源：http://eft.jlsjyb.cn

Java: list.size();
来源：http://tyu.jinqigufen.top

Go:   len(arr)
来源：http://osv.vehdjk.com

Ruby: arr.length; arr.size
来源：http://oub.iojbl.cn

C#:   list.Count;
来源：http://tlk.shuidangran.top

[D07] 切片 / 取子数组
来源：http://uvo.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iwu.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vqd.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://psu.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://wnv.iojbl.cn

Java: list.subList(1, 4);
来源：http://amn.pycfn.com

Go:   arr[1:4]
来源：http://clz.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://kyp.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://tqo.cdnleiting.top

[D08] 合并两个数组
来源：http://btk.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://lpx.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://jpx.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://zew.vehdjk.com

TS:   [...a, ...b];
来源：http://jhi.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vop.zhiwuduotai.top

Go:   append(a, b...)
来源：http://niq.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://yxz.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://zaj.chenzaomai.com

[D09] 排序（升序）
来源：http://vql.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://yda.gotoacloud.top

PHP:  sort($arr);
来源：http://hvc.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gbu.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hlr.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mwt.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oft.jlsjyb.cn

Ruby: arr.sort
来源：http://veg.jqgfzy.top

C#:   list.Sort();
来源：http://qpe.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oar.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yje.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwg.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://beg.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://thl.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://arc.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vjb.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xav.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ppi.nwbrower.top

[D11] 反转数组
来源：http://vhv.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ida.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://bki.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rem.xinyue.icu

TS:   [...arr].reverse();
来源：http://psc.bjfxy.top

Java: Collections.reverse(list);
来源：http://hix.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://gjf.9152youxi.cn

Ruby: arr.reverse
来源：http://umt.yonumen.top

C#:   list.Reverse();
来源：http://dju.snrcjt.cn

[D12] 查找元素下标
来源：http://jdq.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://kjq.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrp.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpj.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbi.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ynj.316326.xyz

Go:   slices.Index(arr, x)
来源：http://vel.hcnkem.com

Ruby: arr.index(x)
来源：http://eeh.wangdashe.top

C#:   list.IndexOf(x);
来源：http://caq.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://vym.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuo.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kyq.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://zkh.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://ydv.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xfp.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kdx.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://inu.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vtb.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://pmy.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vqc.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hld.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://svt.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://eiy.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wry.dashuyun.cn

Go:   // 手写循环
来源：http://cvm.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://clg.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kgj.c1oappe.top

[D15] 去重
来源：http://mpb.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ugu.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://ujt.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://hiu.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://miv.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dbz.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hgd.iojbl.cn

Ruby: arr.uniq
来源：http://cca.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://lvl.chenjidiqi.icu

[D16] 求和与平均值
来源：http://ecy.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://juu.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tjt.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yga.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dnx.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://icl.hnqzz.top

Go:   // 手写循环累加
来源：http://sze.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pdb.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://ljc.cucudq.cn

[D17] 最大值与最小值
来源：http://qrf.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://yre.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://bhh.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cjg.hysaishi.cn

TS:   Math.max(...arr);
来源：http://rke.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ahs.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gdj.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://ups.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://ttx.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://kjg.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://flt.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://viw.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aqt.fehbvm.com

TS:   nested.flat();
来源：http://tob.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zcj.yfazqb.com

Go:   // 手写双层循环
来源：http://xmi.cdnleiting.top

Ruby: nested.flatten
来源：http://myy.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uhh.gogol.net.cn

[D19] 按字段分组
来源：http://kpz.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zlh.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tqp.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://coa.meibo888.top


<!-- 参考信息 -->