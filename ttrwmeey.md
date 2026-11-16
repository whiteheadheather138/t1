代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lmv.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ilo.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cxh.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yom.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pbm.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kcu.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aql.cucudq.cn

[C09] 递归
来源：http://qrk.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nzn.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gbz.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lye.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sde.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mxx.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ixg.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ylh.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ttv.shangyingyoupin.top

[C10] 变量作用域
来源：http://vst.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hzg.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfx.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tcm.vehdjk.com

TS:   同 JS
来源：http://yhx.9152youxi.cn

Java: 方法内为块级作用域
来源：http://woq.jyoumei.cn

Go:   花括号块级作用域
来源：http://aul.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pkj.meibo888.top

C#:   块级作用域
来源：http://baq.zdbjq.cn

[C11] 模块导入与导出
来源：http://jro.zhixingplan.top

Py:   from module import func
来源：http://lbz.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://snj.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tke.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://onp.jlsjyb.cn

Java: import java.util.List;
来源：http://ujz.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rep.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://won.quarkkingdee.top

C#:   using System.Text;
来源：http://bxe.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://wcq.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://voh.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://pfx.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://uhx.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://wij.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rmo.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://era.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://ern.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qqi.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://lyl.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ynp.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asr.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jdy.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fut.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://lwi.chenzaomai.com

Go:   func add(a, b int) int
来源：http://fib.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qck.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://ahh.snrcjt.cn

[C14] 泛型函数
来源：http://xej.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dlw.52xcode.cn

PHP:  // 无泛型
来源：http://lhm.wangdashe.top

JS:   // 无泛型
来源：http://qvh.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bma.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fxr.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qgi.sxryk.cn

Ruby: # 无泛型
来源：http://iuk.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lwm.smart0.xyz

[C15] 解构 / 展开参数
来源：http://apm.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lji.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://axw.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jgp.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgu.shangyingyoupin.top

Java: // 无解构
来源：http://vcb.hcnkem.com

Go:   // 无解构
来源：http://vlb.sysykeji.top

Ruby: a, b = pair
来源：http://yvf.jianghu66.top

C#:   var (a, b) = pair;
来源：http://jjv.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://xct.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nac.fzhhl.top

PHP:  // 无重载
来源：http://mjk.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pxi.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://scq.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://dza.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://bhs.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://cpy.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ktl.tanke756.top

================================================================================
来源：http://bor.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://lrf.pengpengdd.cyou

================================================================================
来源：http://efr.xuanzx.com

[D01] 创建数组 / 列表
来源：http://bvv.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ayq.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jni.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lhh.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ncd.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lmc.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://dxh.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://zst.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://now.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://dwn.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcp.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fhq.hammf.cn

JS:   arr.push(4);
来源：http://cxz.c1oappe.top

TS:   arr.push(4);
来源：http://gxg.zhijiandao.cn

Java: list.add(4);
来源：http://acc.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://dhm.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://fri.0kj1m.cn

C#:   list.Add(4);
来源：http://iod.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://yxd.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://nuw.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bkr.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hyr.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://isz.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://dcj.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://xri.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nnd.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://ofu.hammf.cn

[D04] 删除元素
来源：http://pis.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jde.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://roc.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://edr.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://hpc.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gof.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://abv.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ysx.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://got.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://dpf.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bat.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lnm.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tfc.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://ykc.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://izt.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://vhd.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rwu.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqc.sysykeji.top

[D06] 数组长度
来源：http://orz.zycfv.cn

Py:   len(arr)
来源：http://qpx.ppjwa.cn

PHP:  count($arr);
来源：http://wya.jinyuanbaomall.cn

JS:   arr.length
来源：http://yrv.sxryk.cn

TS:   arr.length
来源：http://kea.jianghu66.top

Java: list.size();
来源：http://ong.9152youxi.cn

Go:   len(arr)
来源：http://vnq.meibo888.top

Ruby: arr.length; arr.size
来源：http://hlk.gotoacloud.top

C#:   list.Count;
来源：http://yep.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://vrr.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rcp.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://zvw.yj20258.top

JS:   arr.slice(1, 4);
来源：http://dwa.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://xhv.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://xeu.ivvv.top

Go:   arr[1:4]
来源：http://ort.snrcjt.cn

Ruby: arr[1, 3]
来源：http://pfq.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://vsv.sjlbkw.cn

[D08] 合并两个数组
来源：http://cfx.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://olq.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://hhp.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gwg.c1oappe.top

TS:   [...a, ...b];
来源：http://zvb.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eiv.wangdashe.top

Go:   append(a, b...)
来源：http://xeh.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://tdx.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://tfc.shuidangran.top

[D09] 排序（升序）
来源：http://fcs.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://goy.yj20258888.top

PHP:  sort($arr);
来源：http://wag.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gyf.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gof.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uol.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yui.52xcode.cn

Ruby: arr.sort
来源：http://cdf.yj20258.top

C#:   list.Sort();
来源：http://eio.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cst.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oct.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdb.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mzx.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cvy.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mxk.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://poh.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rxs.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xfv.fehbvm.com

[D11] 反转数组
来源：http://sai.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wew.sweek.top

PHP:  array_reverse($arr);
来源：http://yjk.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uzh.cqqwz.cn

TS:   [...arr].reverse();
来源：http://vpn.chenlongwang.top

Java: Collections.reverse(list);
来源：http://gtv.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://ssv.yueranfly.top

Ruby: arr.reverse
来源：http://vgk.gotoacloud.top

C#:   list.Reverse();
来源：http://jak.hnqzz.top

[D12] 查找元素下标
来源：http://fig.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://odp.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gcm.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sms.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dhm.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cxr.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://urz.hfpthk.cn

Ruby: arr.index(x)
来源：http://spm.tanke756.top

C#:   list.IndexOf(x);
来源：http://ygm.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://jjl.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eft.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yvz.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://gjt.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://jsm.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ftn.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xdw.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://qze.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cpg.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://vaj.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fkt.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zzc.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://uej.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://quz.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://shc.cheryme.top

Go:   // 手写循环
来源：http://thx.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://asu.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tko.jinqigfzy.top

[D15] 去重
来源：http://jxv.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://icr.tian-w.cn

PHP:  array_unique($arr);
来源：http://fjq.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://stj.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://awt.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vqx.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://poo.jqgufenzy.top

Ruby: arr.uniq
来源：http://gkg.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://hcf.nanxinkj.top

[D16] 求和与平均值
来源：http://nrx.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hmh.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kbf.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqe.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ygv.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tgl.yuxming.cn

Go:   // 手写循环累加
来源：http://maj.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exc.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://loc.yonumen.top

[D17] 最大值与最小值
来源：http://far.ppjwa.cn

Py:   max(arr);  min(arr)
来源：http://mzv.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://gzi.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dsl.ctjpmb.com

TS:   Math.max(...arr);
来源：http://dxr.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ldt.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymp.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://guk.hammf.cn

C#:   list.Max();  list.Min()
来源：http://vay.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://dkz.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xqo.hammf.cn

PHP:  array_merge(...$nested);
来源：http://yjd.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://njh.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://ojk.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kku.hfpthk.cn

Go:   // 手写双层循环
来源：http://iyw.pycfn.com

Ruby: nested.flatten
来源：http://skl.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://pky.birdmap.top

[D19] 按字段分组
来源：http://pvo.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wdz.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ife.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cku.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nur.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abr.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://pzp.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://vos.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zyv.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://pil.xziqi.cn

Py:   Counter(arr)
来源：http://kyh.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://efz.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pla.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdf.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tnu.zycfv.cn

Go:   // 手写 map[T]int
来源：http://ktt.nanxinkj.top

Ruby: arr.tally
来源：http://fdf.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lzk.pycfn.com

[D21] 判断是否包含某元素
来源：http://rip.shzxlz.cn

Py:   x in arr
来源：http://rrg.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://wdn.chenzaomai.com

JS:   arr.includes(x)
来源：http://prz.yfazqb.com

TS:   arr.includes(x)
来源：http://flk.birdmap.top

Java: list.contains(x)
来源：http://szc.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://gmu.jiagoushi.top

Ruby: arr.include?(x)
来源：http://glb.xinyue.icu

C#:   list.Contains(x)
来源：http://kfe.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://yno.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dtr.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zmo.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fgn.yuanzhike.top

TS:   [...arr];
来源：http://sgf.fzhhl.top

Java: new ArrayList<>(list);
来源：http://ian.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://cvf.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://bum.jianghu66.top

C#:   new List<int>(list);
来源：http://qkk.shuidangran.top

[D23] reduce 累积计算
来源：http://lwo.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zsg.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rwi.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igm.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfc.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ial.havefunace.top

Go:   // 手写循环
来源：http://tqk.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://itw.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://khz.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://lmq.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rtn.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kop.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://txc.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://thg.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aqd.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rnf.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cnw.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uck.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://gah.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzl.zhixingplan.top


<!-- 参考信息 -->