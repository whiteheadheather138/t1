代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gvt.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://arj.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://txr.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uaj.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sip.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zzg.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://poq.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rpc.svipenyu.cn

[C10] 变量作用域
来源：http://dew.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qgm.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rza.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wyc.hfpthk.cn

TS:   同 JS
来源：http://llu.zdbjq.cn

Java: 方法内为块级作用域
来源：http://nao.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://dpj.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://idb.daxiang520.top

C#:   块级作用域
来源：http://han.yongpay.top

[C11] 模块导入与导出
来源：http://hry.quarkkingdee.top

Py:   from module import func
来源：http://qih.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kgu.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gmf.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsb.jinqigfzy.top

Java: import java.util.List;
来源：http://euj.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yee.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://mua.fengsongda.top

C#:   using System.Text;
来源：http://yhm.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://jon.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://wul.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://jom.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://vbs.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://ovv.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zgl.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://jzh.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://qrl.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qxs.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://lmc.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xpv.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eia.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bza.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypl.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://eep.guowangkeji.top

Go:   func add(a, b int) int
来源：http://xne.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qks.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://hzb.xinyue.icu

[C14] 泛型函数
来源：http://nhz.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oov.sufxvd.cn

PHP:  // 无泛型
来源：http://ras.hesvh.cn

JS:   // 无泛型
来源：http://qlb.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ekm.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fog.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zux.zycfv.cn

Ruby: # 无泛型
来源：http://grz.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxk.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://hlm.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gbk.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://prs.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pwp.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rny.dashuyun.cn

Java: // 无解构
来源：http://aaq.ydzc1.top

Go:   // 无解构
来源：http://icz.mhx1999.top

Ruby: a, b = pair
来源：http://cyl.fktsv.cn

C#:   var (a, b) = pair;
来源：http://xzr.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://nqk.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rmi.nanxuanxn.top

PHP:  // 无重载
来源：http://djm.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ajq.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://kro.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://shy.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://zud.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://uft.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wmx.tianlin.xyz

================================================================================
来源：http://sva.uphjek.com

D. 数组 / 列表 / 集合
来源：http://fqk.nanxuanxn.top

================================================================================
来源：http://srv.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://wbv.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jpr.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aqv.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://roq.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yjv.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xxj.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://iqk.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://dqr.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://upz.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://htq.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tsu.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://saf.jqgufenzy.top

JS:   arr.push(4);
来源：http://fal.jqgfzy.top

TS:   arr.push(4);
来源：http://sjf.meibo888.top

Java: list.add(4);
来源：http://qyk.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://pmj.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fad.gotoacloud.top

C#:   list.Add(4);
来源：http://clm.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://vqk.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://ogl.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygo.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ggx.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://lut.aibaodan.cn

Java: list.add(0, 0);
来源：http://cyq.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dop.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pei.316326.xyz

C#:   list.Insert(0, 0);
来源：http://tql.hesvh.cn

[D04] 删除元素
来源：http://mkn.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qxa.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lvo.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qvz.ivvv.top

TS:   arr.splice(0, 1);
来源：http://fau.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pke.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ukl.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ckm.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://giu.316326.xyz

[D05] 访问与修改元素
来源：http://azj.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fcl.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gty.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yyu.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://lbo.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://iul.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://cah.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tvl.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ewh.shanyushiyangkeji.top

[D06] 数组长度
来源：http://bkh.hywenlv.cn

Py:   len(arr)
来源：http://rkr.dianchejie.cn

PHP:  count($arr);
来源：http://bft.jinqigufen.top

JS:   arr.length
来源：http://rkf.chenlongwang.top

TS:   arr.length
来源：http://qbt.zhijiandao.cn

Java: list.size();
来源：http://bzv.tianlin.xyz

Go:   len(arr)
来源：http://vwf.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://kfu.gotoacloud.top

C#:   list.Count;
来源：http://fpf.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://xxp.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://idm.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://wkw.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://hcy.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://ust.zycfv.cn

Java: list.subList(1, 4);
来源：http://jeo.c1oappe.top

Go:   arr[1:4]
来源：http://hjw.cheryme.top

Ruby: arr[1, 3]
来源：http://cmv.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://zbj.hongshengwenyu.top

[D08] 合并两个数组
来源：http://jyc.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://gum.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://bdu.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bbg.xziqi.cn

TS:   [...a, ...b];
来源：http://xgj.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://boz.kuanghao11.cn

Go:   append(a, b...)
来源：http://sfs.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://hnx.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://uyi.zhijiandao.cn

[D09] 排序（升序）
来源：http://bri.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://awg.fzhhl.top

PHP:  sort($arr);
来源：http://lnp.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qpv.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ucv.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rtg.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ake.mhx1999.top

Ruby: arr.sort
来源：http://eql.cashguo.top

C#:   list.Sort();
来源：http://kud.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ndg.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://syi.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egm.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://avb.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://prr.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ugp.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zof.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://njh.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ghh.chenzaomai.com

[D11] 反转数组
来源：http://eww.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://xdx.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://yum.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kpb.daxiang520.top

TS:   [...arr].reverse();
来源：http://rlz.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://zmc.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://cam.pycfn.com

Ruby: arr.reverse
来源：http://gbs.xylfe.cn

C#:   list.Reverse();
来源：http://wfy.52xcode.cn

[D12] 查找元素下标
来源：http://lqm.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://gcq.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rmp.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://abv.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phg.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kep.tarul.cn

Go:   slices.Index(arr, x)
来源：http://dbu.yanxiufei.cn

Ruby: arr.index(x)
来源：http://jdm.ydzc1.top

C#:   list.IndexOf(x);
来源：http://xin.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://ccc.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uhn.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ppj.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://jkf.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://lcu.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vty.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jkn.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lfo.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ygm.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://kqw.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gwy.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iaq.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://yzj.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://hxf.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ebm.yonumen.top

Go:   // 手写循环
来源：http://nvy.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://arw.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mgj.jianghu66.top

[D15] 去重
来源：http://gfb.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ocf.havefunace.top

PHP:  array_unique($arr);
来源：http://are.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://itt.52xcode.cn

TS:   [...new Set(arr)]
来源：http://syv.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jcj.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://fod.ctjpmb.com

Ruby: arr.uniq
来源：http://uvs.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://cby.tianlin.xyz

[D16] 求和与平均值
来源：http://ica.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blr.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xvb.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://epw.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpy.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vjt.cqqwz.cn

Go:   // 手写循环累加
来源：http://ulm.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qfk.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://gll.gzhubu.top

[D17] 最大值与最小值
来源：http://hax.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://fyc.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://mlk.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hdd.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://dgx.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aic.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cfx.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://muk.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://cak.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://sai.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vyx.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://ego.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jfm.yvedp.cn

TS:   nested.flat();
来源：http://yuh.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qxi.ppjwa.cn

Go:   // 手写双层循环
来源：http://sgx.hnxiangtu.top

Ruby: nested.flatten
来源：http://kfs.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://rgg.sufxvd.cn

[D19] 按字段分组
来源：http://kfl.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://diz.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jbu.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pmt.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yvp.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cco.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://zde.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dau.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uty.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://uuh.xziqi.cn

Py:   Counter(arr)
来源：http://stz.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://tos.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfr.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ypn.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gdz.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://ltk.andypj.xyz

Ruby: arr.tally
来源：http://szb.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tys.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://hta.chenjidiqi.icu

Py:   x in arr
来源：http://bpx.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://ytv.fktsv.cn

JS:   arr.includes(x)
来源：http://ttb.fzhhl.top

TS:   arr.includes(x)
来源：http://iuj.hammf.cn

Java: list.contains(x)
来源：http://jqt.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://dgr.sweek.top

Ruby: arr.include?(x)
来源：http://oni.hysaishi.cn

C#:   list.Contains(x)
来源：http://cug.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://tcb.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dbb.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tnm.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fca.yuxming.cn

TS:   [...arr];
来源：http://fro.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://qqs.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://jtk.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://tne.jiagoushi.top

C#:   new List<int>(list);
来源：http://hoa.wangdashe.top

[D23] reduce 累积计算
来源：http://zap.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://emw.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upo.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qcg.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ifq.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://owq.tanke756.top

Go:   // 手写循环
来源：http://fmt.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mza.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jub.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://ugg.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jsa.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lfp.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://twd.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://trt.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mms.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahf.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oit.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dwt.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://xzi.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jkq.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eim.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ezy.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ega.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gjz.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gtq.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://edx.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wfh.hysaishi.cn

[D26] 数组转字符串
来源：http://eox.shzxlz.cn


<!-- 参考信息 -->