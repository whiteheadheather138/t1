代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://ynp.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tei.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qcr.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://dsz.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://flr.iojbl.cn

[C03] 可变参数
来源：http://iae.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://nlw.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xaf.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://spq.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xzz.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://onu.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ooo.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://gxu.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cmj.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://akm.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xfw.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bgw.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gfd.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ezv.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://off.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://iyj.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://jbp.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://fem.xylfe.cn

[C05] 返回多个值
来源：http://bzw.jyoumei.cn

Py:   return a, b
来源：http://bdx.snrcjt.cn

PHP:  return [$a, $b];
来源：http://rpd.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://who.bbcook.cn

TS:   return { a, b };
来源：http://vtb.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bsy.pycfn.com

Go:   return a, b
来源：http://deb.yangfankeji.com

Ruby: return a, b
来源：http://zdz.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://utc.pycfn.com

[C06] 匿名函数 / lambda
来源：http://oxp.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://iub.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zvt.hammf.cn

JS:   const square = x => x * x;
来源：http://tfy.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://hsj.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aoa.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://dtg.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://erk.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dyw.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://llz.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pca.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hsi.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cel.shanyushiyangtech.top

TS:   arr.map(String)
来源：http://srg.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://osm.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lso.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://itz.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kxx.shuidangran.top

[C08] 闭包
来源：http://gtw.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojl.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nvw.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://elp.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tmk.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hwi.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fkr.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uen.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ubm.hfpthk.cn

[C09] 递归
来源：http://hfm.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bfz.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wln.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ngd.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gku.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfr.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vlc.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mlk.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ryf.fengsongda.top

[C10] 变量作用域
来源：http://uaw.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://amd.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mzb.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nyt.yueranfly.top

TS:   同 JS
来源：http://zlw.c1oappe.top

Java: 方法内为块级作用域
来源：http://qte.guowangkeji.top

Go:   花括号块级作用域
来源：http://qfr.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nue.0kj1m.cn

C#:   块级作用域
来源：http://sxg.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://yay.daxiang520.top

Py:   from module import func
来源：http://vzu.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iit.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iqn.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hdf.gaohongyu789.top

Java: import java.util.List;
来源：http://zqy.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cso.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://zhv.yuanzhike.top

C#:   using System.Text;
来源：http://okd.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://anx.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://gkg.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://tsk.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://tuq.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://lyl.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rol.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://lho.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://gpb.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://dyk.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://ytt.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fbh.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mjv.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iom.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vpd.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://grh.wangdashe.top

Go:   func add(a, b int) int
来源：http://xmh.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ntk.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://lmo.9152youxi.cn

[C14] 泛型函数
来源：http://sdk.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uau.shangyingyoupin.top

PHP:  // 无泛型
来源：http://grt.sysykeji.top

JS:   // 无泛型
来源：http://pat.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bkq.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wot.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uls.yj202588.top

Ruby: # 无泛型
来源：http://nba.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nvt.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://kbt.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://psn.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://mll.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://abn.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gaf.yanxiufei.cn

Java: // 无解构
来源：http://nif.smart0.xyz

Go:   // 无解构
来源：http://etv.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://suv.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://wvm.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://lfu.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fok.yueranfly.top

PHP:  // 无重载
来源：http://bly.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://kma.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://fqz.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://sbo.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://uov.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://ejm.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://uwu.yfazqb.com

================================================================================
来源：http://iaa.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://fsz.ywan-chungtsiang.top

================================================================================
来源：http://zrn.daria6918.cn

[D01] 创建数组 / 列表
来源：http://tal.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://snk.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mqz.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gix.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dpx.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bdr.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://ntc.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://qwy.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ahy.yvedp.cn

[D02] 追加元素到末尾
来源：http://ijw.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ovd.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uxj.jianghu66.top

JS:   arr.push(4);
来源：http://smb.sweek.top

TS:   arr.push(4);
来源：http://ijr.fehbvm.com

Java: list.add(4);
来源：http://wkx.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://zoe.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://pvj.dianchejie.cn

C#:   list.Add(4);
来源：http://zsu.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://kjg.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://ktg.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lfe.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://giq.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://bfe.aizwys.cn

Java: list.add(0, 0);
来源：http://kbb.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://puo.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fuy.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://vvd.jyoumei.cn

[D04] 删除元素
来源：http://nez.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jyx.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ftr.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnv.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://iuv.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wqm.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cpj.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hnt.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yoe.hysaishi.cn

[D05] 访问与修改元素
来源：http://ykp.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ftw.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nnn.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iju.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://bxa.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://xql.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://kia.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jou.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rni.gaohongyu789.top

[D06] 数组长度
来源：http://zbx.shuidangran.top

Py:   len(arr)
来源：http://ghd.mhx1999.top

PHP:  count($arr);
来源：http://drs.hongshengwenyu.top

JS:   arr.length
来源：http://sye.sufxvd.cn

TS:   arr.length
来源：http://xpv.cdnleiting.top

Java: list.size();
来源：http://bcp.tianlin.xyz

Go:   len(arr)
来源：http://lkk.yueranfly.top

Ruby: arr.length; arr.size
来源：http://dvw.jiagoushi.top

C#:   list.Count;
来源：http://gow.tian-w.cn

[D07] 切片 / 取子数组
来源：http://zum.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mju.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://jpm.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://lhk.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://hxd.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://vrk.hnxiangtu.top

Go:   arr[1:4]
来源：http://fcx.yvedp.cn

Ruby: arr[1, 3]
来源：http://vsl.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://hje.hesvh.cn

[D08] 合并两个数组
来源：http://qat.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://qic.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://owb.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://khk.smart0.xyz

TS:   [...a, ...b];
来源：http://ogp.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cpi.yuanzhike.top

Go:   append(a, b...)
来源：http://tfd.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://qnl.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://qph.nwbrower.top

[D09] 排序（升序）
来源：http://jte.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://zig.jyoumei.cn

PHP:  sort($arr);
来源：http://lui.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iim.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kuz.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lcj.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kfv.yj20258888.top

Ruby: arr.sort
来源：http://prf.bjfxy.top

C#:   list.Sort();
来源：http://xqz.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rvn.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iyu.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwu.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvo.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzj.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wuc.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wiw.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ydi.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbs.hywenlv.cn

[D11] 反转数组
来源：http://ykj.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://igc.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://ckg.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bkf.yonumen.top

TS:   [...arr].reverse();
来源：http://gtr.nanxinkj.top

Java: Collections.reverse(list);
来源：http://pgd.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://npe.hywenlv.cn

Ruby: arr.reverse
来源：http://cmq.hfpthk.cn

C#:   list.Reverse();
来源：http://jbc.sxryk.cn

[D12] 查找元素下标
来源：http://old.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://fik.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ron.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hmy.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cdy.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aga.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://irr.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://izw.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://cwm.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://etg.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vlf.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mdf.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://xgu.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://rkp.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://agk.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://crb.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://rxu.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://oal.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://eoz.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://msr.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tgq.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://uht.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://gyd.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xgl.gaohongyu789.top

Go:   // 手写循环
来源：http://pgp.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hjb.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pmy.tanke756.top

[D15] 去重
来源：http://lwa.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gof.xuanzx.com

PHP:  array_unique($arr);
来源：http://bmx.guannengcc.top

JS:   [...new Set(arr)]
来源：http://yko.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://nim.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zmu.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://yib.fengsongda.top

Ruby: arr.uniq
来源：http://hyl.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://nkg.bjfxy.top

[D16] 求和与平均值
来源：http://vuu.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yfy.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://seo.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tsd.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tby.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://abl.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://fyo.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://skd.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://jsq.vehdjk.com

[D17] 最大值与最小值
来源：http://jdk.yonumen.top

Py:   max(arr);  min(arr)
来源：http://ifp.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://ubo.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vwz.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://cuf.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://evh.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vhd.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://gto.tarul.cn

C#:   list.Max();  list.Min()
来源：http://caa.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://btg.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://teo.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://rni.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tfs.quarkkingdee.top

TS:   nested.flat();
来源：http://oft.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehz.xziqi.cn

Go:   // 手写双层循环
来源：http://cbp.zdbjq.cn

Ruby: nested.flatten
来源：http://mod.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhh.fehbvm.com

[D19] 按字段分组
来源：http://ukh.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cjz.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rlh.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xkv.yonumen.top


<!-- 参考信息 -->