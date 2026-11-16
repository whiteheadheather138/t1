代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://tew.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://not.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://vbf.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qxt.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://lez.gotoacloud.top

C#:   using System.Text;
来源：http://lzd.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://wpf.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://job.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://eve.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://keu.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://jjl.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ged.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://sxn.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://bfb.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uym.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://qrr.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rjy.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yea.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://amf.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akb.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ufh.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://diu.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dar.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://jpk.epnwcf.com

[C14] 泛型函数
来源：http://ctu.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rhj.sweek.top

PHP:  // 无泛型
来源：http://jtp.ehwqpu.com

JS:   // 无泛型
来源：http://hjl.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bnq.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tyl.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nbu.iojbl.cn

Ruby: # 无泛型
来源：http://erj.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wka.c1oappe.top

[C15] 解构 / 展开参数
来源：http://efd.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pws.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://rcn.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vsj.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ipw.shanyushiyangkeji.top

Java: // 无解构
来源：http://yet.redwolf501.top

Go:   // 无解构
来源：http://wdc.jyoumei.cn

Ruby: a, b = pair
来源：http://ftm.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://nfg.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://lgu.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hly.gzhubu.top

PHP:  // 无重载
来源：http://jqg.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vei.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://mmc.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nbe.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://cuz.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://jmk.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iik.yj20258.top

================================================================================
来源：http://nsc.meibo888.top

D. 数组 / 列表 / 集合
来源：http://wgf.svipenyu.cn

================================================================================
来源：http://cye.sysykeji.top

[D01] 创建数组 / 列表
来源：http://dae.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fag.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vll.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rtr.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rio.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://set.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://ulb.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://gzy.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://igu.tian-w.cn

[D02] 追加元素到末尾
来源：http://egr.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dyi.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vzc.smart0.xyz

JS:   arr.push(4);
来源：http://zey.guowangkeji.top

TS:   arr.push(4);
来源：http://oqb.daria6918.cn

Java: list.add(4);
来源：http://ewy.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://uns.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ahx.chenzaomai.com

C#:   list.Add(4);
来源：http://enc.hammf.cn

[D03] 在指定位置插入元素
来源：http://guv.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://tas.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://twy.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bch.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ono.sweek.top

Java: list.add(0, 0);
来源：http://mcq.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://tfh.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ybo.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://ile.feifeiyinyue.top

[D04] 删除元素
来源：http://maj.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xpl.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xcz.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://out.tanke756.top

TS:   arr.splice(0, 1);
来源：http://ueu.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aci.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mif.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yzl.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sxh.yvedp.cn

[D05] 访问与修改元素
来源：http://bcl.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://snm.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gmp.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rjf.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://vzk.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://iwi.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://pdd.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xed.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bux.tarul.cn

[D06] 数组长度
来源：http://yqb.zhiwuduotai.top

Py:   len(arr)
来源：http://iut.xuanzx.com

PHP:  count($arr);
来源：http://lqi.sysykeji.top

JS:   arr.length
来源：http://xli.zdqjudy.top

TS:   arr.length
来源：http://hpu.yvedp.cn

Java: list.size();
来源：http://muv.jlsjyb.cn

Go:   len(arr)
来源：http://irl.c1oappe.top

Ruby: arr.length; arr.size
来源：http://lvs.xuanzx.com

C#:   list.Count;
来源：http://edg.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://lqi.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sxt.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gkt.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://rba.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://pjj.hcnkem.com

Java: list.subList(1, 4);
来源：http://icv.daria6918.cn

Go:   arr[1:4]
来源：http://spz.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://zhk.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://ric.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://fqq.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://wui.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://hxu.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xfk.ybcxt.top

TS:   [...a, ...b];
来源：http://zqm.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fmy.sweek.top

Go:   append(a, b...)
来源：http://dez.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://sie.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://bnl.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://jph.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://rmw.ybcxt.top

PHP:  sort($arr);
来源：http://xdb.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fyx.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bpc.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mfw.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://afr.ehwqpu.com

Ruby: arr.sort
来源：http://vxw.hcnkem.com

C#:   list.Sort();
来源：http://nmt.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://plb.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dvc.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://swm.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nll.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fdu.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gig.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mqt.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ktv.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mmu.zhixingplan.top

[D11] 反转数组
来源：http://yjw.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://fca.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://vpk.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lux.yonumen.top

TS:   [...arr].reverse();
来源：http://eoo.sweek.top

Java: Collections.reverse(list);
来源：http://qqg.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://pvi.zhengqikj.top

Ruby: arr.reverse
来源：http://vme.jinqigfzy.top

C#:   list.Reverse();
来源：http://wox.ivvv.top

[D12] 查找元素下标
来源：http://bnn.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://sdp.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tml.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cru.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://elj.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdo.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://fux.shzxlz.cn

Ruby: arr.index(x)
来源：http://pla.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://axb.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://ifo.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vqz.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qlh.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://wmk.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://cyf.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dwv.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ysu.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://nrs.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bau.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://wdu.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gmg.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jyp.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://iwk.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://nig.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvp.haohaochexian.top

Go:   // 手写循环
来源：http://eke.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://oex.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qls.316326.xyz

[D15] 去重
来源：http://fcq.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kov.smart0.xyz

PHP:  array_unique($arr);
来源：http://ybn.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://veb.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://sgx.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://akd.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yfh.mhx1999.top

Ruby: arr.uniq
来源：http://zll.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://llp.cashguo.top

[D16] 求和与平均值
来源：http://bxq.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ycl.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mup.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tbn.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ues.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bfk.hnqzz.top

Go:   // 手写循环累加
来源：http://woy.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sct.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://ijg.vehdjk.com

[D17] 最大值与最小值
来源：http://mhs.havefunace.top

Py:   max(arr);  min(arr)
来源：http://roh.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://zkl.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tuo.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://ceb.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ktk.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jdr.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://olv.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://jit.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://dnq.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vpw.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://ver.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tpq.zhongyouzk.top

TS:   nested.flat();
来源：http://zbg.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://etv.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://nme.hnxiangtu.top

Ruby: nested.flatten
来源：http://hwa.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fvr.wangdashe.top

[D19] 按字段分组
来源：http://vue.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zgu.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cpb.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ter.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nox.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://whq.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://cgi.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qqc.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sto.tarul.cn

[D20] 统计每个元素出现次数
来源：http://glw.sufxvd.cn

Py:   Counter(arr)
来源：http://rzc.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://oft.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vdy.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yst.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://llc.guannengcc.top

Go:   // 手写 map[T]int
来源：http://gof.ybcxt.top

Ruby: arr.tally
来源：http://qfa.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://snl.cucudq.cn

[D21] 判断是否包含某元素
来源：http://wax.yj20258.top

Py:   x in arr
来源：http://ued.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://xab.gogol.net.cn

JS:   arr.includes(x)
来源：http://hxq.dashuyun.cn

TS:   arr.includes(x)
来源：http://sbm.yuxming.cn

Java: list.contains(x)
来源：http://btr.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://wjj.tianlin.xyz

Ruby: arr.include?(x)
来源：http://iur.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ago.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://fyi.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kte.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://khp.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://exp.0kj1m.cn

TS:   [...arr];
来源：http://gee.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://paq.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://kmk.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://ugl.chenlongwang.top

C#:   new List<int>(list);
来源：http://sjj.sxryk.cn

[D23] reduce 累积计算
来源：http://dfk.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hlq.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mgv.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zob.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ehj.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cra.wangshuangyany.cn

Go:   // 手写循环
来源：http://sxc.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgu.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pag.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://ksx.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uck.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ynm.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cwl.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cdd.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uah.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hfb.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xwm.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pzc.cashguo.top

[D25] Set 集合去重与交并差
来源：http://zqd.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jms.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udv.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mzc.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tfz.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kqg.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uuf.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zsr.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwh.tanke756.top

[D26] 数组转字符串
来源：http://tkc.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://srr.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://xky.yanxiufei.cn

JS:   arr.join(", ")
来源：http://cmn.dashuyun.cn

TS:   arr.join(", ")
来源：http://hrj.vehdjk.com

Java: String.join(", ", list)
来源：http://zjk.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://rvy.shuidangran.top

Ruby: arr.join(", ")
来源：http://qfw.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://ete.hfpthk.cn

================================================================================
来源：http://wlj.bjfxy.top

E. 字符串处理
来源：http://fft.zdbjq.cn

================================================================================
来源：http://mmj.hysaishi.cn

[E01] 拼接字符串
来源：http://wol.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pxv.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://znm.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ytf.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ctl.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jcu.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pqb.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qgs.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yux.yuanzhike.top


<!-- 参考信息 -->