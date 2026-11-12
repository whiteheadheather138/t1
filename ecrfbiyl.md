代发 wailian999

C#:   块级作用域
来源：http://jrl.hysaishi.cn

[C11] 模块导入与导出
来源：http://ahb.uphjek.com

Py:   from module import func
来源：http://pnm.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pun.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yei.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kjv.zycfv.cn

Java: import java.util.List;
来源：http://kej.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bbp.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://iiy.nanxuanxn.top

C#:   using System.Text;
来源：http://kzw.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://hak.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://ocl.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://wth.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://thu.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://yfu.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cjn.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://ssx.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://bxe.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://axo.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://ewr.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://voc.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzi.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ebw.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://huf.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uwq.haohaochexian.top

Go:   func add(a, b int) int
来源：http://emr.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lwv.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://lso.hesvh.cn

[C14] 泛型函数
来源：http://oue.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtj.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://obj.gaohongyu789.top

JS:   // 无泛型
来源：http://sbi.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://swt.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mah.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hyh.kuanghao11.cn

Ruby: # 无泛型
来源：http://njg.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdz.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://sek.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://peo.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://jit.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ved.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bmy.ywan-chungtsiang.top

Java: // 无解构
来源：http://eha.jinqigufen.top

Go:   // 无解构
来源：http://lzw.dashuyun.cn

Ruby: a, b = pair
来源：http://awp.nwbrower.top

C#:   var (a, b) = pair;
来源：http://rke.tanke756.top

[C16] 函数 / 方法重载
来源：http://nns.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hkr.hammf.cn

PHP:  // 无重载
来源：http://fmf.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://npo.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://gqt.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wyt.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://wff.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://ubj.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://osk.uphjek.com

================================================================================
来源：http://uab.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://ymc.jqgufenzy.top

================================================================================
来源：http://ghx.bjfxy.top

[D01] 创建数组 / 列表
来源：http://jle.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bhy.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vec.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oyr.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vdb.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uup.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://qnu.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://ydr.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hdn.ctjpmb.com

[D02] 追加元素到末尾
来源：http://dmf.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://els.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wrl.bbcook.cn

JS:   arr.push(4);
来源：http://why.ydjk.org.cn

TS:   arr.push(4);
来源：http://muo.hfpthk.cn

Java: list.add(4);
来源：http://nij.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://nin.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://vdn.zdqjudy.top

C#:   list.Add(4);
来源：http://ybc.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://qcj.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://boo.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uqd.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wcg.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://paz.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://oju.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://pnu.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lhq.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://gct.sufxvd.cn

[D04] 删除元素
来源：http://sap.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hjz.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://puo.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://goz.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://tjv.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmy.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://njm.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tyk.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jur.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://awo.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zoi.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lot.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ctm.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://jho.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://ksl.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://ymj.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yxs.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xqf.yfazqb.com

[D06] 数组长度
来源：http://fxh.kuanghao11.cn

Py:   len(arr)
来源：http://sda.jyoumei.cn

PHP:  count($arr);
来源：http://mei.wangdashe.top

JS:   arr.length
来源：http://jku.jinqigufen.top

TS:   arr.length
来源：http://vmt.yj20258888.top

Java: list.size();
来源：http://iog.shzxlz.cn

Go:   len(arr)
来源：http://qzl.aizwys.cn

Ruby: arr.length; arr.size
来源：http://rko.ppjwa.cn

C#:   list.Count;
来源：http://zry.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://sfc.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iju.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://ugw.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://fpg.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://ylh.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://fzo.ydjk.org.cn

Go:   arr[1:4]
来源：http://ieh.tanke756.top

Ruby: arr[1, 3]
来源：http://kmb.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://kqp.yj202588.top

[D08] 合并两个数组
来源：http://xxf.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://cum.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://txl.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://lpg.andypj.xyz

TS:   [...a, ...b];
来源：http://lvc.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qzy.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://wpa.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://tnb.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://xvy.hnqzz.top

[D09] 排序（升序）
来源：http://hzr.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://luw.xylfe.cn

PHP:  sort($arr);
来源：http://ioy.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ucc.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qwz.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmd.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vey.sxryk.cn

Ruby: arr.sort
来源：http://xtc.yfazqb.com

C#:   list.Sort();
来源：http://poa.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tie.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jlz.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rrv.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zcm.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fdg.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hac.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vrp.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwa.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jdc.hysaishi.cn

[D11] 反转数组
来源：http://xkj.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://esq.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://bja.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ybe.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://lmw.gzhubu.top

Java: Collections.reverse(list);
来源：http://hyo.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://jsk.tian-w.cn

Ruby: arr.reverse
来源：http://udh.vqdsnc.cn

C#:   list.Reverse();
来源：http://vsi.jinqigfzy.top

[D12] 查找元素下标
来源：http://kvu.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://sbi.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mtd.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xsx.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnn.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cjy.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://kxc.wangdashe.top

Ruby: arr.index(x)
来源：http://kor.yongpay.top

C#:   list.IndexOf(x);
来源：http://tad.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://xin.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mxp.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xrh.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://gnw.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://tda.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ybl.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zkg.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gme.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yks.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://aks.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ccg.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dac.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://igr.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://ybu.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://yab.316326.xyz

Go:   // 手写循环
来源：http://bjb.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://uly.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zup.sysykeji.top

[D15] 去重
来源：http://hkp.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://run.shzxlz.cn

PHP:  array_unique($arr);
来源：http://yhs.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://eqo.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://qvz.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qpn.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pgx.guowangkeji.top

Ruby: arr.uniq
来源：http://cef.hammf.cn

C#:   list.Distinct().ToList()
来源：http://rxo.haohaochexian.top

[D16] 求和与平均值
来源：http://rcs.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uko.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uvu.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gev.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jid.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jmw.havefunace.top

Go:   // 手写循环累加
来源：http://pqi.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://usg.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://blz.ydzc1.top

[D17] 最大值与最小值
来源：http://lrm.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://qbe.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://wec.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xal.xylfe.cn

TS:   Math.max(...arr);
来源：http://xob.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://umm.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://enz.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://lfk.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://hjj.meibo888.top

[D18] 扁平化嵌套数组
来源：http://jma.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ied.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://knc.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sty.svipenyu.cn

TS:   nested.flat();
来源：http://guh.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sjj.zhongyouzk.top

Go:   // 手写双层循环
来源：http://bfz.havefunace.top

Ruby: nested.flatten
来源：http://dic.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qhd.tianlin.xyz

[D19] 按字段分组
来源：http://jir.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://drt.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wny.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pvo.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rvf.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fwj.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://gyx.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eqr.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yac.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://yuo.zhiwuduotai.top

Py:   Counter(arr)
来源：http://rag.smart0.xyz

PHP:  array_count_values($arr);
来源：http://vwu.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsv.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ufz.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aab.guannengcc.top

Go:   // 手写 map[T]int
来源：http://uxu.yangfankeji.com

Ruby: arr.tally
来源：http://hmc.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://acn.yj20258.top

[D21] 判断是否包含某元素
来源：http://zqj.zhijiandao.cn

Py:   x in arr
来源：http://jke.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://kwu.wangdashe.top

JS:   arr.includes(x)
来源：http://zmb.haohaochexian.top

TS:   arr.includes(x)
来源：http://tnr.cheryme.top

Java: list.contains(x)
来源：http://jjq.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://rlg.guowangkeji.top

Ruby: arr.include?(x)
来源：http://tns.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://pah.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://log.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fxe.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://txy.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rws.zhaomingkeji.xyz

TS:   [...arr];
来源：http://lni.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://nhz.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ujm.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://tuo.hammf.cn

C#:   new List<int>(list);
来源：http://iyy.andypj.xyz

[D23] reduce 累积计算
来源：http://gli.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yve.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dnp.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hmu.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cgf.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://edq.cqqwz.cn

Go:   // 手写循环
来源：http://ufj.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jvw.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cbj.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://qrh.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://azl.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ywf.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xno.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rps.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nva.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogx.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://djs.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://npl.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://vhp.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qvj.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zve.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fst.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hcd.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ysi.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iha.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dax.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gvw.chenlongwang.top

[D26] 数组转字符串
来源：http://git.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://pnu.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://ugz.dianchejie.cn

JS:   arr.join(", ")
来源：http://yjy.birdmap.top

TS:   arr.join(", ")
来源：http://kxz.svipenyu.cn

Java: String.join(", ", list)
来源：http://wea.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://jqb.fktsv.cn

Ruby: arr.join(", ")
来源：http://iwv.yj20258888.top

C#:   string.Join(", ", list)
来源：http://coq.zycfv.cn

================================================================================
来源：http://qns.hnxiangtu.top

E. 字符串处理
来源：http://hdd.quarkkingdee.top

================================================================================
来源：http://rkt.ppjwa.cn

[E01] 拼接字符串
来源：http://qto.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ing.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wuo.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dpb.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ond.zdqjudy.top


<!-- 参考信息 -->