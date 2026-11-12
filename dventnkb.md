代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://him.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ndn.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yhq.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://azi.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://jef.meibo888.top

[C03] 可变参数
来源：http://tdo.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://sch.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://opx.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kvl.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jek.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jzc.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hes.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://hgz.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pey.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://lnh.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zmv.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bjs.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xnn.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://owm.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://ypq.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://qqj.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://ocd.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://ryh.jyoumei.cn

[C05] 返回多个值
来源：http://gjn.yfazqb.com

Py:   return a, b
来源：http://yvn.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://euf.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oaa.snrcjt.cn

TS:   return { a, b };
来源：http://jks.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://crh.andypj.xyz

Go:   return a, b
来源：http://pdw.fanxiaobao.xyz

Ruby: return a, b
来源：http://bps.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://naf.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://qna.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://bpr.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cvh.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://pxa.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ybg.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://max.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://fic.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://new.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://ejg.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://jer.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tdp.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gsk.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://swx.guowangkeji.top

TS:   arr.map(String)
来源：http://cdy.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcd.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bfs.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://umm.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ssj.52xcode.cn

[C08] 闭包
来源：http://nfr.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://azp.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bug.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rbt.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://beb.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oie.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://elx.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://siz.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uya.chenlongwang.top

[C09] 递归
来源：http://fia.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kkr.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yte.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfd.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eek.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mgr.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ajw.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gey.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kbu.mhx1999.top

[C10] 变量作用域
来源：http://sqa.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bgx.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kwb.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jdz.ppjwa.cn

TS:   同 JS
来源：http://shu.fzhhl.top

Java: 方法内为块级作用域
来源：http://jmf.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://uxe.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cva.fktsv.cn

C#:   块级作用域
来源：http://yxa.ivvv.top

[C11] 模块导入与导出
来源：http://xsu.chenlongwang.top

Py:   from module import func
来源：http://ntf.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hdx.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qrq.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cpl.52xcode.cn

Java: import java.util.List;
来源：http://sbt.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kxs.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://uyc.sxryk.cn

C#:   using System.Text;
来源：http://vda.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://xzg.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://bel.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://nls.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://prh.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://ikj.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tcz.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://fvh.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://nyf.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gho.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://uub.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jgq.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dam.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vek.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://acg.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jvr.aizwys.cn

Go:   func add(a, b int) int
来源：http://pwl.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ncl.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://svk.ppjwa.cn

[C14] 泛型函数
来源：http://wbi.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ihr.ydzc1.top

PHP:  // 无泛型
来源：http://kra.chenlongwang.top

JS:   // 无泛型
来源：http://tmv.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hka.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fmf.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nwa.chenjidiqi.icu

Ruby: # 无泛型
来源：http://zof.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfw.bbcook.cn

[C15] 解构 / 展开参数
来源：http://php.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://imz.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://mvf.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bcn.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mgn.uphjek.com

Java: // 无解构
来源：http://trd.ctjpmb.com

Go:   // 无解构
来源：http://hux.yangfankeji.com

Ruby: a, b = pair
来源：http://tmh.xziqi.cn

C#:   var (a, b) = pair;
来源：http://kur.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://wca.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dzd.shanyushiyangtech.top

PHP:  // 无重载
来源：http://mmr.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://buo.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://bzv.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vgd.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://nqt.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://rjk.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fnq.xuetiantiany.cn

================================================================================
来源：http://ija.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://hvv.tian-w.cn

================================================================================
来源：http://myy.ivvv.top

[D01] 创建数组 / 列表
来源：http://lbd.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://nuu.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yum.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://adr.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://def.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xol.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://rrm.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://cko.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tlc.jianghu66.top

[D02] 追加元素到末尾
来源：http://gvm.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wio.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oar.daxiang520.top

JS:   arr.push(4);
来源：http://qsk.hysaishi.cn

TS:   arr.push(4);
来源：http://idj.tanke756.top

Java: list.add(4);
来源：http://fyr.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://ztk.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://jlz.52xcode.cn

C#:   list.Add(4);
来源：http://rel.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://tpy.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://efd.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://exd.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gxr.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://zgv.ehwqpu.com

Java: list.add(0, 0);
来源：http://dlv.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dwl.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://grl.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://drn.ctjpmb.com

[D04] 删除元素
来源：http://lat.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pur.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ron.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fyq.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://vhd.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ntg.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kwc.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aqh.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wzu.gotoacloud.top

[D05] 访问与修改元素
来源：http://jfj.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vus.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ceo.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xpj.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://jsn.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://kis.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://svr.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fkq.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eke.0kj1m.cn

[D06] 数组长度
来源：http://lzp.zhixingplan.top

Py:   len(arr)
来源：http://ykr.feifeiyinyue.top

PHP:  count($arr);
来源：http://eoc.yuanzhike.top

JS:   arr.length
来源：http://mxo.hammf.cn

TS:   arr.length
来源：http://sxc.fktsv.cn

Java: list.size();
来源：http://agz.xinyue.icu

Go:   len(arr)
来源：http://gpt.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://fiw.guowangkeji.top

C#:   list.Count;
来源：http://zcv.yonumen.top

[D07] 切片 / 取子数组
来源：http://sfo.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gbs.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lwq.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://owg.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://ofv.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://phx.52xcode.cn

Go:   arr[1:4]
来源：http://epu.yonumen.top

Ruby: arr[1, 3]
来源：http://umm.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://czj.chenlongwang.top

[D08] 合并两个数组
来源：http://klq.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://sbf.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://hlr.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mqf.yj202588.top

TS:   [...a, ...b];
来源：http://zot.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qmh.fzhhl.top

Go:   append(a, b...)
来源：http://jsh.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://oxu.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://qew.yvedp.cn

[D09] 排序（升序）
来源：http://oep.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://hma.fengsongda.top

PHP:  sort($arr);
来源：http://vvl.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vdo.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zen.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://thh.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tvw.hesvh.cn

Ruby: arr.sort
来源：http://yrc.zhengqikj.top

C#:   list.Sort();
来源：http://fdd.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yhz.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://azl.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pxn.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bnp.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wng.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://syh.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kxy.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hzi.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yeh.sjlbkw.cn

[D11] 反转数组
来源：http://fji.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://vfq.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://klq.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vaq.fengsongda.top

TS:   [...arr].reverse();
来源：http://csb.chenzaomai.com

Java: Collections.reverse(list);
来源：http://yjt.hfpthk.cn

Go:   slices.Reverse(arr)
来源：http://zlx.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://iav.mhx1999.top

C#:   list.Reverse();
来源：http://ols.sjlbkw.cn

[D12] 查找元素下标
来源：http://sdf.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://viz.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ueq.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzr.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgf.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dtq.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://wnv.hammf.cn

Ruby: arr.index(x)
来源：http://kvh.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://bss.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://jcl.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bve.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jzg.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://wur.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://iap.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfp.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fsy.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://qvw.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zzz.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://ltq.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://idr.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yxq.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://wzh.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://xwb.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gsd.hesvh.cn

Go:   // 手写循环
来源：http://rgn.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://rmm.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://txs.sysykeji.top

[D15] 去重
来源：http://xtu.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ipo.shzxlz.cn

PHP:  array_unique($arr);
来源：http://ajb.cucudq.cn

JS:   [...new Set(arr)]
来源：http://tnc.hesvh.cn

TS:   [...new Set(arr)]
来源：http://odi.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djt.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://whq.sjlbkw.cn

Ruby: arr.uniq
来源：http://lkl.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://yao.yanxiufei.cn

[D16] 求和与平均值
来源：http://cli.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sba.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jfi.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gce.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pah.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vuq.yongpay.top

Go:   // 手写循环累加
来源：http://hdv.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kwl.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://gwh.havefunace.top

[D17] 最大值与最小值
来源：http://yuw.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://raq.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://vfx.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://siu.bjfxy.top

TS:   Math.max(...arr);
来源：http://wiq.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vln.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wat.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://goj.tarul.cn

C#:   list.Max();  list.Min()
来源：http://sws.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://dor.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://srx.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://vpw.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vhh.meibo888.top

TS:   nested.flat();
来源：http://lik.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://keu.cqqwz.cn

Go:   // 手写双层循环
来源：http://ula.snrcjt.cn

Ruby: nested.flatten
来源：http://mqk.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fub.mhx1999.top

[D19] 按字段分组
来源：http://vrx.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zfp.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ttp.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pqe.fehbvm.com


<!-- 参考信息 -->