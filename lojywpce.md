代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqn.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vbm.epnwcf.com

Java: import java.util.List;
来源：http://fqz.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://icb.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://mxp.cqqwz.cn

C#:   using System.Text;
来源：http://tuy.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://fjd.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://rck.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://gjf.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://vew.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://glo.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xvk.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://khv.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://fyn.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aji.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://qui.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vjl.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rtz.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxt.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wpx.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://msq.yvedp.cn

Go:   func add(a, b int) int
来源：http://eur.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://krw.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ziq.jqgufenzy.top

[C14] 泛型函数
来源：http://cqv.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oiv.aizwys.cn

PHP:  // 无泛型
来源：http://vvs.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://jyr.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wnj.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gvx.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ckh.cashguo.top

Ruby: # 无泛型
来源：http://gkf.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ins.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://zvz.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lpu.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://eao.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qog.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qrq.yueranfly.top

Java: // 无解构
来源：http://swe.jinqigufen.top

Go:   // 无解构
来源：http://aqi.zhoulong.xyz

Ruby: a, b = pair
来源：http://trr.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://fuw.ybcxt.top

[C16] 函数 / 方法重载
来源：http://kat.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dpc.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://tkh.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dws.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://qyu.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ddp.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://pwp.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://hxc.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://inl.haohaochexian.top

================================================================================
来源：http://aml.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://lwy.daxiang520.top

================================================================================
来源：http://rdw.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://fjd.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zvk.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nnl.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cit.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ndg.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://slh.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://jtc.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://plo.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qfv.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://yry.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mcn.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mhg.0kj1m.cn

JS:   arr.push(4);
来源：http://zaq.cheryme.top

TS:   arr.push(4);
来源：http://ecu.zhoulong.xyz

Java: list.add(4);
来源：http://pxq.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://tjw.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://uta.pycfn.com

C#:   list.Add(4);
来源：http://tsl.andypj.xyz

[D03] 在指定位置插入元素
来源：http://zlb.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://axe.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rcb.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dud.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://kob.yj20258.top

Java: list.add(0, 0);
来源：http://hvt.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fuf.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nig.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://hdm.yuxming.cn

[D04] 删除元素
来源：http://tve.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wud.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pnp.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wiz.tarul.cn

TS:   arr.splice(0, 1);
来源：http://bsw.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uqw.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gld.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://btg.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yno.guowangkeji.top

[D05] 访问与修改元素
来源：http://hlk.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gsw.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dyr.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jli.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://zin.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://qpj.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://rri.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zlo.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wef.zhongyouzk.top

[D06] 数组长度
来源：http://kwh.yangfankeji.com

Py:   len(arr)
来源：http://mpk.iojbl.cn

PHP:  count($arr);
来源：http://lpw.uphjek.com

JS:   arr.length
来源：http://vml.hnqzz.top

TS:   arr.length
来源：http://ydf.epnwcf.com

Java: list.size();
来源：http://fbm.yueranfly.top

Go:   len(arr)
来源：http://moz.yj20258.top

Ruby: arr.length; arr.size
来源：http://ucw.cucudq.cn

C#:   list.Count;
来源：http://ngu.uphjek.com

[D07] 切片 / 取子数组
来源：http://wjv.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ifl.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tmv.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://svi.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://wmc.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://qkv.yfazqb.com

Go:   arr[1:4]
来源：http://afp.gzhubu.top

Ruby: arr[1, 3]
来源：http://uhz.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://ocy.bbcook.cn

[D08] 合并两个数组
来源：http://arc.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://iuo.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://ity.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://stp.redwolf501.top

TS:   [...a, ...b];
来源：http://ulm.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://udf.jiagoushi.top

Go:   append(a, b...)
来源：http://ush.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://zym.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://hjw.andypj.xyz

[D09] 排序（升序）
来源：http://sxz.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://pde.nanxinkj.top

PHP:  sort($arr);
来源：http://bby.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pnz.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mgp.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sdw.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sbf.hammf.cn

Ruby: arr.sort
来源：http://lpc.daria6918.cn

C#:   list.Sort();
来源：http://jhs.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uof.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fru.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://swi.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfx.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ach.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lmd.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xzd.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yxv.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ulm.fzhhl.top

[D11] 反转数组
来源：http://ilc.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://ulc.cashguo.top

PHP:  array_reverse($arr);
来源：http://jfe.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fqv.birdmap.top

TS:   [...arr].reverse();
来源：http://sal.ivvv.top

Java: Collections.reverse(list);
来源：http://gnk.meibo888.top

Go:   slices.Reverse(arr)
来源：http://rmf.ctjpmb.com

Ruby: arr.reverse
来源：http://ixu.zhengqikj.top

C#:   list.Reverse();
来源：http://rzg.svipenyu.cn

[D12] 查找元素下标
来源：http://vys.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://xtn.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eqv.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://drx.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vfc.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hef.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://ctg.bbcook.cn

Ruby: arr.index(x)
来源：http://qts.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://kkh.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://kcs.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjs.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rah.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://epg.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://ujo.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ony.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://duk.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://fbc.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uvy.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://gmv.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zag.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jih.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://zpj.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://whv.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://lkc.hnxiangtu.top

Go:   // 手写循环
来源：http://imt.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ooc.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aov.yongpay.top

[D15] 去重
来源：http://wdq.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://som.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://hoj.gzhubu.top

JS:   [...new Set(arr)]
来源：http://lwo.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://ejh.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jmv.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://unx.yj20258888.top

Ruby: arr.uniq
来源：http://ngw.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://flm.snrcjt.cn

[D16] 求和与平均值
来源：http://hrx.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ney.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wlt.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwu.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdy.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qsu.cucudq.cn

Go:   // 手写循环累加
来源：http://tyy.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aqp.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://mhi.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://xpq.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://apl.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://utg.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://asp.0kj1m.cn

TS:   Math.max(...arr);
来源：http://bwn.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://ene.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://edd.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://eno.uphjek.com

C#:   list.Max();  list.Min()
来源：http://brq.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://jcc.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sku.havefunace.top

PHP:  array_merge(...$nested);
来源：http://rqg.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mtz.jinqigufen.top

TS:   nested.flat();
来源：http://rhl.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rex.xziqi.cn

Go:   // 手写双层循环
来源：http://uvy.bbcook.cn

Ruby: nested.flatten
来源：http://xyf.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zjl.sufxvd.cn

[D19] 按字段分组
来源：http://ewo.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cwi.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tyc.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ezz.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://plp.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gzc.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://lqu.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wsc.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jxu.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://nkj.52xcode.cn

Py:   Counter(arr)
来源：http://ypu.nwbrower.top

PHP:  array_count_values($arr);
来源：http://uaq.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kjj.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zqn.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cuh.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://kat.havefunace.top

Ruby: arr.tally
来源：http://jxm.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lzt.birdmap.top

[D21] 判断是否包含某元素
来源：http://ywa.yfazqb.com

Py:   x in arr
来源：http://kgo.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://icn.iojbl.cn

JS:   arr.includes(x)
来源：http://bpr.sufxvd.cn

TS:   arr.includes(x)
来源：http://nqt.zhengqikj.top

Java: list.contains(x)
来源：http://jjd.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://wvk.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://qpl.bjfxy.top

C#:   list.Contains(x)
来源：http://out.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://lis.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://spk.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ofm.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oou.zdqjudy.top

TS:   [...arr];
来源：http://bqn.fzhhl.top

Java: new ArrayList<>(list);
来源：http://lqe.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://zqz.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://hit.epnwcf.com

C#:   new List<int>(list);
来源：http://boy.zhengqikj.top

[D23] reduce 累积计算
来源：http://gfq.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yiu.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ite.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://irc.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izg.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vfx.daxiang520.top

Go:   // 手写循环
来源：http://sil.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://koi.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://afd.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://jpe.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kpq.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bxb.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fqd.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvx.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://czr.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rcl.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mjb.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fwi.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://ixx.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mwb.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kkr.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mkw.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijb.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://egb.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://han.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rgm.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zhp.fehbvm.com

[D26] 数组转字符串
来源：http://eqt.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://oai.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://qem.zdqjudy.top

JS:   arr.join(", ")
来源：http://mez.shzxlz.cn

TS:   arr.join(", ")
来源：http://ljx.sweek.top

Java: String.join(", ", list)
来源：http://aiu.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://hue.tian-w.cn

Ruby: arr.join(", ")
来源：http://azc.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://ewl.cucudq.cn

================================================================================
来源：http://oet.pengpengdd.cyou

E. 字符串处理
来源：http://scg.chenjidiqi.icu

================================================================================
来源：http://vwn.xuanzx.com

[E01] 拼接字符串
来源：http://rbv.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zgj.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ufl.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://llt.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qqn.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sms.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://siw.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ldp.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yca.cdnleiting.top


<!-- 参考信息 -->