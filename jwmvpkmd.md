代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://vzu.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ygo.jiagoushi.top

Java: import java.util.List;
来源：http://tlx.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lbt.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://pji.pengpengdd.cyou

C#:   using System.Text;
来源：http://itb.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://xgc.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://ikd.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://sfu.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://mzp.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://yjf.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aou.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://cmz.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://euu.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nka.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://eia.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://osh.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pwl.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zni.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrd.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fkz.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://gfm.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cth.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://uxh.bjfxy.top

[C14] 泛型函数
来源：http://jdz.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qyf.sxryk.cn

PHP:  // 无泛型
来源：http://fwb.yj20258888.top

JS:   // 无泛型
来源：http://cgw.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ong.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zva.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xvy.jqgfzy.top

Ruby: # 无泛型
来源：http://lrs.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://say.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://uyi.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vvj.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://efg.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nbz.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdg.bjfxy.top

Java: // 无解构
来源：http://lwa.fanxiaobao.xyz

Go:   // 无解构
来源：http://xee.chenlongwang.top

Ruby: a, b = pair
来源：http://fpr.cheryme.top

C#:   var (a, b) = pair;
来源：http://gcn.yueranfly.top

[C16] 函数 / 方法重载
来源：http://xqh.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fmt.cdnleiting.top

PHP:  // 无重载
来源：http://ytd.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oox.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://nvg.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zkb.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://dll.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://uuy.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ypl.quarkkingdee.top

================================================================================
来源：http://xns.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://dyy.zhongyouzk.top

================================================================================
来源：http://fie.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://yjm.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://osz.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cuk.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wqd.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zqq.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oeu.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://cyk.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://yej.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://drm.c1oappe.top

[D02] 追加元素到末尾
来源：http://nvl.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://syt.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jyr.yj20258888.top

JS:   arr.push(4);
来源：http://daj.zhongyouzk.top

TS:   arr.push(4);
来源：http://utc.yfazqb.com

Java: list.add(4);
来源：http://gfl.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://jwa.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://nom.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://fdx.havefunace.top

[D03] 在指定位置插入元素
来源：http://pzb.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://zcu.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gsd.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bdw.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://jwa.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://kic.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://ach.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gxf.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://pej.nanxuanxn.top

[D04] 删除元素
来源：http://cog.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vma.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rqk.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tii.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://nfj.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hqh.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tzn.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wri.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yug.ctjpmb.com

[D05] 访问与修改元素
来源：http://nlt.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://klw.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cak.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pzv.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://bop.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://wug.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://kow.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dqt.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://akb.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://vsx.fengsongda.top

Py:   len(arr)
来源：http://jyl.epnwcf.com

PHP:  count($arr);
来源：http://okf.cashguo.top

JS:   arr.length
来源：http://ces.xylfe.cn

TS:   arr.length
来源：http://pld.xziqi.cn

Java: list.size();
来源：http://poa.smart0.xyz

Go:   len(arr)
来源：http://qsc.cucudq.cn

Ruby: arr.length; arr.size
来源：http://qcx.haohaochexian.top

C#:   list.Count;
来源：http://bvk.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://jin.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wrw.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://sxl.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://kqg.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://mqx.jinqigufen.top

Java: list.subList(1, 4);
来源：http://fyo.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://frb.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://fwq.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://hkl.jinqigfzy.top

[D08] 合并两个数组
来源：http://kyt.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://zfz.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://ilv.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://huh.yanxiufei.cn

TS:   [...a, ...b];
来源：http://oll.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aip.316326.xyz

Go:   append(a, b...)
来源：http://mze.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://ral.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://yrk.guowangkeji.top

[D09] 排序（升序）
来源：http://sju.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://ggr.daxiang520.top

PHP:  sort($arr);
来源：http://cjb.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzh.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://deu.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hui.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ano.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://iac.zdqjudy.top

C#:   list.Sort();
来源：http://ctu.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://mke.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://alr.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://upz.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tix.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rft.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://thj.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jue.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zqd.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pyf.yonumen.top

[D11] 反转数组
来源：http://ilg.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://rnf.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://ynt.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zxr.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://ekt.zhixingplan.top

Java: Collections.reverse(list);
来源：http://wcx.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://pcr.haohaochexian.top

Ruby: arr.reverse
来源：http://oxt.shzxlz.cn

C#:   list.Reverse();
来源：http://ely.shuidangran.top

[D12] 查找元素下标
来源：http://szt.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://pqh.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kbh.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xug.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ncc.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://isk.yonumen.top

Go:   slices.Index(arr, x)
来源：http://pmi.uphjek.com

Ruby: arr.index(x)
来源：http://yww.52xcode.cn

C#:   list.IndexOf(x);
来源：http://mjc.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://kqz.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ugs.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lwv.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://nwb.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://twa.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gnn.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lal.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tvq.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cup.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://buv.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://btx.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dvs.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://rei.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://lnw.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cgs.shzxlz.cn

Go:   // 手写循环
来源：http://nhc.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://bjj.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kvr.cashguo.top

[D15] 去重
来源：http://akf.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ouz.tarul.cn

PHP:  array_unique($arr);
来源：http://boj.52xcode.cn

JS:   [...new Set(arr)]
来源：http://xii.yj20258888.top

TS:   [...new Set(arr)]
来源：http://ujf.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ana.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://mcg.guowangkeji.top

Ruby: arr.uniq
来源：http://wvs.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://crh.yangfankeji.com

[D16] 求和与平均值
来源：http://xju.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ycb.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://quw.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gsq.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bsn.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://azi.bbcook.cn

Go:   // 手写循环累加
来源：http://mbb.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bsy.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://rdy.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://wli.yonumen.top

Py:   max(arr);  min(arr)
来源：http://ejs.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://pjv.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aes.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://loq.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mnu.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gjy.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://fgg.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://wnc.sweek.top

[D18] 扁平化嵌套数组
来源：http://vhp.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujm.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://rwc.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bei.yonumen.top

TS:   nested.flat();
来源：http://pcn.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rwn.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://vds.zdqjudy.top

Ruby: nested.flatten
来源：http://woh.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cxs.birdmap.top

[D19] 按字段分组
来源：http://ram.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iaf.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ynv.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cjb.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kxa.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://izb.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://yeb.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wvy.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fqb.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://viu.ehwqpu.com

Py:   Counter(arr)
来源：http://gjd.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nji.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eah.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qeh.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ljb.nwbrower.top

Go:   // 手写 map[T]int
来源：http://apq.zhoulong.xyz

Ruby: arr.tally
来源：http://hhs.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rhm.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://qce.epnwcf.com

Py:   x in arr
来源：http://icu.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://qun.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://uyd.dianchejie.cn

TS:   arr.includes(x)
来源：http://hww.hysaishi.cn

Java: list.contains(x)
来源：http://lpw.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://eet.fehbvm.com

Ruby: arr.include?(x)
来源：http://rzb.aizwys.cn

C#:   list.Contains(x)
来源：http://mwl.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://apl.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vjf.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ljw.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iif.ybcxt.top

TS:   [...arr];
来源：http://vap.hammf.cn

Java: new ArrayList<>(list);
来源：http://sgb.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://quw.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://lxh.yangfankeji.com

C#:   new List<int>(list);
来源：http://wdq.sxryk.cn

[D23] reduce 累积计算
来源：http://xgy.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://woc.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hun.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnq.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyi.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tvb.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://mhj.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bkz.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wxt.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://qkt.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dov.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iup.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ybl.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xsm.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nnj.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ikt.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kjm.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hzj.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://ylv.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jdm.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ukv.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ixy.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kju.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tep.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ewg.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gbh.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rqb.mhx1999.top

[D26] 数组转字符串
来源：http://xba.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://pih.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://ozi.cqqwz.cn

JS:   arr.join(", ")
来源：http://suv.hammf.cn

TS:   arr.join(", ")
来源：http://wby.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://bjj.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://dhs.316326.xyz

Ruby: arr.join(", ")
来源：http://qxe.smart0.xyz

C#:   string.Join(", ", list)
来源：http://hbn.ybcxt.top

================================================================================
来源：http://jdl.nwbrower.top

E. 字符串处理
来源：http://shy.iojbl.cn

================================================================================
来源：http://ydy.hnqzz.top

[E01] 拼接字符串
来源：http://jsx.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://byd.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icd.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvc.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ekv.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ugu.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wwq.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://scl.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qgm.bjfxy.top


<!-- 参考信息 -->