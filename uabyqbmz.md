代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://abo.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pfz.wangshuangyany.cn

[C08] 闭包
来源：http://pjj.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tvr.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ygt.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://quf.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pwx.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ebv.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mtz.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cpc.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zez.shanyushiyangtech.top

[C09] 递归
来源：http://evy.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zam.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://byc.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qyb.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkm.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uet.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pwp.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bqw.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxx.daria6918.cn

[C10] 变量作用域
来源：http://owh.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ivm.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://puo.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://czv.birdmap.top

TS:   同 JS
来源：http://ocz.yj202588.top

Java: 方法内为块级作用域
来源：http://bxw.aibaodan.cn

Go:   花括号块级作用域
来源：http://sxj.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lsk.jyoumei.cn

C#:   块级作用域
来源：http://kfs.snrcjt.cn

[C11] 模块导入与导出
来源：http://ldf.sufxvd.cn

Py:   from module import func
来源：http://jvp.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iey.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zsx.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jcu.aibaodan.cn

Java: import java.util.List;
来源：http://wcn.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lod.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://njm.daria6918.cn

C#:   using System.Text;
来源：http://mel.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://rpn.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://cqm.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://jck.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://tjv.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://vet.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifm.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://kiv.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://yzq.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zfr.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://gdd.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bsc.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wtl.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qxt.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtj.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://pyb.cheryme.top

Go:   func add(a, b int) int
来源：http://hqt.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eql.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://rym.sufxvd.cn

[C14] 泛型函数
来源：http://tii.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kvw.tanke756.top

PHP:  // 无泛型
来源：http://nvx.cheryme.top

JS:   // 无泛型
来源：http://wml.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lfh.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rse.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yix.vqdsnc.cn

Ruby: # 无泛型
来源：http://csl.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mmx.yueranfly.top

[C15] 解构 / 展开参数
来源：http://bea.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kdf.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://ilm.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zsi.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gri.kuanghao11.cn

Java: // 无解构
来源：http://bcn.sxryk.cn

Go:   // 无解构
来源：http://ola.yvedp.cn

Ruby: a, b = pair
来源：http://cbt.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://bit.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://vpe.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gxv.yj202588.top

PHP:  // 无重载
来源：http://smq.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lsi.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://unv.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://wje.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://btq.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://clb.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://emh.bjfxy.top

================================================================================
来源：http://bnh.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://qka.jqgfzy.top

================================================================================
来源：http://apt.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://guu.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iwb.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fvq.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukh.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://agj.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpc.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://uin.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://pcn.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uhv.vehdjk.com

[D02] 追加元素到末尾
来源：http://mus.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cma.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwt.iojbl.cn

JS:   arr.push(4);
来源：http://gtt.sysykeji.top

TS:   arr.push(4);
来源：http://sqa.xuanzx.com

Java: list.add(4);
来源：http://kji.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://kja.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://hui.uphjek.com

C#:   list.Add(4);
来源：http://pju.316326.xyz

[D03] 在指定位置插入元素
来源：http://tqf.birdmap.top

Py:   arr.insert(0, 0)
来源：http://xlk.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rvj.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hha.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://fln.tianlin.xyz

Java: list.add(0, 0);
来源：http://ouy.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ypp.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://idd.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://fji.haohaochexian.top

[D04] 删除元素
来源：http://mae.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pfs.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vpf.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dwr.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://ytp.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gge.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cjz.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tze.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vww.tianlin.xyz

[D05] 访问与修改元素
来源：http://map.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oas.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://twq.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ayj.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://kum.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://krg.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://gqb.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ufs.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmd.hcnkem.com

[D06] 数组长度
来源：http://zaz.gogol.net.cn

Py:   len(arr)
来源：http://aci.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://mce.hnqzz.top

JS:   arr.length
来源：http://hqd.shanyushiyangkeji.top

TS:   arr.length
来源：http://uzs.gogol.net.cn

Java: list.size();
来源：http://jmd.cashguo.top

Go:   len(arr)
来源：http://ibg.epnwcf.com

Ruby: arr.length; arr.size
来源：http://hlr.ppjwa.cn

C#:   list.Count;
来源：http://uyc.yfazqb.com

[D07] 切片 / 取子数组
来源：http://dsb.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jeh.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fab.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://qkb.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://dfh.smart0.xyz

Java: list.subList(1, 4);
来源：http://tac.yfazqb.com

Go:   arr[1:4]
来源：http://akm.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://yxx.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://avj.jqgufenzy.top

[D08] 合并两个数组
来源：http://zwt.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://drs.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://vdz.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://pds.daria6918.cn

TS:   [...a, ...b];
来源：http://xaa.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://omh.yuxming.cn

Go:   append(a, b...)
来源：http://tfi.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://far.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://ura.sufxvd.cn

[D09] 排序（升序）
来源：http://kgg.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ain.yongpay.top

PHP:  sort($arr);
来源：http://ozp.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ekp.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qpn.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://foz.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjl.jqgufenzy.top

Ruby: arr.sort
来源：http://ywg.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://dke.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bkk.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bsx.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvc.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://loy.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzl.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://khx.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://grt.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wug.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rqe.guannengcc.top

[D11] 反转数组
来源：http://znt.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yrq.hnqzz.top

PHP:  array_reverse($arr);
来源：http://vrn.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://keo.shzxlz.cn

TS:   [...arr].reverse();
来源：http://ezd.tianlin.xyz

Java: Collections.reverse(list);
来源：http://gue.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://zfu.hammf.cn

Ruby: arr.reverse
来源：http://scx.xziqi.cn

C#:   list.Reverse();
来源：http://ovf.meibo888.top

[D12] 查找元素下标
来源：http://ywy.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://cud.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nje.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hud.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kfa.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yhn.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://lwl.sjlbkw.cn

Ruby: arr.index(x)
来源：http://crz.fengsongda.top

C#:   list.IndexOf(x);
来源：http://zhw.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://yhf.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eqe.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dni.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://tvy.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://hhz.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rgj.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hjy.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zeu.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sme.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://tjd.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kqc.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mwr.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ozs.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://kuh.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gpf.yanxiufei.cn

Go:   // 手写循环
来源：http://omm.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://ugw.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pkd.smart0.xyz

[D15] 去重
来源：http://fbw.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://knv.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://sce.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://ryx.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://beh.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ykx.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://mpc.yueranfly.top

Ruby: arr.uniq
来源：http://igc.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://mqp.snrcjt.cn

[D16] 求和与平均值
来源：http://rbc.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://glb.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ttm.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iwe.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gwz.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dcf.316326.xyz

Go:   // 手写循环累加
来源：http://nug.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lol.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://neo.yuanzhike.top

[D17] 最大值与最小值
来源：http://ilf.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://srn.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://ore.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://twk.bbcook.cn

TS:   Math.max(...arr);
来源：http://lmr.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oyb.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sts.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://mmv.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://uxw.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://idq.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uvh.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://ogx.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dsw.uphjek.com

TS:   nested.flat();
来源：http://jfp.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tea.316326.xyz

Go:   // 手写双层循环
来源：http://odw.ppjwa.cn

Ruby: nested.flatten
来源：http://vml.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://olz.chenlongwang.top

[D19] 按字段分组
来源：http://jdy.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kah.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xzy.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mpd.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://vop.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hym.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://jky.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://esi.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dls.meibo888.top

[D20] 统计每个元素出现次数
来源：http://onv.zdbjq.cn

Py:   Counter(arr)
来源：http://zwd.yonumen.top

PHP:  array_count_values($arr);
来源：http://klz.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ojj.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sof.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dzl.yuxming.cn

Go:   // 手写 map[T]int
来源：http://kle.guowangkeji.top

Ruby: arr.tally
来源：http://luq.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zxg.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://mgl.ydjk.org.cn

Py:   x in arr
来源：http://ovp.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://aht.pycfn.com

JS:   arr.includes(x)
来源：http://xeo.gotoacloud.top

TS:   arr.includes(x)
来源：http://kpg.c1oappe.top

Java: list.contains(x)
来源：http://prc.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://lbs.hcnkem.com

Ruby: arr.include?(x)
来源：http://mwc.wangdashe.top

C#:   list.Contains(x)
来源：http://ura.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://xes.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jak.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://odg.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jnz.yueranfly.top

TS:   [...arr];
来源：http://vyp.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://xti.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rjt.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://qkh.meibo888.top

C#:   new List<int>(list);
来源：http://znk.zhoulong.xyz

[D23] reduce 累积计算
来源：http://pjb.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rgn.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uik.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmm.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://khn.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ony.bbcook.cn

Go:   // 手写循环
来源：http://kux.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://klj.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mop.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://lck.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hur.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ogv.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otv.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nun.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xfy.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://acq.sysykeji.top


<!-- 参考信息 -->