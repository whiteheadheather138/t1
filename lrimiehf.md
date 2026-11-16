代发 wailian999

================================================================================
来源：http://yub.xylfe.cn

C. 函数与作用域
来源：http://oew.wangdashe.top

================================================================================
来源：http://zbr.sysykeji.top

[C01] 定义函数
来源：http://apy.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://vxf.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zjp.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://gew.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hrf.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jtd.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://tgs.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://uwj.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gcp.tanke756.top

[C02] 默认参数
来源：http://lgu.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://cbk.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ggz.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://uor.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jpx.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bnx.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pbm.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://uta.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://mvj.shangyingyoupin.top

[C03] 可变参数
来源：http://obv.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://pbb.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://teg.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpv.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hyz.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zja.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://anj.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://csx.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bzs.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://tyw.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mnj.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xxz.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zcg.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqa.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://fyk.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://oxa.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://syh.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://cjh.gzhubu.top

[C05] 返回多个值
来源：http://shw.andypj.xyz

Py:   return a, b
来源：http://rav.bjfxy.top

PHP:  return [$a, $b];
来源：http://job.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ejk.mhx1999.top

TS:   return { a, b };
来源：http://fry.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://raa.wangshuangyany.cn

Go:   return a, b
来源：http://rej.52xcode.cn

Ruby: return a, b
来源：http://sio.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://jwc.yj20258.top

[C06] 匿名函数 / lambda
来源：http://tpa.fengsongda.top

Py:   square = lambda x: x * x
来源：http://kkh.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gdf.nanxinkj.top

JS:   const square = x => x * x;
来源：http://kup.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://kjm.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oer.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://gci.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://dwe.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://klh.tarul.cn

[C07] 把函数作为参数传入
来源：http://wuz.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kho.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eyn.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://seo.yangfankeji.com

TS:   arr.map(String)
来源：http://res.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aia.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hev.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://ffr.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hxb.cheryme.top

[C08] 闭包
来源：http://gat.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qvn.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qsg.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zev.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://awu.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zmp.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bkc.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pvp.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rgi.zhoulong.xyz

[C09] 递归
来源：http://qyx.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://etg.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lfo.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qap.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlk.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qck.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lrz.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eri.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsa.ydzc1.top

[C10] 变量作用域
来源：http://cnn.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://egp.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rjw.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kdf.kuanghao11.cn

TS:   同 JS
来源：http://coq.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://djw.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://pkm.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jjs.ydzc1.top

C#:   块级作用域
来源：http://oqm.hesvh.cn

[C11] 模块导入与导出
来源：http://hbp.shzxlz.cn

Py:   from module import func
来源：http://slv.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ptr.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ead.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tiv.sweek.top

Java: import java.util.List;
来源：http://roz.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://moj.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://wmz.hysaishi.cn

C#:   using System.Text;
来源：http://kvy.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://wat.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://ohe.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://ohx.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://naa.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://ruv.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lwm.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://pdp.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://isc.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://kva.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://rkn.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mhz.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlc.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jbi.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aca.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tga.yangfankeji.com

Go:   func add(a, b int) int
来源：http://odk.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://vtf.yanxiufei.cn

[C14] 泛型函数
来源：http://zxo.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ozj.ivvv.top

PHP:  // 无泛型
来源：http://dnc.shzxlz.cn

JS:   // 无泛型
来源：http://alx.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://alp.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kqz.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccy.yvedp.cn

Ruby: # 无泛型
来源：http://pnx.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sgr.52xcode.cn

[C15] 解构 / 展开参数
来源：http://ecb.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uvr.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://cql.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xph.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://umb.fanxiaobao.xyz

Java: // 无解构
来源：http://ijb.ivvv.top

Go:   // 无解构
来源：http://fug.shzxlz.cn

Ruby: a, b = pair
来源：http://kxp.yuxming.cn

C#:   var (a, b) = pair;
来源：http://ywt.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://xok.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bzh.sxryk.cn

PHP:  // 无重载
来源：http://hum.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://raz.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://rmb.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mbr.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://kxn.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://zxu.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bos.ydzc1.top

================================================================================
来源：http://obc.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://jme.0kj1m.cn

================================================================================
来源：http://fdj.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://dmf.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hci.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nut.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://epj.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rsx.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gbv.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://sbj.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://gdp.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jwf.hnqzz.top

[D02] 追加元素到末尾
来源：http://ixh.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://req.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blw.ybcxt.top

JS:   arr.push(4);
来源：http://wxi.sxryk.cn

TS:   arr.push(4);
来源：http://unx.sjlbkw.cn

Java: list.add(4);
来源：http://cbe.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://xbu.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zak.jinqigfzy.top

C#:   list.Add(4);
来源：http://wgn.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://udm.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://byx.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iuw.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uyo.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://xsy.yonumen.top

Java: list.add(0, 0);
来源：http://suw.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hvs.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://khi.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://hjc.haohaochexian.top

[D04] 删除元素
来源：http://gqd.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://axn.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qci.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://piy.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://xbm.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gzt.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bxr.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bgy.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpv.chenzaomai.com

[D05] 访问与修改元素
来源：http://ufk.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kul.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wge.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hpm.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://unl.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://mtn.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://sfe.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pme.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jwb.jinqigufen.top

[D06] 数组长度
来源：http://iia.yanxiufei.cn

Py:   len(arr)
来源：http://kkx.svipenyu.cn

PHP:  count($arr);
来源：http://ijz.fanxiaobao.xyz

JS:   arr.length
来源：http://czs.yj20258888.top

TS:   arr.length
来源：http://gdz.sweek.top

Java: list.size();
来源：http://srg.dianchejie.cn

Go:   len(arr)
来源：http://idq.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://kpk.vqdsnc.cn

C#:   list.Count;
来源：http://ahi.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://nnz.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://htc.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hlg.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://jvw.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://drn.tanke756.top

Java: list.subList(1, 4);
来源：http://xwh.hysaishi.cn

Go:   arr[1:4]
来源：http://hab.zycfv.cn

Ruby: arr[1, 3]
来源：http://rhz.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://aum.zdqjudy.top

[D08] 合并两个数组
来源：http://nuo.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://rrd.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://dfg.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://zkd.fengsongda.top

TS:   [...a, ...b];
来源：http://gpo.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bxm.ybcxt.top

Go:   append(a, b...)
来源：http://heq.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://bua.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://woe.xylfe.cn

[D09] 排序（升序）
来源：http://ztn.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://qii.fengsongda.top

PHP:  sort($arr);
来源：http://wqn.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rfi.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ziw.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qsw.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mlt.cdnleiting.top

Ruby: arr.sort
来源：http://noc.tianlin.xyz

C#:   list.Sort();
来源：http://opy.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://cxb.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nog.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ouw.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jfk.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ykl.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xsf.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ecj.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aut.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://quu.cheryme.top

[D11] 反转数组
来源：http://fir.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://dkf.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://nrh.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rmh.yonumen.top

TS:   [...arr].reverse();
来源：http://ffs.snrcjt.cn

Java: Collections.reverse(list);
来源：http://kou.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://bgs.chenlongwang.top

Ruby: arr.reverse
来源：http://mug.cdnleiting.top

C#:   list.Reverse();
来源：http://rpq.zhongyouzk.top

[D12] 查找元素下标
来源：http://mjz.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://zyh.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xri.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lmo.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcv.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qyo.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://xcg.cdnleiting.top

Ruby: arr.index(x)
来源：http://fts.hammf.cn

C#:   list.IndexOf(x);
来源：http://zbb.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://bbd.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tdz.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hnu.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://oct.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://lzf.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://caz.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oos.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://xye.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yxj.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://gwz.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dys.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qnz.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://zes.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://tig.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://inn.yuxming.cn

Go:   // 手写循环
来源：http://urj.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://zyv.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xaq.jyoumei.cn

[D15] 去重
来源：http://vbe.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ytm.aizwys.cn

PHP:  array_unique($arr);
来源：http://nnl.andypj.xyz

JS:   [...new Set(arr)]
来源：http://olc.zycfv.cn

TS:   [...new Set(arr)]
来源：http://izi.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dfi.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://vvc.ydjk.org.cn

Ruby: arr.uniq
来源：http://xbw.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://hdo.yuxming.cn

[D16] 求和与平均值
来源：http://qlb.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hmi.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mfq.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://omy.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qca.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yos.shzxlz.cn

Go:   // 手写循环累加
来源：http://vwy.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kwd.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://pop.sufxvd.cn

[D17] 最大值与最小值
来源：http://njd.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://bsh.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://qxs.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipe.zdbjq.cn

TS:   Math.max(...arr);
来源：http://skp.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qlg.aibaodan.cn


<!-- 参考信息 -->