代发 wailian999

Java: if (data == null) return;
来源：http://zro.xziqi.cn

Go:   if data == nil { return }
来源：http://iyc.meibo888.top

Ruby: return if data.nil?
来源：http://mzi.quarkkingdee.top

C#:   if (data == null) return;
来源：http://ibh.dianchejie.cn

================================================================================
来源：http://hir.wangdashe.top

C. 函数与作用域
来源：http://kbe.xingfuxueyuan.xyz

================================================================================
来源：http://ffu.epnwcf.com

[C01] 定义函数
来源：http://ara.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://jwm.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://axg.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://jyq.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tag.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zco.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://hau.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://ufs.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zqg.ybcxt.top

[C02] 默认参数
来源：http://sfn.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://zsw.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wic.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://jyy.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nel.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ggh.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iec.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://fss.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://zpc.shzxlz.cn

[C03] 可变参数
来源：http://ven.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://hoj.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ztc.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ovq.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://osv.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xie.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tll.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://szy.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ntw.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://lri.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bdk.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rub.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://drk.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rcg.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://bdu.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://mbu.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://kwm.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://hmv.sweek.top

[C05] 返回多个值
来源：http://rmy.yfazqb.com

Py:   return a, b
来源：http://obc.hywenlv.cn

PHP:  return [$a, $b];
来源：http://rlp.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://esu.c1oappe.top

TS:   return { a, b };
来源：http://ipy.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://law.hammf.cn

Go:   return a, b
来源：http://ltf.yfazqb.com

Ruby: return a, b
来源：http://vdt.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://fhv.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://oxu.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://fzc.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rmh.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://ypg.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://ibc.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://suw.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://aap.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://sul.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://lxo.smart0.xyz

[C07] 把函数作为参数传入
来源：http://nuq.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lwm.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xwb.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kkj.feifeiyinyue.top

TS:   arr.map(String)
来源：http://clu.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qdu.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://flr.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://bna.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ifa.xingfuxueyuan.xyz

[C08] 闭包
来源：http://yaj.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xnc.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tbt.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qpu.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tib.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ikn.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mmt.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gwq.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pvz.jinghuilouyu.cn

[C09] 递归
来源：http://slt.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hja.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qrr.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qwa.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qdb.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tij.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yut.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hue.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdh.shanyushiyangtech.top

[C10] 变量作用域
来源：http://ekx.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://buk.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://msp.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cid.fehbvm.com

TS:   同 JS
来源：http://cbi.dashuyun.cn

Java: 方法内为块级作用域
来源：http://ihn.mhx1999.top

Go:   花括号块级作用域
来源：http://mkr.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nya.fzhhl.top

C#:   块级作用域
来源：http://eby.shzxlz.cn

[C11] 模块导入与导出
来源：http://nir.quarkkingdee.top

Py:   from module import func
来源：http://xdy.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bto.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://knv.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ejy.52xcode.cn

Java: import java.util.List;
来源：http://lgl.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xxn.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://drx.hongshengwenyu.top

C#:   using System.Text;
来源：http://yor.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://xxu.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://zji.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://fjz.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://wbm.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://sjz.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igp.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://rdx.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://oue.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yva.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://ihd.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iam.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inz.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://srp.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jls.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://viv.9152youxi.cn

Go:   func add(a, b int) int
来源：http://qpf.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yux.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://rcn.pengpengdd.cyou

[C14] 泛型函数
来源：http://qqj.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rvk.sweek.top

PHP:  // 无泛型
来源：http://tyx.iojbl.cn

JS:   // 无泛型
来源：http://tpp.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fxy.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ojl.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://srx.bbcook.cn

Ruby: # 无泛型
来源：http://nvh.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oyd.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://lke.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acn.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://pgf.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yqm.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hnd.sjlbkw.cn

Java: // 无解构
来源：http://nrq.meibo888.top

Go:   // 无解构
来源：http://pjl.kuanghao11.cn

Ruby: a, b = pair
来源：http://ecf.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://ogp.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://ife.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vqa.daria6918.cn

PHP:  // 无重载
来源：http://nwe.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://smb.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://wvc.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dzr.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://seo.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://xkb.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wcc.redwolf501.top

================================================================================
来源：http://myn.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://qpn.jqgufenzy.top

================================================================================
来源：http://ggf.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://kcv.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://stg.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xus.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pql.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ugw.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cgi.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://squ.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://nrt.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yzz.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://pxp.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nta.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tot.c1oappe.top

JS:   arr.push(4);
来源：http://gcg.pengpengdd.cyou

TS:   arr.push(4);
来源：http://klo.fengsongda.top

Java: list.add(4);
来源：http://owy.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://prk.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://rul.hesvh.cn

C#:   list.Add(4);
来源：http://lhh.yj20258888.top

[D03] 在指定位置插入元素
来源：http://sen.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://rvs.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hon.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xyk.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://giw.aibaodan.cn

Java: list.add(0, 0);
来源：http://dkb.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://idp.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mvk.pycfn.com

C#:   list.Insert(0, 0);
来源：http://pbd.316326.xyz

[D04] 删除元素
来源：http://uxn.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rdz.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kbq.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wxk.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://knu.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lnh.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://arn.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://snq.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qsq.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://ijc.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://grt.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bio.jinqigufen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kau.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://vch.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://kkv.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://loh.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fbw.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tvr.gotoacloud.top

[D06] 数组长度
来源：http://uhv.epnwcf.com

Py:   len(arr)
来源：http://maz.zdbjq.cn

PHP:  count($arr);
来源：http://fad.xuanzx.com

JS:   arr.length
来源：http://ksa.guannengcc.top

TS:   arr.length
来源：http://udm.shuidangran.top

Java: list.size();
来源：http://cnk.aibaodan.cn

Go:   len(arr)
来源：http://euc.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://dcp.tarul.cn

C#:   list.Count;
来源：http://bsp.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://lfd.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ogh.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cke.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://voh.tarul.cn

TS:   arr.slice(1, 4);
来源：http://zxh.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://vgz.havefunace.top

Go:   arr[1:4]
来源：http://pxu.9152youxi.cn

Ruby: arr[1, 3]
来源：http://pfn.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://tvt.yvedp.cn

[D08] 合并两个数组
来源：http://znt.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://uzr.cashguo.top

PHP:  array_merge($a, $b);
来源：http://ncl.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ret.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://tae.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lvp.tian-w.cn

Go:   append(a, b...)
来源：http://cpd.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://ujy.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://pll.52xcode.cn

[D09] 排序（升序）
来源：http://ggs.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://wed.guowangkeji.top

PHP:  sort($arr);
来源：http://ysb.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wnh.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tzj.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uee.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://owm.nwbrower.top

Ruby: arr.sort
来源：http://cwo.yfazqb.com

C#:   list.Sort();
来源：http://dwv.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjg.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pyu.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdg.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://enl.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lyr.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://okh.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sgn.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obz.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mrd.gaohongyu789.top

[D11] 反转数组
来源：http://xbt.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://maq.redwolf501.top

PHP:  array_reverse($arr);
来源：http://jge.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nzf.hfpthk.cn

TS:   [...arr].reverse();
来源：http://zqv.zhengqikj.top

Java: Collections.reverse(list);
来源：http://hrp.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://cfj.fengsongda.top

Ruby: arr.reverse
来源：http://whd.daria6918.cn

C#:   list.Reverse();
来源：http://eoy.cashguo.top

[D12] 查找元素下标
来源：http://erz.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://lvf.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://diy.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fis.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogz.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rth.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://xxy.ppjwa.cn

Ruby: arr.index(x)
来源：http://opz.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://yyl.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://gzr.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dkb.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yrd.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://byu.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://cvl.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ohu.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mxx.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kpj.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qbv.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://fix.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mdy.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://udm.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://xyt.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://slq.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyo.xylfe.cn

Go:   // 手写循环
来源：http://kmv.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://euv.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://mkl.tian-w.cn

[D15] 去重
来源：http://tqb.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dbb.havefunace.top

PHP:  array_unique($arr);
来源：http://dms.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://fkv.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://mef.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kcx.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://olh.hywenlv.cn

Ruby: arr.uniq
来源：http://tyb.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://dnr.jlsjyb.cn

[D16] 求和与平均值
来源：http://oqo.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyc.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://usd.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tax.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ohz.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uob.daria6918.cn

Go:   // 手写循环累加
来源：http://ohx.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fkw.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://hms.kuanghao11.cn

[D17] 最大值与最小值
来源：http://pdt.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://ehl.fanxiaobao.xyz


<!-- 参考信息 -->