代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://rui.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://anh.pycfn.com

[C08] 闭包
来源：http://gan.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vhp.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jsg.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpn.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zxw.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bql.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqv.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kms.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oah.sysykeji.top

[C09] 递归
来源：http://ccb.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lan.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rrl.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgz.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpq.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvb.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mzi.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vmh.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pqn.bbcook.cn

[C10] 变量作用域
来源：http://deh.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kry.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blv.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://krl.gaohongyu789.top

TS:   同 JS
来源：http://wck.aizwys.cn

Java: 方法内为块级作用域
来源：http://loc.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://wdv.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yxe.c1oappe.top

C#:   块级作用域
来源：http://clh.yfazqb.com

[C11] 模块导入与导出
来源：http://jsr.xuetiantiany.cn

Py:   from module import func
来源：http://dal.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aah.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://czd.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ccm.hongshengwenyu.top

Java: import java.util.List;
来源：http://hsf.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://avf.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://vhf.iojbl.cn

C#:   using System.Text;
来源：http://ilw.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://dyp.yongpay.top

Py:   (lambda: print("run"))()
来源：http://tio.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://mxv.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://ple.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://fuy.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://esq.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://mah.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://tmy.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cvp.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://egb.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abm.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vme.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vua.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckt.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eat.yueranfly.top

Go:   func add(a, b int) int
来源：http://exu.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tpp.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pfj.dashuyun.cn

[C14] 泛型函数
来源：http://cyd.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzu.tarul.cn

PHP:  // 无泛型
来源：http://ebz.redwolf501.top

JS:   // 无泛型
来源：http://bdj.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://enl.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rxs.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zay.aibaodan.cn

Ruby: # 无泛型
来源：http://hlw.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pit.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://ewn.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nxo.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://onw.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://myn.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sci.nanxinkj.top

Java: // 无解构
来源：http://jcr.nanxinkj.top

Go:   // 无解构
来源：http://cir.dashuyun.cn

Ruby: a, b = pair
来源：http://cnj.yonumen.top

C#:   var (a, b) = pair;
来源：http://gsv.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://mui.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tit.zhiwuduotai.top

PHP:  // 无重载
来源：http://vet.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://adk.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://wqa.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iav.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://rsy.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://edo.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ndo.xuetiantiany.cn

================================================================================
来源：http://tcn.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://nhf.jiagoushi.top

================================================================================
来源：http://shr.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://xti.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tzm.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ouq.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://avb.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://onf.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ahi.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://aha.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://uzi.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qbm.uphjek.com

[D02] 追加元素到末尾
来源：http://cmr.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oic.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ruw.yangfankeji.com

JS:   arr.push(4);
来源：http://riu.gogol.net.cn

TS:   arr.push(4);
来源：http://abv.jyoumei.cn

Java: list.add(4);
来源：http://rvo.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://yfz.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://iml.tianlin.xyz

C#:   list.Add(4);
来源：http://yco.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://evt.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://qnb.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rcy.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hww.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://qan.svipenyu.cn

Java: list.add(0, 0);
来源：http://kux.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://src.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://viu.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://jxf.sjlbkw.cn

[D04] 删除元素
来源：http://krz.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fqz.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qyb.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxx.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://zhg.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvr.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xdw.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aeh.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xys.yj202588.top

[D05] 访问与修改元素
来源：http://egn.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ctj.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blr.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zwr.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://nhl.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://edc.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://cay.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zxr.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tpc.vehdjk.com

[D06] 数组长度
来源：http://buk.zycfv.cn

Py:   len(arr)
来源：http://pfm.jlsjyb.cn

PHP:  count($arr);
来源：http://auf.zdqjudy.top

JS:   arr.length
来源：http://axs.yueranfly.top

TS:   arr.length
来源：http://zmw.hnxiangtu.top

Java: list.size();
来源：http://pfd.gzhubu.top

Go:   len(arr)
来源：http://mzb.smart0.xyz

Ruby: arr.length; arr.size
来源：http://vft.tian-w.cn

C#:   list.Count;
来源：http://dqu.tarul.cn

[D07] 切片 / 取子数组
来源：http://efw.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xpd.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://vgl.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://nko.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://qbv.dashuyun.cn

Java: list.subList(1, 4);
来源：http://uft.xziqi.cn

Go:   arr[1:4]
来源：http://awe.cqqwz.cn

Ruby: arr[1, 3]
来源：http://rli.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://byz.xuetiantiany.cn

[D08] 合并两个数组
来源：http://vrf.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://hjg.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://cai.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xff.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://vss.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ihg.jqgufenzy.top

Go:   append(a, b...)
来源：http://vgj.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://zwm.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://lny.xylfe.cn

[D09] 排序（升序）
来源：http://uuw.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://wkc.nanxuanxn.top

PHP:  sort($arr);
来源：http://mgf.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nrr.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dpi.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zta.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gtv.guowangkeji.top

Ruby: arr.sort
来源：http://elm.yongpay.top

C#:   list.Sort();
来源：http://xar.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpw.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wqr.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tat.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfl.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwq.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rtg.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bfz.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ksy.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ike.hfpthk.cn

[D11] 反转数组
来源：http://ysy.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bwf.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://xfp.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uyw.cucudq.cn

TS:   [...arr].reverse();
来源：http://lzd.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://rsq.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://iqs.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://ikr.xuetiantiany.cn

C#:   list.Reverse();
来源：http://smm.sysykeji.top

[D12] 查找元素下标
来源：http://jfg.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://lwq.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efn.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixd.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://als.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zjt.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://npv.hfpthk.cn

Ruby: arr.index(x)
来源：http://ckf.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://rjy.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://kek.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jec.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ucx.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://kpr.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://who.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mtj.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hmn.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://vie.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://shs.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://mve.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kua.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://urz.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://yoa.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://bia.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nih.hfpthk.cn

Go:   // 手写循环
来源：http://fhw.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://cky.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uzc.sweek.top

[D15] 去重
来源：http://ykd.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ewd.sweek.top

PHP:  array_unique($arr);
来源：http://qbj.gzhubu.top

JS:   [...new Set(arr)]
来源：http://atd.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://vuh.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ufc.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://hbt.yj202588.top

Ruby: arr.uniq
来源：http://twi.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://msq.nanxinkj.top

[D16] 求和与平均值
来源：http://aog.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nkm.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://evn.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fir.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsk.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yfq.52xcode.cn

Go:   // 手写循环累加
来源：http://xdr.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tre.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://dfm.havefunace.top

[D17] 最大值与最小值
来源：http://fgb.tanke756.top

Py:   max(arr);  min(arr)
来源：http://wqc.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://txx.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xyc.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://teo.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://msy.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://asn.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://qzv.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://ehf.birdmap.top

[D18] 扁平化嵌套数组
来源：http://kcp.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xht.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://ukq.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cdv.hongshengwenyu.top

TS:   nested.flat();
来源：http://btc.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nud.cashguo.top

Go:   // 手写双层循环
来源：http://dcy.cdnleiting.top

Ruby: nested.flatten
来源：http://pzh.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://jmu.316326.xyz

[D19] 按字段分组
来源：http://xcn.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ktz.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://moi.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qsy.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hcs.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzl.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://gln.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://doz.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tsh.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://mnb.jyoumei.cn

Py:   Counter(arr)
来源：http://kav.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://qet.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pra.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tub.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eyl.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://eyx.zhoulong.xyz

Ruby: arr.tally
来源：http://mwx.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fuc.yj20258888.top

[D21] 判断是否包含某元素
来源：http://xbp.jyoumei.cn

Py:   x in arr
来源：http://eno.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://cvq.hcnkem.com

JS:   arr.includes(x)
来源：http://fsm.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://bzb.zhiwuduotai.top

Java: list.contains(x)
来源：http://nnu.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://qtz.sufxvd.cn

Ruby: arr.include?(x)
来源：http://ski.cqqwz.cn

C#:   list.Contains(x)
来源：http://nqf.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://kki.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kkh.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nwo.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jcj.chenlongwang.top

TS:   [...arr];
来源：http://fkz.yuxming.cn

Java: new ArrayList<>(list);
来源：http://dck.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://ihd.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://iah.sysykeji.top

C#:   new List<int>(list);
来源：http://tfx.cashguo.top

[D23] reduce 累积计算
来源：http://ibh.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qze.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pkh.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://phk.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lgd.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://alc.fzhhl.top

Go:   // 手写循环
来源：http://lna.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vga.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fon.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://bxv.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bni.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://odn.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wxv.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xzg.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccl.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uof.smart0.xyz


<!-- 参考信息 -->