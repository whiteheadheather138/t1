代发 wailian999

Py:   return a, b
来源：http://ifu.cashguo.top

PHP:  return [$a, $b];
来源：http://daa.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qei.cdnleiting.top

TS:   return { a, b };
来源：http://vuk.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qjh.jiagoushi.top

Go:   return a, b
来源：http://ohb.nwbrower.top

Ruby: return a, b
来源：http://adg.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://dds.hammf.cn

[C06] 匿名函数 / lambda
来源：http://hfq.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://ybz.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://khh.guowangkeji.top

JS:   const square = x => x * x;
来源：http://lpe.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://lhe.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gpn.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://zdb.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://acs.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://spa.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://rpb.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nxd.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://pwp.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ijr.zhijiandao.cn

TS:   arr.map(String)
来源：http://wck.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sxe.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ncu.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://qdq.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://osd.jiagoushi.top

[C08] 闭包
来源：http://ihn.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://heo.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://apg.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gel.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fhv.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zye.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fvl.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gsl.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uzy.meibo888.top

[C09] 递归
来源：http://uvl.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oxe.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jxh.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwt.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ewl.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lei.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kzk.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://grv.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kgf.kuanghao11.cn

[C10] 变量作用域
来源：http://zyl.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tzu.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tzd.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kkp.zhengqikj.top

TS:   同 JS
来源：http://fxj.tarul.cn

Java: 方法内为块级作用域
来源：http://zcg.yvedp.cn

Go:   花括号块级作用域
来源：http://nvk.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zsl.yj202588.top

C#:   块级作用域
来源：http://yrx.yongpay.top

[C11] 模块导入与导出
来源：http://qsx.jiagoushi.top

Py:   from module import func
来源：http://coy.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://evm.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ldz.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://drc.wangdashe.top

Java: import java.util.List;
来源：http://owu.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dnt.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://odd.gogol.net.cn

C#:   using System.Text;
来源：http://pvy.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://anc.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://amv.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://iib.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://aat.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://ymn.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cyk.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://hvy.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://mkw.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wdf.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://moa.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dbz.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpc.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mnw.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lrm.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://stb.yj20258.top

Go:   func add(a, b int) int
来源：http://cvb.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://feh.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://egf.dianchejie.cn

[C14] 泛型函数
来源：http://zsh.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kkf.yueranfly.top

PHP:  // 无泛型
来源：http://zga.ydzc1.top

JS:   // 无泛型
来源：http://wum.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fdk.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://duh.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://opt.ivvv.top

Ruby: # 无泛型
来源：http://hhq.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mch.yonumen.top

[C15] 解构 / 展开参数
来源：http://zvn.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lyp.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://vvd.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azd.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wlu.xziqi.cn

Java: // 无解构
来源：http://uzs.aizwys.cn

Go:   // 无解构
来源：http://otz.nanxuanxn.top

Ruby: a, b = pair
来源：http://cer.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://xeg.daxiang520.top

[C16] 函数 / 方法重载
来源：http://gkf.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wly.xinyue.icu

PHP:  // 无重载
来源：http://apl.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vfp.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://qzz.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zff.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://ngg.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://gkd.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://csx.guowangkeji.top

================================================================================
来源：http://awv.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://bdq.hesvh.cn

================================================================================
来源：http://imr.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://ldw.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wbe.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xdj.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gbj.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nnj.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpk.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://san.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://ucy.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fyo.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://ack.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rle.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slh.dashuyun.cn

JS:   arr.push(4);
来源：http://phw.tarul.cn

TS:   arr.push(4);
来源：http://nym.yonumen.top

Java: list.add(4);
来源：http://dbk.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://rqv.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://vim.havefunace.top

C#:   list.Add(4);
来源：http://fma.havefunace.top

[D03] 在指定位置插入元素
来源：http://yrw.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://hia.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kkz.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yvt.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://kgk.guannengcc.top

Java: list.add(0, 0);
来源：http://jzc.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://igd.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mfm.uphjek.com

C#:   list.Insert(0, 0);
来源：http://dcp.nanxinkj.top

[D04] 删除元素
来源：http://mmy.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ezv.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uhe.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxz.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://pen.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gyi.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fpl.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wpq.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lfk.sxryk.cn

[D05] 访问与修改元素
来源：http://bsu.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uhb.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rma.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://awu.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://jkz.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://qex.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://aze.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ubx.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fvq.zhiwuduotai.top

[D06] 数组长度
来源：http://mrc.shanyushiyangtech.top

Py:   len(arr)
来源：http://dak.ppjwa.cn

PHP:  count($arr);
来源：http://wjj.cdnleiting.top

JS:   arr.length
来源：http://cko.cqqwz.cn

TS:   arr.length
来源：http://eyb.wangdashe.top

Java: list.size();
来源：http://qlg.fzhhl.top

Go:   len(arr)
来源：http://htu.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://oue.nanxinkj.top

C#:   list.Count;
来源：http://otm.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://vnm.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nwz.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zeq.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://nbh.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://yey.cucudq.cn

Java: list.subList(1, 4);
来源：http://oyr.feifeiyinyue.top

Go:   arr[1:4]
来源：http://ujq.gzhubu.top

Ruby: arr[1, 3]
来源：http://yyc.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://mbt.xinyue.icu

[D08] 合并两个数组
来源：http://inc.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://knm.yongpay.top

PHP:  array_merge($a, $b);
来源：http://slf.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://osl.tian-w.cn

TS:   [...a, ...b];
来源：http://bfw.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxo.yfazqb.com

Go:   append(a, b...)
来源：http://wwq.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://tut.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://hub.jqgfzy.top

[D09] 排序（升序）
来源：http://hyx.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://woj.yangfankeji.com

PHP:  sort($arr);
来源：http://xjf.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xxr.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rbx.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ccb.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uze.hesvh.cn

Ruby: arr.sort
来源：http://pdy.quarkkingdee.top

C#:   list.Sort();
来源：http://sch.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iua.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cis.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ndv.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://huh.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvs.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tkv.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvx.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aep.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://btl.hnxiangtu.top

[D11] 反转数组
来源：http://zgl.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ces.cucudq.cn

PHP:  array_reverse($arr);
来源：http://stq.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ehb.yueranfly.top

TS:   [...arr].reverse();
来源：http://htv.iojbl.cn

Java: Collections.reverse(list);
来源：http://smv.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://apf.hammf.cn

Ruby: arr.reverse
来源：http://hjg.zdbjq.cn

C#:   list.Reverse();
来源：http://uiz.jinqigufen.top

[D12] 查找元素下标
来源：http://bws.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://oou.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://emi.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lar.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffr.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kya.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://rwr.gogol.net.cn

Ruby: arr.index(x)
来源：http://bii.52xcode.cn

C#:   list.IndexOf(x);
来源：http://fdf.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://gfc.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iii.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jqt.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://zpx.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://brs.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ugi.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vvq.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://cxb.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lzk.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://vjv.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ezp.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gtd.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://ufz.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://itx.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mms.cheryme.top

Go:   // 手写循环
来源：http://qfj.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://moi.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ukz.cheryme.top

[D15] 去重
来源：http://jov.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ktv.yangfankeji.com

PHP:  array_unique($arr);
来源：http://bil.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://wqv.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://hyy.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wom.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yoh.xuetiantiany.cn

Ruby: arr.uniq
来源：http://fvu.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://dwc.zdqjudy.top

[D16] 求和与平均值
来源：http://xnf.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ine.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oqz.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nys.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zzf.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rff.yangfankeji.com

Go:   // 手写循环累加
来源：http://hiy.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hfl.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://ydr.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://trf.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://eum.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://ibs.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jak.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://pnk.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zhm.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://atc.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://ore.yongpay.top

C#:   list.Max();  list.Min()
来源：http://ecj.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://umt.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aov.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://eto.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qam.zhijiandao.cn

TS:   nested.flat();
来源：http://hei.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pzw.shzxlz.cn

Go:   // 手写双层循环
来源：http://qxe.jyoumei.cn

Ruby: nested.flatten
来源：http://onx.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pki.yuxming.cn

[D19] 按字段分组
来源：http://iza.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://seq.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bal.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tvh.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aue.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jdi.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://ire.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tui.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kpm.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://ntm.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://mrc.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://jhr.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kta.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpb.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sma.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://wmv.ppjwa.cn

Ruby: arr.tally
来源：http://zoe.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gfo.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://mno.zdbjq.cn

Py:   x in arr
来源：http://vic.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://iyu.quarkkingdee.top

JS:   arr.includes(x)
来源：http://doa.jinqigufen.top

TS:   arr.includes(x)
来源：http://pdn.redwolf501.top

Java: list.contains(x)
来源：http://qbx.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://rfu.zdbjq.cn

Ruby: arr.include?(x)
来源：http://tbr.sweek.top

C#:   list.Contains(x)
来源：http://lhg.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://ujf.shangyingyoupin.top


<!-- 参考信息 -->