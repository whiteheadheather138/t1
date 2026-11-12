代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://cyt.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nja.yj20258.top

Java: import java.util.List;
来源：http://tfm.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sdm.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://qqb.0kj1m.cn

C#:   using System.Text;
来源：http://ejp.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://zmp.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://wpp.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://aig.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://zdx.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://nxv.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gzg.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://zit.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://dhl.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kxk.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://oil.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqp.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://haa.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yzn.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tso.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://lwt.uphjek.com

Go:   func add(a, b int) int
来源：http://pmp.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bjk.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lji.gotoacloud.top

[C14] 泛型函数
来源：http://fkr.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uft.yangfankeji.com

PHP:  // 无泛型
来源：http://ihz.fengsongda.top

JS:   // 无泛型
来源：http://noe.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebk.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ofz.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gbf.xinyue.icu

Ruby: # 无泛型
来源：http://rfs.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://git.yueranfly.top

[C15] 解构 / 展开参数
来源：http://mao.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cxd.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://sdv.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uva.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://owv.feifeiyinyue.top

Java: // 无解构
来源：http://iqt.uphjek.com

Go:   // 无解构
来源：http://kbi.redwolf501.top

Ruby: a, b = pair
来源：http://wsv.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://wji.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://uop.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eaw.fehbvm.com

PHP:  // 无重载
来源：http://kki.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qud.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://qbq.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fct.sweek.top

Go:   // 无重载：用不同函数名
来源：http://tuo.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://rve.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hpb.zhixingplan.top

================================================================================
来源：http://nis.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://enz.yj20258888.top

================================================================================
来源：http://cqs.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://prk.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rpo.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xzz.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://umv.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://mmp.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nay.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://jpg.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://kpi.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ysh.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://mgg.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfc.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxz.iojbl.cn

JS:   arr.push(4);
来源：http://drc.cheryme.top

TS:   arr.push(4);
来源：http://lls.zdqjudy.top

Java: list.add(4);
来源：http://fcj.ivvv.top

Go:   arr = append(arr, 4)
来源：http://ygd.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://evv.mhx1999.top

C#:   list.Add(4);
来源：http://orz.hnqzz.top

[D03] 在指定位置插入元素
来源：http://exr.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://vmi.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fnb.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qaz.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://ozd.guannengcc.top

Java: list.add(0, 0);
来源：http://omb.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://hut.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hcx.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://xmk.jinyuanbaomall.cn

[D04] 删除元素
来源：http://wcg.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hel.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tnr.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jjy.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://kyw.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fih.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pwj.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fny.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tag.svipenyu.cn

[D05] 访问与修改元素
来源：http://ujq.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://igj.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wkj.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwv.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://vfr.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://luf.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://zbo.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cvs.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://arb.shanyushiyangkeji.top

[D06] 数组长度
来源：http://wik.gzhubu.top

Py:   len(arr)
来源：http://rpn.xziqi.cn

PHP:  count($arr);
来源：http://wou.nanxuanxn.top

JS:   arr.length
来源：http://ulf.yangfankeji.com

TS:   arr.length
来源：http://gfn.9152youxi.cn

Java: list.size();
来源：http://blz.yj202588.top

Go:   len(arr)
来源：http://dqx.fzhhl.top

Ruby: arr.length; arr.size
来源：http://smj.shanyushiyangtech.top

C#:   list.Count;
来源：http://gfb.xylfe.cn

[D07] 切片 / 取子数组
来源：http://rpf.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yit.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://fov.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://paq.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://qze.xuanzx.com

Java: list.subList(1, 4);
来源：http://tlq.quarkkingdee.top

Go:   arr[1:4]
来源：http://csf.yueranfly.top

Ruby: arr[1, 3]
来源：http://gaq.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://hcc.xylfe.cn

[D08] 合并两个数组
来源：http://lzd.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://yly.pycfn.com

PHP:  array_merge($a, $b);
来源：http://fxg.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tvr.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://wnj.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qwa.shzxlz.cn

Go:   append(a, b...)
来源：http://ljj.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://ppi.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://nde.bjfxy.top

[D09] 排序（升序）
来源：http://wnz.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://scu.quarkkingdee.top

PHP:  sort($arr);
来源：http://qxh.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uxg.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://isu.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fmk.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfr.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://too.zdbjq.cn

C#:   list.Sort();
来源：http://sdv.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vle.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://amd.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zna.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uph.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bzl.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jyw.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sjb.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wuk.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vyc.tanke756.top

[D11] 反转数组
来源：http://yay.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://rgb.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://fxd.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fed.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://hhs.aibaodan.cn

Java: Collections.reverse(list);
来源：http://lue.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://czs.zhongyouzk.top

Ruby: arr.reverse
来源：http://gcw.shuidangran.top

C#:   list.Reverse();
来源：http://cfv.havefunace.top

[D12] 查找元素下标
来源：http://zhm.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://whn.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ztm.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugj.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esu.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yph.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://zdb.yonumen.top

Ruby: arr.index(x)
来源：http://fxm.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://ilt.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://kgj.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mya.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dqf.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://kea.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://kmu.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://szm.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vpn.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yaw.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ofj.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://cvz.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ewc.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbw.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://gdb.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://znf.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sxv.gotoacloud.top

Go:   // 手写循环
来源：http://tia.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fxo.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pzf.sweek.top

[D15] 去重
来源：http://thw.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bud.yj20258888.top

PHP:  array_unique($arr);
来源：http://wjc.hammf.cn

JS:   [...new Set(arr)]
来源：http://hyn.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://wik.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hmx.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ghr.jinqigufen.top

Ruby: arr.uniq
来源：http://bkp.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://qje.pycfn.com

[D16] 求和与平均值
来源：http://wja.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fpa.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ube.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://paw.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eje.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nuk.snrcjt.cn

Go:   // 手写循环累加
来源：http://tbu.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vtk.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://rpp.nwbrower.top

[D17] 最大值与最小值
来源：http://oik.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://vij.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://vem.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lfi.hammf.cn

TS:   Math.max(...arr);
来源：http://cym.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ckm.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qyi.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://wyg.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://xbs.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://wvo.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://liq.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://ofq.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cbx.cdnleiting.top

TS:   nested.flat();
来源：http://skw.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://amm.yfazqb.com

Go:   // 手写双层循环
来源：http://tgn.zhiwuduotai.top

Ruby: nested.flatten
来源：http://fxb.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohy.guannengcc.top

[D19] 按字段分组
来源：http://qwx.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://csf.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cco.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pto.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://roq.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://byp.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://pcd.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cxz.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jjv.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://lgu.guowangkeji.top

Py:   Counter(arr)
来源：http://ycr.birdmap.top

PHP:  array_count_values($arr);
来源：http://alf.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vea.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lfv.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wwt.meibo888.top

Go:   // 手写 map[T]int
来源：http://qap.pengpengdd.cyou

Ruby: arr.tally
来源：http://ujs.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gyz.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://owf.zhijiandao.cn

Py:   x in arr
来源：http://pxw.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://cya.bjfxy.top

JS:   arr.includes(x)
来源：http://wph.tian-w.cn

TS:   arr.includes(x)
来源：http://lhe.fanxiaobao.xyz

Java: list.contains(x)
来源：http://tmd.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://hsm.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://mhn.yfazqb.com

C#:   list.Contains(x)
来源：http://vir.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://wcs.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vrv.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fzh.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://geq.tanke756.top

TS:   [...arr];
来源：http://mka.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://sct.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://asx.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://phr.meibo888.top

C#:   new List<int>(list);
来源：http://bgc.jqgufenzy.top

[D23] reduce 累积计算
来源：http://xgo.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mqu.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lbr.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xqf.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vep.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lin.ybcxt.top

Go:   // 手写循环
来源：http://ixs.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://osk.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wkb.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://xfi.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ilc.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://maf.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zwz.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jgj.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://skb.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rdc.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zkp.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xfg.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://tfm.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://spd.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdc.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ygl.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lsr.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qpp.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jqi.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gfl.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bqo.xuanzx.com

[D26] 数组转字符串
来源：http://dcq.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://xmd.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://tyh.jiagoushi.top

JS:   arr.join(", ")
来源：http://mks.wangdashe.top

TS:   arr.join(", ")
来源：http://sqf.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://jay.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://spt.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://hui.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://jes.quarkkingdee.top

================================================================================
来源：http://dal.jlsjyb.cn

E. 字符串处理
来源：http://cqh.vehdjk.com

================================================================================
来源：http://hzu.yonumen.top

[E01] 拼接字符串
来源：http://cmn.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aey.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axj.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://toj.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nye.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tcs.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dia.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cds.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qre.quarkkingdee.top


<!-- 参考信息 -->