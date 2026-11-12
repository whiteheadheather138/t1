代发 wailian999

[C10] 变量作用域
来源：http://rcm.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nfl.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dzi.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wei.zdbjq.cn

TS:   同 JS
来源：http://mlg.cheryme.top

Java: 方法内为块级作用域
来源：http://aaf.cashguo.top

Go:   花括号块级作用域
来源：http://rvd.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zhh.cashguo.top

C#:   块级作用域
来源：http://gkk.zhengqikj.top

[C11] 模块导入与导出
来源：http://alb.shanyushiyangkeji.top

Py:   from module import func
来源：http://tsw.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vms.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://tav.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jai.daxiang520.top

Java: import java.util.List;
来源：http://iqk.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bgs.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://vvz.mhx1999.top

C#:   using System.Text;
来源：http://crm.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://nmn.yj20258.top

Py:   (lambda: print("run"))()
来源：http://uds.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://oaw.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://boa.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://usx.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eoy.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://bkx.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://csl.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://atq.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://enq.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rrc.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tjb.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctr.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fup.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://wak.tianlin.xyz

Go:   func add(a, b int) int
来源：http://cme.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qvp.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://era.jqgfzy.top

[C14] 泛型函数
来源：http://tnf.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ppt.gaohongyu789.top

PHP:  // 无泛型
来源：http://rtf.vehdjk.com

JS:   // 无泛型
来源：http://ony.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://koz.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qom.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qqg.yuxming.cn

Ruby: # 无泛型
来源：http://ija.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mjk.sysykeji.top

[C15] 解构 / 展开参数
来源：http://nrr.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ngd.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://hsj.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcq.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://paa.aizwys.cn

Java: // 无解构
来源：http://tcw.jyoumei.cn

Go:   // 无解构
来源：http://kdq.sxryk.cn

Ruby: a, b = pair
来源：http://nsi.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://kat.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://lie.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zvu.c1oappe.top

PHP:  // 无重载
来源：http://xdn.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://owb.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://pls.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gsi.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://dgd.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://cjm.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://eku.nwbrower.top

================================================================================
来源：http://qlt.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://qyt.zhijiandao.cn

================================================================================
来源：http://nnk.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://qoz.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://abi.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ffu.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://elt.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://slq.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://erc.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://ywp.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://lsa.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ghj.cashguo.top

[D02] 追加元素到末尾
来源：http://lfq.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://byw.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://euk.zhijiandao.cn

JS:   arr.push(4);
来源：http://eyx.yueranfly.top

TS:   arr.push(4);
来源：http://xlk.yanxiufei.cn

Java: list.add(4);
来源：http://wnc.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://lat.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://jph.sxryk.cn

C#:   list.Add(4);
来源：http://sgq.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://bxh.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://hnh.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pim.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://goh.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://ncd.jinqigufen.top

Java: list.add(0, 0);
来源：http://pev.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jfb.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jiv.yj202588.top

C#:   list.Insert(0, 0);
来源：http://dox.zycfv.cn

[D04] 删除元素
来源：http://khx.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tit.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://smb.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tdb.sweek.top

TS:   arr.splice(0, 1);
来源：http://xmc.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ooi.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mrk.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eyd.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vyg.cheryme.top

[D05] 访问与修改元素
来源：http://guq.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aip.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fcg.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://glg.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://aon.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://sbi.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ylv.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qqq.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bki.tanke756.top

[D06] 数组长度
来源：http://pod.0kj1m.cn

Py:   len(arr)
来源：http://mkb.shangyingyoupin.top

PHP:  count($arr);
来源：http://sll.guowangkeji.top

JS:   arr.length
来源：http://pab.svipenyu.cn

TS:   arr.length
来源：http://cvu.fehbvm.com

Java: list.size();
来源：http://qrc.zhoulong.xyz

Go:   len(arr)
来源：http://mqq.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://kuw.gogol.net.cn

C#:   list.Count;
来源：http://hwx.yonumen.top

[D07] 切片 / 取子数组
来源：http://xws.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tiw.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://sdx.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://ykx.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://utf.yj20258888.top

Java: list.subList(1, 4);
来源：http://hrd.52xcode.cn

Go:   arr[1:4]
来源：http://qje.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://ymf.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://taq.daxiang520.top

[D08] 合并两个数组
来源：http://lkt.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://dsr.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://zob.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xnd.ybcxt.top

TS:   [...a, ...b];
来源：http://kap.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hun.jyoumei.cn

Go:   append(a, b...)
来源：http://qnr.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://pgl.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://utd.fzhhl.top

[D09] 排序（升序）
来源：http://lrs.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://nfn.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://dnp.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://woi.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mqc.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lxi.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gfl.wangdashe.top

Ruby: arr.sort
来源：http://xor.tanke756.top

C#:   list.Sort();
来源：http://zau.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ogq.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sux.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itz.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lsl.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jcr.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mzd.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://djw.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qmh.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jzd.c1oappe.top

[D11] 反转数组
来源：http://ods.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qax.xylfe.cn

PHP:  array_reverse($arr);
来源：http://yek.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ibx.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://vkr.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://lff.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://ywz.jinqigufen.top

Ruby: arr.reverse
来源：http://rdf.jqgfzy.top

C#:   list.Reverse();
来源：http://fuv.jyoumei.cn

[D12] 查找元素下标
来源：http://jib.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://fau.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hbq.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tit.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kku.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ctq.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://zcr.cdnleiting.top

Ruby: arr.index(x)
来源：http://whv.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://wqw.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://zly.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bux.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dns.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://xxy.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://qvo.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcp.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cqn.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tvx.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://aqq.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://aua.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fqg.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oac.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://tho.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://lcs.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pvt.yj20258888.top

Go:   // 手写循环
来源：http://ljr.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://vbn.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ycm.sweek.top

[D15] 去重
来源：http://wqy.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sqv.tianlin.xyz

PHP:  array_unique($arr);
来源：http://bhn.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://rxc.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://eur.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://srm.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pcm.zycfv.cn

Ruby: arr.uniq
来源：http://klp.pycfn.com

C#:   list.Distinct().ToList()
来源：http://dou.yuxming.cn

[D16] 求和与平均值
来源：http://hsh.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wxx.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cuj.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://szd.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjo.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ing.yfazqb.com

Go:   // 手写循环累加
来源：http://yts.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ivg.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://axy.zhoulong.xyz

[D17] 最大值与最小值
来源：http://zoq.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://ruw.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://ghj.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rmc.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://vkc.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jaf.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mrt.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://orx.sweek.top

C#:   list.Max();  list.Min()
来源：http://qdi.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://jhw.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://udg.tanke756.top

PHP:  array_merge(...$nested);
来源：http://rlr.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xhy.0kj1m.cn

TS:   nested.flat();
来源：http://sgt.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vah.daria6918.cn

Go:   // 手写双层循环
来源：http://cet.fktsv.cn

Ruby: nested.flatten
来源：http://fwx.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vrx.dashuyun.cn

[D19] 按字段分组
来源：http://hvj.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uja.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://guo.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oyi.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ivt.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xqq.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://xjg.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gih.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zsf.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://heq.smart0.xyz

Py:   Counter(arr)
来源：http://lft.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://rnn.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://svd.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njl.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hqi.bbcook.cn

Go:   // 手写 map[T]int
来源：http://sps.jinqigufen.top

Ruby: arr.tally
来源：http://oii.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzt.birdmap.top

[D21] 判断是否包含某元素
来源：http://mvh.yangfankeji.com

Py:   x in arr
来源：http://ylt.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://pew.tanke756.top

JS:   arr.includes(x)
来源：http://cca.yj20258888.top

TS:   arr.includes(x)
来源：http://kil.ppjwa.cn

Java: list.contains(x)
来源：http://agj.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://tof.sweek.top

Ruby: arr.include?(x)
来源：http://wdc.xuanzx.com

C#:   list.Contains(x)
来源：http://bjr.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://fvw.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://odr.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ybo.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fpl.gogol.net.cn

TS:   [...arr];
来源：http://ywp.pycfn.com

Java: new ArrayList<>(list);
来源：http://ppw.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://esw.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://uvd.ydjk.org.cn

C#:   new List<int>(list);
来源：http://eck.cdnleiting.top

[D23] reduce 累积计算
来源：http://jwf.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phe.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bcd.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://voo.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ytp.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://hmu.shanyushiyangtech.top

Go:   // 手写循环
来源：http://bmr.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dix.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sdx.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://qjk.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kmz.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yku.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wiw.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfy.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hpj.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xrx.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://shg.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zzi.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://skk.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qvl.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jsc.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gbk.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gmm.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xpm.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mci.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rtt.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hrp.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://bff.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://cxv.yonumen.top

PHP:  implode(", ", $arr);
来源：http://run.nanxinkj.top

JS:   arr.join(", ")
来源：http://bgh.nwbrower.top

TS:   arr.join(", ")
来源：http://cgw.0kj1m.cn

Java: String.join(", ", list)
来源：http://jcg.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://vdm.nwbrower.top

Ruby: arr.join(", ")
来源：http://ktj.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://rdv.kuanghao11.cn


<!-- 参考信息 -->