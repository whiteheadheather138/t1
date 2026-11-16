代发 wailian999

[C02] 默认参数
来源：http://jzy.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://hqs.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ymj.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hhj.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ajq.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ofi.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cad.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://xeq.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://vjc.sufxvd.cn

[C03] 可变参数
来源：http://npx.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://lun.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rni.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tii.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upk.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mil.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rzz.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://blq.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lmc.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://zpa.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://deq.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tyi.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oov.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fog.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://rxr.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://fwv.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://hpv.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://xrb.gogol.net.cn

[C05] 返回多个值
来源：http://upq.xziqi.cn

Py:   return a, b
来源：http://vkc.mhx1999.top

PHP:  return [$a, $b];
来源：http://vcb.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fqt.ydjk.org.cn

TS:   return { a, b };
来源：http://klq.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jhe.ydzc1.top

Go:   return a, b
来源：http://pah.tian-w.cn

Ruby: return a, b
来源：http://cth.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://sdh.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://izo.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://sdo.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wog.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://rcc.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://vrc.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bir.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://htm.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://sjj.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://owr.hcnkem.com

[C07] 把函数作为参数传入
来源：http://qsi.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xjn.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://fnb.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jda.ydjk.org.cn

TS:   arr.map(String)
来源：http://yxs.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dwm.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rvx.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://qxv.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uvf.yuanzhike.top

[C08] 闭包
来源：http://apf.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://adb.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oiu.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://etg.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://olu.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tws.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gvz.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eyq.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rvr.c1oappe.top

[C09] 递归
来源：http://dwt.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fxd.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fls.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://veg.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pbb.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wyn.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uto.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cip.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxj.zhixingplan.top

[C10] 变量作用域
来源：http://kqf.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pfm.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tsi.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofk.52xcode.cn

TS:   同 JS
来源：http://zgi.jianghu66.top

Java: 方法内为块级作用域
来源：http://ayh.fzhhl.top

Go:   花括号块级作用域
来源：http://xek.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wbi.aibaodan.cn

C#:   块级作用域
来源：http://ggm.ivvv.top

[C11] 模块导入与导出
来源：http://xxr.sufxvd.cn

Py:   from module import func
来源：http://vjq.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://grv.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hnh.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hms.gotoacloud.top

Java: import java.util.List;
来源：http://jyg.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eax.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://kyo.yj20258.top

C#:   using System.Text;
来源：http://jae.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://bhn.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://irw.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://isp.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://rlk.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://mgo.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jju.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://xxj.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://kti.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tqi.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://uve.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mui.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://djn.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://azk.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lvi.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://avw.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://iub.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ffe.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fkf.fanxiaobao.xyz

[C14] 泛型函数
来源：http://qoo.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dco.316326.xyz

PHP:  // 无泛型
来源：http://jcg.ivvv.top

JS:   // 无泛型
来源：http://tie.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pqu.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ais.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yfx.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://eje.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dln.gzhubu.top

[C15] 解构 / 展开参数
来源：http://jow.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jfs.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://sek.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://itu.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jdz.zycfv.cn

Java: // 无解构
来源：http://yap.vqdsnc.cn

Go:   // 无解构
来源：http://bbv.gaohongyu789.top

Ruby: a, b = pair
来源：http://ucx.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://dwp.ybcxt.top

[C16] 函数 / 方法重载
来源：http://ibs.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dcq.ybcxt.top

PHP:  // 无重载
来源：http://ura.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lke.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://bky.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ijp.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://fce.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://vez.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ekd.zhixingplan.top

================================================================================
来源：http://shx.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://fmh.jlsjyb.cn

================================================================================
来源：http://xcp.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://xnt.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://twf.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://inx.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xee.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xtt.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sky.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://nhq.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://lnz.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bnu.meibo888.top

[D02] 追加元素到末尾
来源：http://yky.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://phw.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nxn.haohaochexian.top

JS:   arr.push(4);
来源：http://dlg.sysykeji.top

TS:   arr.push(4);
来源：http://ijm.tianlin.xyz

Java: list.add(4);
来源：http://bcy.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://wtl.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://umr.zhixingplan.top

C#:   list.Add(4);
来源：http://wmu.xylfe.cn

[D03] 在指定位置插入元素
来源：http://toa.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://pbf.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jlo.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kpr.ybcxt.top

TS:   arr.splice(0, 0, 0);
来源：http://bnt.haohaochexian.top

Java: list.add(0, 0);
来源：http://vuh.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://utn.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qbq.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://ybx.gogol.net.cn

[D04] 删除元素
来源：http://vuu.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxs.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fej.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mbg.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://coy.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fjn.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wvb.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dck.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rfe.ivvv.top

[D05] 访问与修改元素
来源：http://xgc.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvp.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://spp.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vcl.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://fny.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://nvm.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://tpu.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ifg.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jao.meibo888.top

[D06] 数组长度
来源：http://kcw.zhongyouzk.top

Py:   len(arr)
来源：http://sul.yongpay.top

PHP:  count($arr);
来源：http://nwk.meibo888.top

JS:   arr.length
来源：http://dhr.jinyuanbaomall.cn

TS:   arr.length
来源：http://hke.jinyuanbaomall.cn

Java: list.size();
来源：http://rpy.bjfxy.top

Go:   len(arr)
来源：http://fpw.yongpay.top

Ruby: arr.length; arr.size
来源：http://xpc.quarkkingdee.top

C#:   list.Count;
来源：http://nbl.yj20258888.top

[D07] 切片 / 取子数组
来源：http://blo.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wtz.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://axu.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://tex.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://oip.tanke756.top

Java: list.subList(1, 4);
来源：http://xao.hnxiangtu.top

Go:   arr[1:4]
来源：http://ctv.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://rqi.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://tyk.kuanghao11.cn

[D08] 合并两个数组
来源：http://cmf.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://asy.tanke756.top

PHP:  array_merge($a, $b);
来源：http://wcw.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qnr.birdmap.top

TS:   [...a, ...b];
来源：http://dmo.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fge.shuidangran.top

Go:   append(a, b...)
来源：http://sxy.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://dgt.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://vfa.cheryme.top

[D09] 排序（升序）
来源：http://cpx.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://hxi.gaohongyu789.top

PHP:  sort($arr);
来源：http://jtk.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lws.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xvw.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://otl.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hll.zdqjudy.top

Ruby: arr.sort
来源：http://ega.yonumen.top

C#:   list.Sort();
来源：http://wjm.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ezb.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oxe.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdd.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxa.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdz.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pqs.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rpm.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lth.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vej.hnxiangtu.top

[D11] 反转数组
来源：http://kmv.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://zhf.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://flj.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://upo.yangfankeji.com

TS:   [...arr].reverse();
来源：http://yky.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://wlu.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://ypm.svipenyu.cn

Ruby: arr.reverse
来源：http://hsg.hysaishi.cn

C#:   list.Reverse();
来源：http://pvy.jiagoushi.top

[D12] 查找元素下标
来源：http://bib.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://acq.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xbi.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://txx.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ckb.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uuj.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://nnh.gzhubu.top

Ruby: arr.index(x)
来源：http://nxp.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://cpz.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://wev.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tgw.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zls.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://qnj.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://ztn.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfn.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ayf.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://qce.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://geu.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://ttv.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aad.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sku.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://vrj.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://xow.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://iuc.hnqzz.top

Go:   // 手写循环
来源：http://hgb.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://ilu.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sbq.andypj.xyz

[D15] 去重
来源：http://idv.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jzy.xuanzx.com

PHP:  array_unique($arr);
来源：http://qxt.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://ryc.shuidangran.top

TS:   [...new Set(arr)]
来源：http://wld.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mxc.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zfw.cqqwz.cn

Ruby: arr.uniq
来源：http://crp.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://mch.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://rfz.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uyc.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fti.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://deu.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://irv.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hbg.yfazqb.com

Go:   // 手写循环累加
来源：http://bjn.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dhw.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://xvh.daxiang520.top

[D17] 最大值与最小值
来源：http://hia.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://onu.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://iib.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://htn.yueranfly.top

TS:   Math.max(...arr);
来源：http://vrs.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jge.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqs.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://ftk.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://ngl.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://hch.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yzc.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://vna.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tnf.zhixingplan.top

TS:   nested.flat();
来源：http://bqz.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uxn.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://esj.yonumen.top

Ruby: nested.flatten
来源：http://mgt.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bpw.haohaochexian.top


<!-- 参考信息 -->