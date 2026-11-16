代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://cgd.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cyg.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bsy.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://npb.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://evo.ehwqpu.com

[C03] 可变参数
来源：http://tog.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://jsu.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ftz.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://evf.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcp.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hwm.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bww.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://ozg.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nlp.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://xzi.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ied.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://znx.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpk.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://enl.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://vrv.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://twn.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://wkp.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://kwc.pycfn.com

[C05] 返回多个值
来源：http://olv.shangyingyoupin.top

Py:   return a, b
来源：http://mhk.yj202588.top

PHP:  return [$a, $b];
来源：http://bzd.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://geq.dashuyun.cn

TS:   return { a, b };
来源：http://kza.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pqq.hywenlv.cn

Go:   return a, b
来源：http://miw.ydjk.org.cn

Ruby: return a, b
来源：http://zqn.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://wnx.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://ssc.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://yzv.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ten.cucudq.cn

JS:   const square = x => x * x;
来源：http://xuu.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://clj.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvb.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://hgv.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://jyk.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cfc.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://ona.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nuu.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fip.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fwd.hnxiangtu.top

TS:   arr.map(String)
来源：http://wst.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jca.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gvh.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://nde.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bvg.jinqigufen.top

[C08] 闭包
来源：http://fap.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iuy.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lqd.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgw.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kjz.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vdc.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://orp.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fmh.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iiq.wangdashe.top

[C09] 递归
来源：http://fhl.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ckv.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oju.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvy.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpx.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rab.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ihf.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wzr.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ncl.yj20258.top

[C10] 变量作用域
来源：http://lfn.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lph.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mnx.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nlp.ehwqpu.com

TS:   同 JS
来源：http://kky.xylfe.cn

Java: 方法内为块级作用域
来源：http://nrk.yuxming.cn

Go:   花括号块级作用域
来源：http://xcr.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nad.yongpay.top

C#:   块级作用域
来源：http://dwh.ehwqpu.com

[C11] 模块导入与导出
来源：http://hqj.yvedp.cn

Py:   from module import func
来源：http://dua.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tys.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://boa.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wnv.hongshengwenyu.top

Java: import java.util.List;
来源：http://kcf.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fkx.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://qbf.yj202588.top

C#:   using System.Text;
来源：http://swf.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://zkc.yongpay.top

Py:   (lambda: print("run"))()
来源：http://vpf.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://cyn.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://oef.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://nmn.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rcm.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://imt.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://uaf.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://szd.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://ixw.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xwo.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmr.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dqs.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tww.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cgf.shzxlz.cn

Go:   func add(a, b int) int
来源：http://szg.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zur.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://mxk.zdqjudy.top

[C14] 泛型函数
来源：http://mie.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ehw.birdmap.top

PHP:  // 无泛型
来源：http://shc.guowangkeji.top

JS:   // 无泛型
来源：http://mny.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dwu.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sbg.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzm.guowangkeji.top

Ruby: # 无泛型
来源：http://uko.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gkq.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://nre.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tpu.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://ilg.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oll.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oqm.nanxuanxn.top

Java: // 无解构
来源：http://lmc.shanyushiyangkeji.top

Go:   // 无解构
来源：http://cqd.ivvv.top

Ruby: a, b = pair
来源：http://qip.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://tff.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://fqn.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zcd.zhiwuduotai.top

PHP:  // 无重载
来源：http://ehd.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mrg.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://cqy.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vzi.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://mxl.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://wfl.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wuh.sjlbkw.cn

================================================================================
来源：http://azl.havefunace.top

D. 数组 / 列表 / 集合
来源：http://ppm.aizwys.cn

================================================================================
来源：http://kcq.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://mla.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mfr.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fvr.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oha.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://daq.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cih.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://aez.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://myh.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lss.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://pbs.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nfv.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zvj.zdbjq.cn

JS:   arr.push(4);
来源：http://xpe.cheryme.top

TS:   arr.push(4);
来源：http://iqt.cqqwz.cn

Java: list.add(4);
来源：http://laj.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://jsj.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://yph.iojbl.cn

C#:   list.Add(4);
来源：http://twk.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://xwk.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://jht.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nhw.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sqb.ybcxt.top

TS:   arr.splice(0, 0, 0);
来源：http://bun.zhijiandao.cn

Java: list.add(0, 0);
来源：http://fkl.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aug.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ymq.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://ncj.vqdsnc.cn

[D04] 删除元素
来源：http://caa.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://axq.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uwv.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lmk.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://hgg.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cjp.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rou.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rfq.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kix.haohaochexian.top

[D05] 访问与修改元素
来源：http://qab.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://diz.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vuc.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fcw.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://mvy.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://shc.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://epy.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vie.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uuc.cashguo.top

[D06] 数组长度
来源：http://oxk.fehbvm.com

Py:   len(arr)
来源：http://atj.yanxiufei.cn

PHP:  count($arr);
来源：http://tbf.fzhhl.top

JS:   arr.length
来源：http://dak.dianchejie.cn

TS:   arr.length
来源：http://cwe.chenjidiqi.icu

Java: list.size();
来源：http://owu.mhx1999.top

Go:   len(arr)
来源：http://atn.tanke756.top

Ruby: arr.length; arr.size
来源：http://lgu.yfazqb.com

C#:   list.Count;
来源：http://bdk.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://icu.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lkl.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://ohw.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://ckl.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://ypw.xinyue.icu

Java: list.subList(1, 4);
来源：http://jbs.zhijiandao.cn

Go:   arr[1:4]
来源：http://gbx.daxiang520.top

Ruby: arr[1, 3]
来源：http://hkt.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://ivv.jqgfzy.top

[D08] 合并两个数组
来源：http://zek.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://zah.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://izj.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fbu.xylfe.cn

TS:   [...a, ...b];
来源：http://qrm.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cgi.jianghu66.top

Go:   append(a, b...)
来源：http://cfx.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://rya.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://vop.yfazqb.com

[D09] 排序（升序）
来源：http://vhu.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://did.wangdashe.top

PHP:  sort($arr);
来源：http://xzy.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qze.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://srz.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zib.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipw.ydjk.org.cn

Ruby: arr.sort
来源：http://ldx.c1oappe.top

C#:   list.Sort();
来源：http://gwo.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xhj.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iuv.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://apv.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mdk.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://two.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lvw.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aip.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://evc.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wep.bbcook.cn

[D11] 反转数组
来源：http://xht.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://qnd.cucudq.cn

PHP:  array_reverse($arr);
来源：http://jpd.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wzb.zdqjudy.top

TS:   [...arr].reverse();
来源：http://mdz.mhx1999.top

Java: Collections.reverse(list);
来源：http://brr.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://zwl.xziqi.cn

Ruby: arr.reverse
来源：http://gng.ctjpmb.com

C#:   list.Reverse();
来源：http://vml.yvedp.cn

[D12] 查找元素下标
来源：http://ajz.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://bfw.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mfd.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grz.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wlc.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cdo.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://dkk.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://jmb.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://sfk.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://eln.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vjj.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayx.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://sfv.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://hpd.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zsr.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://axt.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://jwl.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cxu.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://uyf.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iat.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rvc.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://pud.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://mwg.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sqt.feifeiyinyue.top

Go:   // 手写循环
来源：http://ghn.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://ilw.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://kby.jqgufenzy.top

[D15] 去重
来源：http://ckf.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://swf.uphjek.com

PHP:  array_unique($arr);
来源：http://hjx.xylfe.cn

JS:   [...new Set(arr)]
来源：http://eud.redwolf501.top

TS:   [...new Set(arr)]
来源：http://yse.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nnq.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ipg.ppjwa.cn

Ruby: arr.uniq
来源：http://uvh.yj20258.top

C#:   list.Distinct().ToList()
来源：http://pcv.hysaishi.cn

[D16] 求和与平均值
来源：http://zcv.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://egb.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qax.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffq.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fla.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ojs.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://orv.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hay.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://izz.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://zbk.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://rzg.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://uke.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ctg.yj20258.top

TS:   Math.max(...arr);
来源：http://cfy.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cgr.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tfu.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://vtx.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://mut.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://tot.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nya.ivvv.top

PHP:  array_merge(...$nested);
来源：http://sqe.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iup.jinghuilouyu.cn

TS:   nested.flat();
来源：http://yyd.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjx.jqgufenzy.top

Go:   // 手写双层循环
来源：http://ygl.hongshengwenyu.top

Ruby: nested.flatten
来源：http://qgl.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wjr.shuidangran.top

[D19] 按字段分组
来源：http://dgj.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jzy.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://otm.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hmp.tarul.cn


<!-- 参考信息 -->