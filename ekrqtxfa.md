代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://guk.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jvc.guannengcc.top

Java: import java.util.List;
来源：http://orv.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bnl.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://plg.fzhhl.top

C#:   using System.Text;
来源：http://zby.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://pll.hammf.cn

Py:   (lambda: print("run"))()
来源：http://ctx.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://wov.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://nvs.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://hyl.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ruq.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://kwj.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ywm.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fdf.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://ytn.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lgc.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dvz.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mie.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zss.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://tqn.yuxming.cn

Go:   func add(a, b int) int
来源：http://yxz.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cov.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://bqn.ydjk.org.cn

[C14] 泛型函数
来源：http://pyy.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lzc.cucudq.cn

PHP:  // 无泛型
来源：http://kjb.nanxinkj.top

JS:   // 无泛型
来源：http://sck.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pwq.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nps.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fsq.cucudq.cn

Ruby: # 无泛型
来源：http://tzv.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kwm.hnqzz.top

[C15] 解构 / 展开参数
来源：http://qjq.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rhe.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://osu.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxg.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqh.ydjk.org.cn

Java: // 无解构
来源：http://fot.jinyuanbaomall.cn

Go:   // 无解构
来源：http://lni.hesvh.cn

Ruby: a, b = pair
来源：http://ajn.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://utq.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://bvh.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lnn.jinqigfzy.top

PHP:  // 无重载
来源：http://wtq.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://auc.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://sgb.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://beq.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://ftl.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://gtl.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yof.jinqigfzy.top

================================================================================
来源：http://lii.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://xmh.gotoacloud.top

================================================================================
来源：http://rbp.bjfxy.top

[D01] 创建数组 / 列表
来源：http://dxj.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gnv.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uka.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://upc.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kcw.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xrl.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://txd.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://qmm.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rav.yangfankeji.com

[D02] 追加元素到末尾
来源：http://zvf.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sog.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wti.ybcxt.top

JS:   arr.push(4);
来源：http://wev.dashuyun.cn

TS:   arr.push(4);
来源：http://csw.jinyuanbaomall.cn

Java: list.add(4);
来源：http://tji.yonumen.top

Go:   arr = append(arr, 4)
来源：http://aod.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://pbe.316326.xyz

C#:   list.Add(4);
来源：http://aba.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://fxm.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://svi.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://waf.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bod.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://mau.fzhhl.top

Java: list.add(0, 0);
来源：http://yfp.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://vvm.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bvi.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://iwl.hcnkem.com

[D04] 删除元素
来源：http://qoc.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pdm.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ioh.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gev.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://yob.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mza.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uij.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cco.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fbf.sysykeji.top

[D05] 访问与修改元素
来源：http://hkh.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sgp.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ghx.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mcr.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://cam.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://yfo.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://zxt.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yyh.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cfa.ctjpmb.com

[D06] 数组长度
来源：http://gsb.xziqi.cn

Py:   len(arr)
来源：http://vuv.ivvv.top

PHP:  count($arr);
来源：http://hhy.snrcjt.cn

JS:   arr.length
来源：http://pei.nanxinkj.top

TS:   arr.length
来源：http://epi.snrcjt.cn

Java: list.size();
来源：http://elo.fzhhl.top

Go:   len(arr)
来源：http://njw.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://sxv.kuanghao11.cn

C#:   list.Count;
来源：http://zzr.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://zhm.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://waw.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gja.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://ike.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://bzy.zycfv.cn

Java: list.subList(1, 4);
来源：http://zwt.zhongyouzk.top

Go:   arr[1:4]
来源：http://rgj.zdqjudy.top

Ruby: arr[1, 3]
来源：http://gpz.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://kzn.iojbl.cn

[D08] 合并两个数组
来源：http://kzd.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://xjn.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://kqa.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nyh.cheryme.top

TS:   [...a, ...b];
来源：http://wxh.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tay.cheryme.top

Go:   append(a, b...)
来源：http://aks.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://zoe.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://ywc.iojbl.cn

[D09] 排序（升序）
来源：http://exq.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dep.smart0.xyz

PHP:  sort($arr);
来源：http://obj.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://adz.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kdc.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://nsq.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyv.fanxiaobao.xyz

Ruby: arr.sort
来源：http://nig.yj20258888.top

C#:   list.Sort();
来源：http://zcf.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjq.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vmc.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aks.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://shk.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://khx.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rpi.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://prd.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ljq.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tmo.cqqwz.cn

[D11] 反转数组
来源：http://oxd.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hhs.fzhhl.top

PHP:  array_reverse($arr);
来源：http://siz.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jnz.yfazqb.com

TS:   [...arr].reverse();
来源：http://sjv.316326.xyz

Java: Collections.reverse(list);
来源：http://wkp.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://imc.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://jot.ctjpmb.com

C#:   list.Reverse();
来源：http://ojy.cqqwz.cn

[D12] 查找元素下标
来源：http://esb.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://zwh.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pwr.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uon.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iln.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jmf.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://vwh.tanke756.top

Ruby: arr.index(x)
来源：http://nvk.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://yyp.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://bcn.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hns.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fxn.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://isn.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://ycg.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjm.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jgv.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://wpb.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jsi.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://lqk.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xwv.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tlz.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://yxr.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://epk.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mkc.sjlbkw.cn

Go:   // 手写循环
来源：http://rce.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://lgo.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://wmu.zhiwuduotai.top

[D15] 去重
来源：http://qac.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://psx.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://mco.hnqzz.top

JS:   [...new Set(arr)]
来源：http://rfg.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://zqi.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cvx.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://izs.zdqjudy.top

Ruby: arr.uniq
来源：http://ytd.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://jsn.bjfxy.top

[D16] 求和与平均值
来源：http://krt.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hpt.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wyu.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcl.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vef.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uzs.vqdsnc.cn

Go:   // 手写循环累加
来源：http://ljr.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fqv.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://xxa.snrcjt.cn

[D17] 最大值与最小值
来源：http://haq.ppjwa.cn

Py:   max(arr);  min(arr)
来源：http://bry.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://bsv.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ttp.zhixingplan.top

TS:   Math.max(...arr);
来源：http://sue.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zxn.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xdu.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://mvn.hammf.cn

C#:   list.Max();  list.Min()
来源：http://vhi.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://yjs.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nuu.yonumen.top

PHP:  array_merge(...$nested);
来源：http://ehu.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lqe.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://npp.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwf.birdmap.top

Go:   // 手写双层循环
来源：http://ova.jinqigfzy.top

Ruby: nested.flatten
来源：http://css.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://azu.cashguo.top

[D19] 按字段分组
来源：http://cnu.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://omm.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://owq.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ptm.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://voi.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aec.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://zhi.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://sav.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://igc.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://ese.cqqwz.cn

Py:   Counter(arr)
来源：http://nip.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://tmk.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qyz.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxu.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jhv.jianghu66.top

Go:   // 手写 map[T]int
来源：http://gdz.yj20258888.top

Ruby: arr.tally
来源：http://jqz.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dci.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://uzl.0kj1m.cn

Py:   x in arr
来源：http://cgz.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://dml.ybcxt.top

JS:   arr.includes(x)
来源：http://ftm.guannengcc.top

TS:   arr.includes(x)
来源：http://hov.zhongyouzk.top

Java: list.contains(x)
来源：http://zju.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://xdq.zdqjudy.top

Ruby: arr.include?(x)
来源：http://vmi.zdbjq.cn

C#:   list.Contains(x)
来源：http://vrn.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://qpp.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oaa.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zrr.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ott.52xcode.cn

TS:   [...arr];
来源：http://xfo.yj202588.top

Java: new ArrayList<>(list);
来源：http://jlr.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dpl.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://poe.pycfn.com

C#:   new List<int>(list);
来源：http://bxf.0kj1m.cn

[D23] reduce 累积计算
来源：http://hgv.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://smk.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ndr.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvj.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pdl.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qhi.9152youxi.cn

Go:   // 手写循环
来源：http://ril.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fcq.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gxn.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://hol.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://efc.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kal.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hvj.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://swt.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wys.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lwa.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tdc.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xgd.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://kab.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tdp.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvf.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ndy.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rrf.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gdt.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sfn.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sdc.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bhd.nanxuanxn.top

[D26] 数组转字符串
来源：http://leq.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://wuy.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://wen.jqgufenzy.top

JS:   arr.join(", ")
来源：http://sqh.zhixingplan.top

TS:   arr.join(", ")
来源：http://qkp.zhengqikj.top

Java: String.join(", ", list)
来源：http://rlk.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://rua.svipenyu.cn

Ruby: arr.join(", ")
来源：http://ffi.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://fnb.xylfe.cn

================================================================================
来源：http://jit.zdbjq.cn

E. 字符串处理
来源：http://vrl.tarul.cn

================================================================================
来源：http://jhs.ybcxt.top

[E01] 拼接字符串
来源：http://oxr.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fif.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mdj.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xey.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://amm.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vwf.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qrp.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ood.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tnq.gogol.net.cn


<!-- 参考信息 -->