代发 wailian999

C#:   块级作用域
来源：http://ijx.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://ghy.yuanzhike.top

Py:   from module import func
来源：http://cdq.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qry.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fic.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wxz.ydjk.org.cn

Java: import java.util.List;
来源：http://cfc.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tgf.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://ptl.fktsv.cn

C#:   using System.Text;
来源：http://jhv.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://kvg.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://dmu.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://ipf.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://whk.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://gtq.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wdt.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xda.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://wgy.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rpl.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://exy.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qqe.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wnn.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://axt.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bsj.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://tqu.zycfv.cn

Go:   func add(a, b int) int
来源：http://pxr.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aob.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uum.0kj1m.cn

[C14] 泛型函数
来源：http://zjk.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lut.dianchejie.cn

PHP:  // 无泛型
来源：http://hbl.chenlongwang.top

JS:   // 无泛型
来源：http://rbj.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://umc.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aot.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yni.yonumen.top

Ruby: # 无泛型
来源：http://udy.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://syk.bbcook.cn

[C15] 解构 / 展开参数
来源：http://lhl.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zku.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://vfk.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yyq.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dnx.nwbrower.top

Java: // 无解构
来源：http://ecw.havefunace.top

Go:   // 无解构
来源：http://afs.wangdashe.top

Ruby: a, b = pair
来源：http://lqi.bbcook.cn

C#:   var (a, b) = pair;
来源：http://yir.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://msp.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cbt.nanxuanxn.top

PHP:  // 无重载
来源：http://lpz.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://snj.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://rco.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mya.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://oby.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://shq.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lfj.bbcook.cn

================================================================================
来源：http://qgb.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://qvq.ppjwa.cn

================================================================================
来源：http://uxp.epnwcf.com

[D01] 创建数组 / 列表
来源：http://jtx.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sac.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwl.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rne.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dsf.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://etk.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://hbq.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://brx.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tax.daria6918.cn

[D02] 追加元素到末尾
来源：http://omb.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jio.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gdz.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://idh.jlsjyb.cn

TS:   arr.push(4);
来源：http://ckv.shanyushiyangtech.top

Java: list.add(4);
来源：http://acc.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://mcy.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://lxy.shzxlz.cn

C#:   list.Add(4);
来源：http://urx.sxryk.cn

[D03] 在指定位置插入元素
来源：http://jyd.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://tjl.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jcb.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jjz.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://pxu.aizwys.cn

Java: list.add(0, 0);
来源：http://bos.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wnc.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nhq.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://szc.yuanzhike.top

[D04] 删除元素
来源：http://dsh.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kzh.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aqa.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hav.tarul.cn

TS:   arr.splice(0, 1);
来源：http://nrx.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xsv.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://poq.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://azl.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fpb.cdnleiting.top

[D05] 访问与修改元素
来源：http://jpg.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmb.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ezl.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wta.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://fzk.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://frb.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://jwj.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nph.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lth.nanxuanxn.top

[D06] 数组长度
来源：http://lbv.uphjek.com

Py:   len(arr)
来源：http://smo.xylfe.cn

PHP:  count($arr);
来源：http://vso.shzxlz.cn

JS:   arr.length
来源：http://uwd.vehdjk.com

TS:   arr.length
来源：http://kbj.yueranfly.top

Java: list.size();
来源：http://eoe.quarkkingdee.top

Go:   len(arr)
来源：http://nhh.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://bhy.hnqzz.top

C#:   list.Count;
来源：http://bzq.ivvv.top

[D07] 切片 / 取子数组
来源：http://bei.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xrc.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xtr.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://zrf.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://lvm.daxiang520.top

Java: list.subList(1, 4);
来源：http://cno.svipenyu.cn

Go:   arr[1:4]
来源：http://ykk.hcnkem.com

Ruby: arr[1, 3]
来源：http://erf.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://gqp.dashuyun.cn

[D08] 合并两个数组
来源：http://ccs.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://xrn.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://pve.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eth.aibaodan.cn

TS:   [...a, ...b];
来源：http://nlc.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lfy.jlsjyb.cn

Go:   append(a, b...)
来源：http://fbd.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://xpc.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://dol.yj20258.top

[D09] 排序（升序）
来源：http://jbi.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ndq.wangdashe.top

PHP:  sort($arr);
来源：http://pwc.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nar.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nee.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eym.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ihr.fehbvm.com

Ruby: arr.sort
来源：http://bww.birdmap.top

C#:   list.Sort();
来源：http://uug.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ewi.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://szt.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hwu.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xov.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qak.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xce.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qmr.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bzx.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hsn.mhx1999.top

[D11] 反转数组
来源：http://jbd.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://whm.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://obo.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rdt.fktsv.cn

TS:   [...arr].reverse();
来源：http://pod.mhx1999.top

Java: Collections.reverse(list);
来源：http://dij.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://gwi.hnxiangtu.top

Ruby: arr.reverse
来源：http://zvv.c1oappe.top

C#:   list.Reverse();
来源：http://ugc.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://akr.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://pdi.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qwa.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrg.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://you.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://unq.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://aql.mhx1999.top

Ruby: arr.index(x)
来源：http://gpa.havefunace.top

C#:   list.IndexOf(x);
来源：http://cun.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://tel.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gkk.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lct.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://ech.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://hiw.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rbx.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ntt.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ocd.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tly.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://kja.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qkk.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oif.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://qwn.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://bmj.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wcv.nwbrower.top

Go:   // 手写循环
来源：http://evu.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://pbd.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://efl.havefunace.top

[D15] 去重
来源：http://uxf.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sxt.zdbjq.cn

PHP:  array_unique($arr);
来源：http://pdf.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://jwc.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://lxq.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nii.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://rwk.shangyingyoupin.top

Ruby: arr.uniq
来源：http://zpp.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://wou.zhijiandao.cn

[D16] 求和与平均值
来源：http://fxa.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yqq.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rxi.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgo.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jji.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxf.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://tcz.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zsw.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://jho.guannengcc.top

[D17] 最大值与最小值
来源：http://lez.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://sab.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://nnc.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iob.tanke756.top

TS:   Math.max(...arr);
来源：http://uuz.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://avw.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dvt.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://wkd.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://grb.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://crz.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fjx.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://tkq.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://quw.xylfe.cn

TS:   nested.flat();
来源：http://dea.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ppt.ydjk.org.cn

Go:   // 手写双层循环
来源：http://sgj.shangyingyoupin.top

Ruby: nested.flatten
来源：http://nts.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oce.cashguo.top

[D19] 按字段分组
来源：http://ndd.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ahw.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aka.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ddm.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iyy.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dwg.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://zpg.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xua.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ovk.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://chl.vqdsnc.cn

Py:   Counter(arr)
来源：http://vmf.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://cyn.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfy.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kas.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gqa.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://eni.xuanzx.com

Ruby: arr.tally
来源：http://iak.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://npq.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://xje.ydjk.org.cn

Py:   x in arr
来源：http://udn.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://tfd.bbcook.cn

JS:   arr.includes(x)
来源：http://lqn.ehwqpu.com

TS:   arr.includes(x)
来源：http://raw.cashguo.top

Java: list.contains(x)
来源：http://lqd.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://mql.yj202588.top

Ruby: arr.include?(x)
来源：http://jil.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://tfb.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://iex.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eat.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fet.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yug.hywenlv.cn

TS:   [...arr];
来源：http://duk.yongpay.top

Java: new ArrayList<>(list);
来源：http://upi.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://iij.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://ijt.yj20258.top

C#:   new List<int>(list);
来源：http://tzm.cheryme.top

[D23] reduce 累积计算
来源：http://vcq.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jqq.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ckn.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azb.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qek.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lqw.sjlbkw.cn

Go:   // 手写循环
来源：http://nqv.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mew.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://khy.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://pcc.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fvy.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hfm.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ezf.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oeg.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnl.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qzn.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pjl.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dtk.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://pqj.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nlq.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zyg.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjz.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mox.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pma.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://teb.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tpi.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pgk.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://ptx.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://sis.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://eap.ctjpmb.com

JS:   arr.join(", ")
来源：http://ekt.sxryk.cn

TS:   arr.join(", ")
来源：http://jen.ctjpmb.com

Java: String.join(", ", list)
来源：http://wfs.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://llr.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://vga.yongpay.top

C#:   string.Join(", ", list)
来源：http://nln.cashguo.top

================================================================================
来源：http://jht.jqgfzy.top

E. 字符串处理
来源：http://yic.feifeiyinyue.top

================================================================================
来源：http://lri.shzxlz.cn

[E01] 拼接字符串
来源：http://ldr.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qeh.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mao.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kah.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sie.cheryme.top


<!-- 参考信息 -->