代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://vgd.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bke.yuanzhike.top

Java: import java.util.List;
来源：http://hxs.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xrb.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://thq.yangfankeji.com

C#:   using System.Text;
来源：http://frw.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://vqa.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://yjr.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://ujf.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://zat.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://twb.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vir.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://xdn.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://zgq.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xza.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://yvi.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npb.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vrv.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dbi.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzn.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://amv.andypj.xyz

Go:   func add(a, b int) int
来源：http://ics.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ryr.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://vrv.jinqigufen.top

[C14] 泛型函数
来源：http://bds.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hku.jqgufenzy.top

PHP:  // 无泛型
来源：http://xic.quarkkingdee.top

JS:   // 无泛型
来源：http://pgh.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iof.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vyv.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tis.andypj.xyz

Ruby: # 无泛型
来源：http://fej.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xee.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://tgd.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://srj.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://wxr.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kaz.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bwl.tian-w.cn

Java: // 无解构
来源：http://nrq.ehwqpu.com

Go:   // 无解构
来源：http://jfp.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://uku.yongpay.top

C#:   var (a, b) = pair;
来源：http://ecv.bjfxy.top

[C16] 函数 / 方法重载
来源：http://vlv.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gof.yuxming.cn

PHP:  // 无重载
来源：http://pgb.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xcx.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://fad.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uio.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://llz.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://saa.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hky.hnxiangtu.top

================================================================================
来源：http://uyn.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://sxk.vehdjk.com

================================================================================
来源：http://lka.fktsv.cn

[D01] 创建数组 / 列表
来源：http://hlc.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kwd.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://azy.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hpa.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vjn.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zez.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://bha.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://ujc.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gyu.fktsv.cn

[D02] 追加元素到末尾
来源：http://dbu.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eoi.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wes.birdmap.top

JS:   arr.push(4);
来源：http://rbe.daria6918.cn

TS:   arr.push(4);
来源：http://kys.zdbjq.cn

Java: list.add(4);
来源：http://squ.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://mlo.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://szx.yongpay.top

C#:   list.Add(4);
来源：http://fci.sysykeji.top

[D03] 在指定位置插入元素
来源：http://nkk.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://tsp.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dji.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jfq.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://dys.daria6918.cn

Java: list.add(0, 0);
来源：http://ejg.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://zju.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qnh.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://tmh.fengsongda.top

[D04] 删除元素
来源：http://yuh.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfb.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rpk.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fyb.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://vgm.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hfu.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fcn.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kzb.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyz.yj20258888.top

[D05] 访问与修改元素
来源：http://jjw.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tdi.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://djn.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duc.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://dia.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://fsi.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://bwv.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nbd.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://okt.snrcjt.cn

[D06] 数组长度
来源：http://xqx.wangdashe.top

Py:   len(arr)
来源：http://mwq.bjfxy.top

PHP:  count($arr);
来源：http://etw.epnwcf.com

JS:   arr.length
来源：http://tlo.mhx1999.top

TS:   arr.length
来源：http://xws.gogol.net.cn

Java: list.size();
来源：http://ddg.xuetiantiany.cn

Go:   len(arr)
来源：http://gou.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://otg.zhiwuduotai.top

C#:   list.Count;
来源：http://syy.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://ohp.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dip.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://npv.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://qqx.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://crp.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://cve.jqgufenzy.top

Go:   arr[1:4]
来源：http://uhk.snrcjt.cn

Ruby: arr[1, 3]
来源：http://syn.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://qtt.smart0.xyz

[D08] 合并两个数组
来源：http://yfz.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://neo.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://ywi.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://gap.vqdsnc.cn

TS:   [...a, ...b];
来源：http://zgh.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ovp.bjfxy.top

Go:   append(a, b...)
来源：http://zjo.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://ncn.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://yjk.cashguo.top

[D09] 排序（升序）
来源：http://vvm.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://lxo.hysaishi.cn

PHP:  sort($arr);
来源：http://dmr.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://chp.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ity.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://chs.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rqq.mhx1999.top

Ruby: arr.sort
来源：http://pgj.meibo888.top

C#:   list.Sort();
来源：http://qhc.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vts.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ufg.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxy.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mms.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://stw.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cee.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cuf.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rgo.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbq.jqgfzy.top

[D11] 反转数组
来源：http://krg.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://bdc.ivvv.top

PHP:  array_reverse($arr);
来源：http://ebh.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ihn.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://lri.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://wan.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://oes.hfpthk.cn

Ruby: arr.reverse
来源：http://ula.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://yhs.zdqjudy.top

[D12] 查找元素下标
来源：http://qkh.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://gef.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqo.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mvg.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jhz.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kwj.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://qhn.meibo888.top

Ruby: arr.index(x)
来源：http://gxc.xylfe.cn

C#:   list.IndexOf(x);
来源：http://vfh.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://lsm.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ygj.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xiw.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://jgl.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://ccs.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sxf.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mfw.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jko.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ilx.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://jrt.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pbl.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zfo.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://gew.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://kad.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yzb.mhx1999.top

Go:   // 手写循环
来源：http://jef.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yry.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kil.yanxiufei.cn

[D15] 去重
来源：http://jcd.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dov.zdbjq.cn

PHP:  array_unique($arr);
来源：http://afy.jianghu66.top

JS:   [...new Set(arr)]
来源：http://bmf.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://oba.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://muy.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://ilm.hammf.cn

Ruby: arr.uniq
来源：http://hss.yj20258.top

C#:   list.Distinct().ToList()
来源：http://nxl.yongpay.top

[D16] 求和与平均值
来源：http://tow.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kqy.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bsq.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zie.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xeb.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgz.cdnleiting.top

Go:   // 手写循环累加
来源：http://pcf.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ttg.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://kfl.xinyue.icu

[D17] 最大值与最小值
来源：http://hrt.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://gis.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://fec.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nyn.yuanzhike.top

TS:   Math.max(...arr);
来源：http://lum.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cwm.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kmp.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://gku.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://wrt.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://pxt.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://why.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://mhz.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mgv.jiagoushi.top

TS:   nested.flat();
来源：http://gym.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tzp.redwolf501.top

Go:   // 手写双层循环
来源：http://gke.sysykeji.top

Ruby: nested.flatten
来源：http://cui.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fxf.yj20258888.top

[D19] 按字段分组
来源：http://ugs.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://thu.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fis.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mpe.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ijm.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cpj.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://nkh.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://vin.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ndg.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://sqv.wangshuangyany.cn

Py:   Counter(arr)
来源：http://dip.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://hwn.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kod.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjz.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xyo.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://jnx.iojbl.cn

Ruby: arr.tally
来源：http://xlf.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://umg.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://rmb.gogol.net.cn

Py:   x in arr
来源：http://axo.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://hqf.tian-w.cn

JS:   arr.includes(x)
来源：http://jyw.gogol.net.cn

TS:   arr.includes(x)
来源：http://kll.jianghu66.top

Java: list.contains(x)
来源：http://soo.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://tbt.yangfankeji.com

Ruby: arr.include?(x)
来源：http://saz.yueranfly.top

C#:   list.Contains(x)
来源：http://orb.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://fel.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://doy.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lcb.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hzu.bbcook.cn

TS:   [...arr];
来源：http://nbz.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://yis.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tjw.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://xpo.shzxlz.cn

C#:   new List<int>(list);
来源：http://pkx.ppjwa.cn

[D23] reduce 累积计算
来源：http://pya.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://anf.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://idc.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eam.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yla.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dwc.yvedp.cn

Go:   // 手写循环
来源：http://dpy.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bol.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lbt.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://odt.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bkb.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obo.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cxd.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eya.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cmf.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jap.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bkv.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://erj.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://tqx.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dya.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wur.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aos.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xln.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uru.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://abi.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bya.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oyj.fzhhl.top

[D26] 数组转字符串
来源：http://yek.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://mif.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://drj.aibaodan.cn

JS:   arr.join(", ")
来源：http://odx.0kj1m.cn

TS:   arr.join(", ")
来源：http://pje.tian-w.cn

Java: String.join(", ", list)
来源：http://zje.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://swn.nwbrower.top

Ruby: arr.join(", ")
来源：http://drs.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://usp.xinyue.icu

================================================================================
来源：http://cxx.zhaomingkeji.xyz

E. 字符串处理
来源：http://lrj.cheryme.top

================================================================================
来源：http://mpw.jyoumei.cn

[E01] 拼接字符串
来源：http://rqn.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://onw.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://njq.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vtr.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iks.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mwu.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tzh.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rvu.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ait.jinqigfzy.top


<!-- 参考信息 -->