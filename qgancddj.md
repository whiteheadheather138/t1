代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://bag.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sct.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mme.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://tav.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://uxg.vehdjk.com

[C03] 可变参数
来源：http://ker.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://hiy.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aip.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsd.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://isi.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://imm.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oet.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://blu.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nvw.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://jye.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://izl.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cqg.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqe.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bfy.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://asi.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://ikv.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://jgo.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://bnp.jinqigfzy.top

[C05] 返回多个值
来源：http://pgz.zhiwuduotai.top

Py:   return a, b
来源：http://dfq.c1oappe.top

PHP:  return [$a, $b];
来源：http://yee.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kpn.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://dft.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iqp.yuanzhike.top

Go:   return a, b
来源：http://rco.tianlin.xyz

Ruby: return a, b
来源：http://vti.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://ejp.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://cdr.jianghu66.top

Py:   square = lambda x: x * x
来源：http://dwi.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://njn.ydzc1.top

JS:   const square = x => x * x;
来源：http://bgr.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://ntr.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tht.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://suh.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://gva.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sqx.cheryme.top

[C07] 把函数作为参数传入
来源：http://isq.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vsb.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ebg.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uso.vehdjk.com

TS:   arr.map(String)
来源：http://omk.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wyc.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mqc.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://vfn.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lpp.yfazqb.com

[C08] 闭包
来源：http://rum.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jrd.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dat.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lnm.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ufe.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dee.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ymt.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tub.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pht.ppjwa.cn

[C09] 递归
来源：http://kgi.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aip.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zlr.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cjg.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzo.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cny.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uiy.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svy.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nzh.wangdashe.top

[C10] 变量作用域
来源：http://kin.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://urz.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fbi.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sqk.xuanzx.com

TS:   同 JS
来源：http://qyb.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://ueg.xziqi.cn

Go:   花括号块级作用域
来源：http://hch.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pqv.nwbrower.top

C#:   块级作用域
来源：http://pjj.zycfv.cn

[C11] 模块导入与导出
来源：http://xfc.dashuyun.cn

Py:   from module import func
来源：http://pxd.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zxh.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ret.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rgg.birdmap.top

Java: import java.util.List;
来源：http://xmz.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjn.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://zvt.ehwqpu.com

C#:   using System.Text;
来源：http://hrz.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://bov.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://enw.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://imy.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://skz.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://bgx.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://plv.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://nlt.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://igs.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bms.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://gug.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://glk.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vuh.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vlz.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ebn.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iea.ppjwa.cn

Go:   func add(a, b int) int
来源：http://agi.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hvy.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://lki.c1oappe.top

[C14] 泛型函数
来源：http://icl.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tom.yvedp.cn

PHP:  // 无泛型
来源：http://zhi.tian-w.cn

JS:   // 无泛型
来源：http://ptd.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ksm.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xos.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fkl.9152youxi.cn

Ruby: # 无泛型
来源：http://zie.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wsg.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://umb.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mtx.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://kmb.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rmo.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzh.pengpengdd.cyou

Java: // 无解构
来源：http://xxv.hesvh.cn

Go:   // 无解构
来源：http://lan.hfpthk.cn

Ruby: a, b = pair
来源：http://rba.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://sen.sysykeji.top

[C16] 函数 / 方法重载
来源：http://dgn.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fpu.ppjwa.cn

PHP:  // 无重载
来源：http://qex.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydt.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://wwm.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ktj.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://xbi.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://soe.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vqh.yangfankeji.com

================================================================================
来源：http://gql.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://zei.havefunace.top

================================================================================
来源：http://zds.fehbvm.com

[D01] 创建数组 / 列表
来源：http://phy.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://hwc.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uso.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cgz.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ehe.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jld.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://fcw.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://lev.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eel.hywenlv.cn

[D02] 追加元素到末尾
来源：http://yeg.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gqb.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ivh.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://afz.andypj.xyz

TS:   arr.push(4);
来源：http://csk.nanxinkj.top

Java: list.add(4);
来源：http://yjk.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://eal.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://ehy.ehwqpu.com

C#:   list.Add(4);
来源：http://izw.mhx1999.top

[D03] 在指定位置插入元素
来源：http://unw.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://nkn.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://idl.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cez.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://hfb.hysaishi.cn

Java: list.add(0, 0);
来源：http://dss.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hze.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://enw.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://asp.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://kzk.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iyf.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qnj.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://efl.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://dvw.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bzt.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://znx.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xsh.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uru.zdqjudy.top

[D05] 访问与修改元素
来源：http://hbn.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xos.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xmi.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jny.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://abh.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://vjm.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://gfe.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://raw.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://twj.ydzc1.top

[D06] 数组长度
来源：http://hej.gogol.net.cn

Py:   len(arr)
来源：http://dqq.vehdjk.com

PHP:  count($arr);
来源：http://hdj.zhengqikj.top

JS:   arr.length
来源：http://fxa.0kj1m.cn

TS:   arr.length
来源：http://zzu.316326.xyz

Java: list.size();
来源：http://ugq.316326.xyz

Go:   len(arr)
来源：http://jvh.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://kqw.daria6918.cn

C#:   list.Count;
来源：http://xyj.bjfxy.top

[D07] 切片 / 取子数组
来源：http://ofe.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jhh.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://rhx.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://adk.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://xcx.smart0.xyz

Java: list.subList(1, 4);
来源：http://qzx.yj20258888.top

Go:   arr[1:4]
来源：http://sdh.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://xpl.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://xur.gzhubu.top

[D08] 合并两个数组
来源：http://sle.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://diq.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://dfo.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pyn.xuanzx.com

TS:   [...a, ...b];
来源：http://plt.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nmm.jinqigufen.top

Go:   append(a, b...)
来源：http://xyl.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://acl.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://vsy.pycfn.com

[D09] 排序（升序）
来源：http://xwc.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://rlt.epnwcf.com

PHP:  sort($arr);
来源：http://tui.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://utf.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mri.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://erl.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://smj.jinghuilouyu.cn

Ruby: arr.sort
来源：http://dgd.sufxvd.cn

C#:   list.Sort();
来源：http://ony.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vmj.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xbx.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssy.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trd.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ygd.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rru.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://piq.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://anb.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iuq.9152youxi.cn

[D11] 反转数组
来源：http://fgj.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nye.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://xqb.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fgp.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://lkt.hywenlv.cn

Java: Collections.reverse(list);
来源：http://gtn.cashguo.top

Go:   slices.Reverse(arr)
来源：http://ywc.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://xti.chenlongwang.top

C#:   list.Reverse();
来源：http://pjt.guowangkeji.top

[D12] 查找元素下标
来源：http://xld.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://vbr.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hgf.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://avm.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rio.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sjr.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://wev.zdqjudy.top

Ruby: arr.index(x)
来源：http://qdw.nwbrower.top

C#:   list.IndexOf(x);
来源：http://rta.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://dks.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ocn.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yrh.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://krb.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://owg.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wtr.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gae.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mmn.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yrx.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://oyn.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eun.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ket.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://fnw.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://lhw.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gsg.hysaishi.cn

Go:   // 手写循环
来源：http://moz.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://bor.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://guk.yj20258.top

[D15] 去重
来源：http://diw.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vlw.c1oappe.top

PHP:  array_unique($arr);
来源：http://ydy.yj202588.top

JS:   [...new Set(arr)]
来源：http://flj.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://sja.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ugw.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://znf.jinqigufen.top

Ruby: arr.uniq
来源：http://aes.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://sqz.xuetiantiany.cn

[D16] 求和与平均值
来源：http://qcq.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://prh.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yml.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcu.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lpb.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rdj.cdnleiting.top

Go:   // 手写循环累加
来源：http://bvm.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://htv.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://gyj.xylfe.cn

[D17] 最大值与最小值
来源：http://cnz.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://qps.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://klr.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rrs.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://luj.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oqq.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qoi.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://aam.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://iqy.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://xrx.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gwe.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://wpp.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aks.fanxiaobao.xyz

TS:   nested.flat();
来源：http://dcd.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qee.quarkkingdee.top

Go:   // 手写双层循环
来源：http://mni.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://bml.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pyr.uphjek.com

[D19] 按字段分组
来源：http://akb.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cbj.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hfq.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kld.uphjek.com


<!-- 参考信息 -->