代发 wailian999

TS:   同 JS
来源：http://nnk.nwbrower.top

Java: 方法内为块级作用域
来源：http://qti.yj202588.top

Go:   花括号块级作用域
来源：http://zdj.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pjm.52xcode.cn

C#:   块级作用域
来源：http://mwj.xziqi.cn

[C11] 模块导入与导出
来源：http://vxc.haohaochexian.top

Py:   from module import func
来源：http://nvm.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ysg.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xcn.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mcm.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://dwu.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ibn.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://irx.hnqzz.top

C#:   using System.Text;
来源：http://cdd.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://fnz.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://yay.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://gnh.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://bwh.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://vsj.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hqf.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://jge.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://jit.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ksc.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://lrg.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zyk.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tuu.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bnp.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ood.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kqw.aibaodan.cn

Go:   func add(a, b int) int
来源：http://anb.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://alk.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://nzh.birdmap.top

[C14] 泛型函数
来源：http://vxb.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tui.hnxiangtu.top

PHP:  // 无泛型
来源：http://urf.316326.xyz

JS:   // 无泛型
来源：http://lqu.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://isy.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://klj.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hgp.zhoulong.xyz

Ruby: # 无泛型
来源：http://usu.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gcx.c1oappe.top

[C15] 解构 / 展开参数
来源：http://qyu.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://max.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://crr.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fkv.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qgw.zhaomingkeji.xyz

Java: // 无解构
来源：http://dzd.quarkkingdee.top

Go:   // 无解构
来源：http://atz.zhoulong.xyz

Ruby: a, b = pair
来源：http://kmk.xylfe.cn

C#:   var (a, b) = pair;
来源：http://wzm.smart0.xyz

[C16] 函数 / 方法重载
来源：http://ctb.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sil.xylfe.cn

PHP:  // 无重载
来源：http://ygl.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qlc.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://iaa.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kvu.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://niq.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://jdq.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ilo.uphjek.com

================================================================================
来源：http://bqu.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://foh.gzhubu.top

================================================================================
来源：http://poq.bjfxy.top

[D01] 创建数组 / 列表
来源：http://yna.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uus.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bhy.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ziw.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qyh.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jdx.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://wea.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://qgh.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://twk.havefunace.top

[D02] 追加元素到末尾
来源：http://xhc.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uak.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ovu.nwbrower.top

JS:   arr.push(4);
来源：http://pss.jlsjyb.cn

TS:   arr.push(4);
来源：http://suh.fzhhl.top

Java: list.add(4);
来源：http://hfx.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://lcp.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://dzx.zdbjq.cn

C#:   list.Add(4);
来源：http://hht.ivvv.top

[D03] 在指定位置插入元素
来源：http://siq.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://mly.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pmj.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fep.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://rxx.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://isi.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://kax.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zvd.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://xtq.nanxuanxn.top

[D04] 删除元素
来源：http://gop.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zoy.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uyr.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://thh.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://qaj.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fhb.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://erl.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pkk.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sfn.ydjk.org.cn

[D05] 访问与修改元素
来源：http://svd.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://roc.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yxa.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://noj.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://amk.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://ddr.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://vwo.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xkf.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kkj.shzxlz.cn

[D06] 数组长度
来源：http://jxf.fengsongda.top

Py:   len(arr)
来源：http://ffm.fengsongda.top

PHP:  count($arr);
来源：http://rat.sxryk.cn

JS:   arr.length
来源：http://buu.guowangkeji.top

TS:   arr.length
来源：http://ypt.zhixingplan.top

Java: list.size();
来源：http://tsl.jyoumei.cn

Go:   len(arr)
来源：http://amc.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://wqd.shzxlz.cn

C#:   list.Count;
来源：http://jng.yj202588.top

[D07] 切片 / 取子数组
来源：http://tpn.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xqp.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bqu.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://ihs.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://crz.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://cpy.sxryk.cn

Go:   arr[1:4]
来源：http://mqs.mhx1999.top

Ruby: arr[1, 3]
来源：http://ojq.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://wjq.cheryme.top

[D08] 合并两个数组
来源：http://lso.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://lei.pycfn.com

PHP:  array_merge($a, $b);
来源：http://lba.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jhk.zhijiandao.cn

TS:   [...a, ...b];
来源：http://mpc.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kmo.jqgufenzy.top

Go:   append(a, b...)
来源：http://qvf.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://qld.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://vqf.hnxiangtu.top

[D09] 排序（升序）
来源：http://hli.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://kei.daria6918.cn

PHP:  sort($arr);
来源：http://kks.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wwv.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ckz.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://paz.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bgv.chenjidiqi.icu

Ruby: arr.sort
来源：http://fny.yuxming.cn

C#:   list.Sort();
来源：http://ryz.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iah.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fhw.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwz.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://frr.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://scl.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://msm.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xzm.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kah.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vdh.chenlongwang.top

[D11] 反转数组
来源：http://iwt.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dlc.iojbl.cn

PHP:  array_reverse($arr);
来源：http://eqa.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ocb.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://flo.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://qso.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://tco.zhiwuduotai.top

Ruby: arr.reverse
来源：http://xct.zhongyouzk.top

C#:   list.Reverse();
来源：http://kwr.kuanghao11.cn

[D12] 查找元素下标
来源：http://vmn.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://xhx.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zaq.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hmk.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krz.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iin.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://vob.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://noa.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://fxc.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://mls.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ahi.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rkl.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://lvz.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://cvf.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pxo.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iew.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://jpf.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rip.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://qpz.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ojc.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dbh.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://lsl.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://xlm.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xpc.shzxlz.cn

Go:   // 手写循环
来源：http://xru.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://tou.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cti.cucudq.cn

[D15] 去重
来源：http://uax.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ayr.aibaodan.cn

PHP:  array_unique($arr);
来源：http://qsn.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://ezf.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://abc.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gqo.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hcc.gogol.net.cn

Ruby: arr.uniq
来源：http://iwf.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://rgz.havefunace.top

[D16] 求和与平均值
来源：http://zrh.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zaa.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hkw.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpq.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ccw.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qow.zhengqikj.top

Go:   // 手写循环累加
来源：http://azc.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ygb.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://aob.dianchejie.cn

[D17] 最大值与最小值
来源：http://nbw.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://hyn.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://wzi.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nmd.cdnleiting.top

TS:   Math.max(...arr);
来源：http://xay.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aae.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ngv.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://glf.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://fzd.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://uyy.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://osv.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://wik.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aai.xylfe.cn

TS:   nested.flat();
来源：http://hvx.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bsk.cdnleiting.top

Go:   // 手写双层循环
来源：http://gwb.yvedp.cn

Ruby: nested.flatten
来源：http://iyr.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ukz.ydjk.org.cn

[D19] 按字段分组
来源：http://nco.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://otd.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fxu.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hxp.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ksw.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kap.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://zbv.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://whe.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://odu.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://pyj.shangyingyoupin.top

Py:   Counter(arr)
来源：http://xac.yj202588.top

PHP:  array_count_values($arr);
来源：http://upr.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwr.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxt.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://crr.tanke756.top

Go:   // 手写 map[T]int
来源：http://vqo.hfpthk.cn

Ruby: arr.tally
来源：http://lfa.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sur.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://ybh.shzxlz.cn

Py:   x in arr
来源：http://eue.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://meq.mhx1999.top

JS:   arr.includes(x)
来源：http://zjn.shuidangran.top

TS:   arr.includes(x)
来源：http://upi.xinyue.icu

Java: list.contains(x)
来源：http://kjj.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://acj.nwbrower.top

Ruby: arr.include?(x)
来源：http://gdb.aizwys.cn

C#:   list.Contains(x)
来源：http://mff.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://est.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ucy.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://niy.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gfr.fzhhl.top

TS:   [...arr];
来源：http://goc.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://vak.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://int.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://cob.svipenyu.cn

C#:   new List<int>(list);
来源：http://pqi.zhoulong.xyz

[D23] reduce 累积计算
来源：http://qql.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tjz.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://apg.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rdo.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmm.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfe.jqgfzy.top

Go:   // 手写循环
来源：http://bxm.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eyr.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zsx.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://pwb.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://spi.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rfc.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://scr.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tnc.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xiy.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jub.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jva.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zrg.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://daf.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://egc.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://juw.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvc.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yfw.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ygd.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fxl.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvk.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://beu.bbcook.cn

[D26] 数组转字符串
来源：http://pya.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://zuv.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://paf.hywenlv.cn

JS:   arr.join(", ")
来源：http://xen.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://fvw.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://hfy.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://fbi.hfpthk.cn

Ruby: arr.join(", ")
来源：http://ptv.shuidangran.top

C#:   string.Join(", ", list)
来源：http://ook.shanyushiyangkeji.top

================================================================================
来源：http://pkd.gotoacloud.top

E. 字符串处理
来源：http://kto.smart0.xyz

================================================================================
来源：http://ecm.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://jlw.wangshuangyany.cn


<!-- 参考信息 -->