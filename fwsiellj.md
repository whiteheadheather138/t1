代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://vwf.zhiwuduotai.top

[C03] 可变参数
来源：http://gwb.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://rri.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bta.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cft.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfm.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ctz.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kgu.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://lwm.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzz.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://lhy.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jlv.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gku.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qpi.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bpv.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://iiq.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://rtv.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://dgf.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://ytq.bbcook.cn

[C05] 返回多个值
来源：http://cvz.mhx1999.top

Py:   return a, b
来源：http://acn.jyoumei.cn

PHP:  return [$a, $b];
来源：http://whg.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vgg.hammf.cn

TS:   return { a, b };
来源：http://bew.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lhx.xziqi.cn

Go:   return a, b
来源：http://trv.cashguo.top

Ruby: return a, b
来源：http://smb.hcnkem.com

C#:   return (a, b);              // ValueTuple
来源：http://wuf.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://urg.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://vxy.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ktz.pycfn.com

JS:   const square = x => x * x;
来源：http://zbg.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://rgn.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bxt.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://krl.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://ljr.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tlo.tian-w.cn

[C07] 把函数作为参数传入
来源：http://qfl.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wlc.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tzu.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yvg.shangyingyoupin.top

TS:   arr.map(String)
来源：http://sgp.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wxp.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jnm.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://iww.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pvz.nwbrower.top

[C08] 闭包
来源：http://stt.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fef.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ugs.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vor.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://llf.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://twm.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yke.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yrl.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psi.haohaochexian.top

[C09] 递归
来源：http://ijv.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ufk.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://abe.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://voh.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgm.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qga.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kix.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://siq.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wtu.epnwcf.com

[C10] 变量作用域
来源：http://zim.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jiv.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nbl.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://igf.guannengcc.top

TS:   同 JS
来源：http://udy.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://tix.zdbjq.cn

Go:   花括号块级作用域
来源：http://nys.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jvv.shanyushiyangkeji.top

C#:   块级作用域
来源：http://owq.yj20258.top

[C11] 模块导入与导出
来源：http://vbt.yfazqb.com

Py:   from module import func
来源：http://rad.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pcc.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xrk.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cla.nwbrower.top

Java: import java.util.List;
来源：http://nhe.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyx.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://vdv.nwbrower.top

C#:   using System.Text;
来源：http://kja.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://jwl.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://gik.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://kyc.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://lrq.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://xgq.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://olc.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://itm.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://ewu.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cqt.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://pua.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nxn.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gav.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kmu.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tyr.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://jck.dianchejie.cn

Go:   func add(a, b int) int
来源：http://pmc.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nkf.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://jjq.yuxming.cn

[C14] 泛型函数
来源：http://nfe.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zmg.fengsongda.top

PHP:  // 无泛型
来源：http://ggc.chenjidiqi.icu

JS:   // 无泛型
来源：http://nil.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://erp.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oor.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qur.cheryme.top

Ruby: # 无泛型
来源：http://lec.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ceg.yj20258.top

[C15] 解构 / 展开参数
来源：http://cot.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://djt.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://qth.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eso.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ldz.0kj1m.cn

Java: // 无解构
来源：http://lkk.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://jfx.pycfn.com

Ruby: a, b = pair
来源：http://hdf.epnwcf.com

C#:   var (a, b) = pair;
来源：http://scw.fktsv.cn

[C16] 函数 / 方法重载
来源：http://rkx.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ovx.zhiwuduotai.top

PHP:  // 无重载
来源：http://vtz.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zjx.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://baz.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kpj.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://mvu.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://dir.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbp.jqgufenzy.top

================================================================================
来源：http://rhh.cheryme.top

D. 数组 / 列表 / 集合
来源：http://wbd.shanyushiyangkeji.top

================================================================================
来源：http://rlh.hammf.cn

[D01] 创建数组 / 列表
来源：http://otj.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mzz.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gmo.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sxf.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hef.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ona.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://axg.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://eya.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://klh.zdqjudy.top

[D02] 追加元素到末尾
来源：http://efe.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rjt.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jrz.316326.xyz

JS:   arr.push(4);
来源：http://qva.yvedp.cn

TS:   arr.push(4);
来源：http://tem.nanxuanxn.top

Java: list.add(4);
来源：http://mmk.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://goh.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://pdl.sysykeji.top

C#:   list.Add(4);
来源：http://xru.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://bey.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://dmo.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gov.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://whv.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://gbt.0kj1m.cn

Java: list.add(0, 0);
来源：http://nta.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://wwx.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yse.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://oni.smart0.xyz

[D04] 删除元素
来源：http://zav.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://icb.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eub.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxh.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://pjx.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cxv.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://asw.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rtf.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oqs.snrcjt.cn

[D05] 访问与修改元素
来源：http://jcx.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dzs.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://anx.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xfs.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://ota.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://wla.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://pyg.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tap.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eiy.gaohongyu789.top

[D06] 数组长度
来源：http://nfe.shuidangran.top

Py:   len(arr)
来源：http://azg.xuanzx.com

PHP:  count($arr);
来源：http://muk.xuetiantiany.cn

JS:   arr.length
来源：http://tfy.yongpay.top

TS:   arr.length
来源：http://edn.fengsongda.top

Java: list.size();
来源：http://pqz.hysaishi.cn

Go:   len(arr)
来源：http://lek.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://fpz.gogol.net.cn

C#:   list.Count;
来源：http://oie.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://xsv.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nyd.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://zsw.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://iru.tanke756.top

TS:   arr.slice(1, 4);
来源：http://wwy.jianghu66.top

Java: list.subList(1, 4);
来源：http://upo.svipenyu.cn

Go:   arr[1:4]
来源：http://zjf.fengsongda.top

Ruby: arr[1, 3]
来源：http://gsw.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://loc.yfazqb.com

[D08] 合并两个数组
来源：http://ojf.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://vqa.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://vig.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://imk.jinqigufen.top

TS:   [...a, ...b];
来源：http://kiv.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qwa.nwbrower.top

Go:   append(a, b...)
来源：http://cpm.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://tim.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://tdn.hnqzz.top

[D09] 排序（升序）
来源：http://gfu.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://nnx.fktsv.cn

PHP:  sort($arr);
来源：http://vlk.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eqx.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fmv.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://snv.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ktn.fengsongda.top

Ruby: arr.sort
来源：http://ezl.bbcook.cn

C#:   list.Sort();
来源：http://dzf.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://san.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://foz.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjv.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sth.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dmi.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xuy.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gtd.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mot.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvv.haohaochexian.top

[D11] 反转数组
来源：http://xhl.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://czn.pycfn.com

PHP:  array_reverse($arr);
来源：http://kps.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lok.sysykeji.top

TS:   [...arr].reverse();
来源：http://rzp.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://gei.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://hvk.nanxinkj.top

Ruby: arr.reverse
来源：http://rfn.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://uuc.chenzaomai.com

[D12] 查找元素下标
来源：http://pom.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://hhs.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qhv.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydn.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lol.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhv.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://tru.jiagoushi.top

Ruby: arr.index(x)
来源：http://eji.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://vvy.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://tlw.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rml.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://huw.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://jrs.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://kpl.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ohy.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zjw.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://ddh.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ljs.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://zgj.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gqc.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yuo.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://hib.jqgufenzy.top

TS:   arr.map(x => x * 2)
来源：http://oxc.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zgh.redwolf501.top

Go:   // 手写循环
来源：http://klg.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://txt.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ktd.zhixingplan.top

[D15] 去重
来源：http://zjk.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xke.zdbjq.cn

PHP:  array_unique($arr);
来源：http://fnx.xinyue.icu

JS:   [...new Set(arr)]
来源：http://qxb.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://xjz.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hyg.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://uwq.nwbrower.top

Ruby: arr.uniq
来源：http://eiv.cheryme.top

C#:   list.Distinct().ToList()
来源：http://iop.xuetiantiany.cn

[D16] 求和与平均值
来源：http://osb.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ven.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qrx.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://don.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://khs.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zgz.hnqzz.top

Go:   // 手写循环累加
来源：http://abm.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bec.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://qgi.hammf.cn

[D17] 最大值与最小值
来源：http://xzi.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://xge.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://ewq.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://koq.mhx1999.top

TS:   Math.max(...arr);
来源：http://plm.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oue.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xpd.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://fhi.yonumen.top

C#:   list.Max();  list.Min()
来源：http://yks.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://xlx.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pvu.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://imc.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ypr.aizwys.cn

TS:   nested.flat();
来源：http://uwn.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://quh.tianlin.xyz

Go:   // 手写双层循环
来源：http://vgx.shuidangran.top

Ruby: nested.flatten
来源：http://gbw.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ebg.zdbjq.cn

[D19] 按字段分组
来源：http://mjr.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kuf.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rqy.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vuy.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://acc.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fyd.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://fpn.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://eom.vqdsnc.cn


<!-- 参考信息 -->