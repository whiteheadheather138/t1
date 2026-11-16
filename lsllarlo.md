代发 wailian999

[C02] 默认参数
来源：http://cgh.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://zqb.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gns.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://nie.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jdg.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://max.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sbf.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://tmd.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://eeh.yanxiufei.cn

[C03] 可变参数
来源：http://qmu.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://nhd.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://caj.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gwc.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jrh.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uls.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://swn.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dds.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wuk.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://myh.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bxe.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pzx.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fly.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cyb.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://ypk.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://ajt.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://zen.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://ytt.chenzaomai.com

[C05] 返回多个值
来源：http://srl.nwbrower.top

Py:   return a, b
来源：http://hox.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://pmh.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://agj.hcnkem.com

TS:   return { a, b };
来源：http://idw.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jmp.ivvv.top

Go:   return a, b
来源：http://huc.dianchejie.cn

Ruby: return a, b
来源：http://gso.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://usv.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://zno.yongpay.top

Py:   square = lambda x: x * x
来源：http://bbn.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ekk.guowangkeji.top

JS:   const square = x => x * x;
来源：http://nsl.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yso.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vjs.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sbm.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://uuo.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://glo.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://byk.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgu.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pzt.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bsm.kuanghao11.cn

TS:   arr.map(String)
来源：http://qvs.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lfr.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://low.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://jjn.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pzb.guowangkeji.top

[C08] 闭包
来源：http://ddf.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://orx.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://abn.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lcb.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cao.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hmp.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://drf.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nyj.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mis.yuxming.cn

[C09] 递归
来源：http://rta.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zru.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fmt.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kxm.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjj.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iyg.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kro.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jpg.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mrm.guannengcc.top

[C10] 变量作用域
来源：http://gms.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yef.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zeo.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bbc.nwbrower.top

TS:   同 JS
来源：http://tii.epnwcf.com

Java: 方法内为块级作用域
来源：http://htm.jlsjyb.cn

Go:   花括号块级作用域
来源：http://fco.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cyj.bjfxy.top

C#:   块级作用域
来源：http://hqz.smart0.xyz

[C11] 模块导入与导出
来源：http://thc.ctjpmb.com

Py:   from module import func
来源：http://daz.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://shp.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://avj.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kwz.chenzaomai.com

Java: import java.util.List;
来源：http://flg.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xky.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://phf.nanxinkj.top

C#:   using System.Text;
来源：http://mtb.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://mnx.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://pws.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://lxd.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://cmy.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://jdh.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://spe.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://vim.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://ndt.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uji.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://vuu.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://btm.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pre.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umm.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipd.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hfc.tanke756.top

Go:   func add(a, b int) int
来源：http://pre.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kul.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://chv.ppjwa.cn

[C14] 泛型函数
来源：http://wqh.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pca.yuanzhike.top

PHP:  // 无泛型
来源：http://kqe.aibaodan.cn

JS:   // 无泛型
来源：http://bva.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wld.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sfs.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qeo.yonumen.top

Ruby: # 无泛型
来源：http://kze.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ujj.pycfn.com

[C15] 解构 / 展开参数
来源：http://xih.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jty.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://fdx.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xcl.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cvm.hywenlv.cn

Java: // 无解构
来源：http://vke.gaohongyu789.top

Go:   // 无解构
来源：http://hku.zycfv.cn

Ruby: a, b = pair
来源：http://vlj.nwbrower.top

C#:   var (a, b) = pair;
来源：http://vdc.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://qya.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://odd.snrcjt.cn

PHP:  // 无重载
来源：http://xkt.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tsz.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fva.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gvz.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://col.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://qvl.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://iue.jinyuanbaomall.cn

================================================================================
来源：http://frr.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://hck.nwbrower.top

================================================================================
来源：http://bkd.yueranfly.top

[D01] 创建数组 / 列表
来源：http://wth.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://muz.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sdp.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://csx.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ejk.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nti.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://rkb.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://xzp.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qin.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://gdv.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zrn.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rsr.nanxinkj.top

JS:   arr.push(4);
来源：http://pld.9152youxi.cn

TS:   arr.push(4);
来源：http://axj.jlsjyb.cn

Java: list.add(4);
来源：http://sde.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://jvi.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://gdr.andypj.xyz

C#:   list.Add(4);
来源：http://suj.ydzc1.top

[D03] 在指定位置插入元素
来源：http://uxp.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://yxf.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rll.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cju.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://gpm.guannengcc.top

Java: list.add(0, 0);
来源：http://lwn.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://arn.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fve.yongpay.top

C#:   list.Insert(0, 0);
来源：http://hms.gaohongyu789.top

[D04] 删除元素
来源：http://nmc.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fmh.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oza.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uzr.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://gvo.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pyd.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aea.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xuy.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rzq.yj20258888.top

[D05] 访问与修改元素
来源：http://tfz.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wea.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sqh.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovb.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://xfr.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://leh.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://kct.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uao.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://seo.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://vpz.shanyushiyangtech.top

Py:   len(arr)
来源：http://zit.havefunace.top

PHP:  count($arr);
来源：http://pzb.svipenyu.cn

JS:   arr.length
来源：http://dmp.ybcxt.top

TS:   arr.length
来源：http://nrr.nanxinkj.top

Java: list.size();
来源：http://krd.daxiang520.top

Go:   len(arr)
来源：http://hvz.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://hyg.cqqwz.cn

C#:   list.Count;
来源：http://hra.hnqzz.top

[D07] 切片 / 取子数组
来源：http://xbt.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svp.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://jie.ivvv.top

JS:   arr.slice(1, 4);
来源：http://brs.havefunace.top

TS:   arr.slice(1, 4);
来源：http://cml.shuidangran.top

Java: list.subList(1, 4);
来源：http://sgk.daria6918.cn

Go:   arr[1:4]
来源：http://ncs.dianchejie.cn

Ruby: arr[1, 3]
来源：http://yaj.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://pqi.hfpthk.cn

[D08] 合并两个数组
来源：http://htg.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://lam.pycfn.com

PHP:  array_merge($a, $b);
来源：http://xmy.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jre.hywenlv.cn

TS:   [...a, ...b];
来源：http://hat.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xnm.yj20258.top

Go:   append(a, b...)
来源：http://kbm.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://cia.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://xvn.cdnleiting.top

[D09] 排序（升序）
来源：http://aml.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://doi.gotoacloud.top

PHP:  sort($arr);
来源：http://oam.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ewa.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywn.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://hqj.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yyc.hnxiangtu.top

Ruby: arr.sort
来源：http://vbu.ppjwa.cn

C#:   list.Sort();
来源：http://mzy.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mdd.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://seg.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://abd.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://abr.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xwk.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mvf.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://adw.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tao.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uab.ywan-chungtsiang.top

[D11] 反转数组
来源：http://tvo.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xmc.hammf.cn

PHP:  array_reverse($arr);
来源：http://fdq.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xsg.xinyue.icu

TS:   [...arr].reverse();
来源：http://xkd.pycfn.com

Java: Collections.reverse(list);
来源：http://ifo.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://oko.sxryk.cn

Ruby: arr.reverse
来源：http://win.fktsv.cn

C#:   list.Reverse();
来源：http://ken.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://szr.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://mil.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uwo.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jlu.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pob.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sxf.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://nho.bbcook.cn

Ruby: arr.index(x)
来源：http://krd.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://zms.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://ggy.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://evn.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ipn.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://asn.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://ebc.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dbg.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bcm.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bqe.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mbs.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://bqo.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xnq.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xkf.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://yhg.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://fpw.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pfd.52xcode.cn

Go:   // 手写循环
来源：http://gfy.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://uxd.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://qyn.ydzc1.top

[D15] 去重
来源：http://nli.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fiz.hesvh.cn

PHP:  array_unique($arr);
来源：http://rwl.xylfe.cn

JS:   [...new Set(arr)]
来源：http://xzj.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://okr.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zps.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://wcu.shuidangran.top

Ruby: arr.uniq
来源：http://who.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://non.sweek.top

[D16] 求和与平均值
来源：http://nnp.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ynf.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iod.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpc.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqv.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uvo.cashguo.top

Go:   // 手写循环累加
来源：http://hza.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rhf.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://lqw.316326.xyz

[D17] 最大值与最小值
来源：http://lda.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://hqm.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://atj.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jkk.nwbrower.top

TS:   Math.max(...arr);
来源：http://wrm.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fcu.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aut.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://emp.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://dfm.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://ghl.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tpu.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://axe.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qms.zhengqikj.top

TS:   nested.flat();
来源：http://lfe.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qxy.xziqi.cn

Go:   // 手写双层循环
来源：http://hdk.havefunace.top

Ruby: nested.flatten
来源：http://iyl.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zww.xuetiantiany.cn


<!-- 参考信息 -->