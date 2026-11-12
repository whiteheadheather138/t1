代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://yyg.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rfo.aibaodan.cn

Java: import java.util.List;
来源：http://mij.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://crz.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://ecm.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://soo.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://bca.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://tee.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://qlh.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://ubj.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://fsf.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wza.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://fga.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://glb.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://njo.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://rrq.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wwg.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zve.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://reg.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ytu.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://yqn.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://yga.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wbi.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://ign.hongshengwenyu.top

[C14] 泛型函数
来源：http://slu.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://quf.hongshengwenyu.top

PHP:  // 无泛型
来源：http://lmx.hfpthk.cn

JS:   // 无泛型
来源：http://snq.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tme.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zbp.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dbe.uphjek.com

Ruby: # 无泛型
来源：http://lvr.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kjk.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://oil.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yva.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://skg.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qef.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ndu.havefunace.top

Java: // 无解构
来源：http://vdj.zdbjq.cn

Go:   // 无解构
来源：http://hwv.shuidangran.top

Ruby: a, b = pair
来源：http://ycx.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://xec.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://usp.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qlt.iojbl.cn

PHP:  // 无重载
来源：http://jvf.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://msy.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://irq.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://exb.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://tce.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://xrl.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://onf.yangfankeji.com

================================================================================
来源：http://ejw.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://npd.quarkkingdee.top

================================================================================
来源：http://blu.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://uke.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hzi.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nmt.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dkq.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wkp.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ubn.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://muw.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://rvb.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vte.fehbvm.com

[D02] 追加元素到末尾
来源：http://mvp.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wdb.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oss.zhiwuduotai.top

JS:   arr.push(4);
来源：http://cke.shuidangran.top

TS:   arr.push(4);
来源：http://jrz.yvedp.cn

Java: list.add(4);
来源：http://xhr.havefunace.top

Go:   arr = append(arr, 4)
来源：http://qfw.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://bpp.ydzc1.top

C#:   list.Add(4);
来源：http://tne.fzhhl.top

[D03] 在指定位置插入元素
来源：http://tgb.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://llr.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://unr.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ynz.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://xrb.xylfe.cn

Java: list.add(0, 0);
来源：http://rzo.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mdo.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zfg.cheryme.top

C#:   list.Insert(0, 0);
来源：http://ivb.cqqwz.cn

[D04] 删除元素
来源：http://qsv.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oga.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tvy.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xdw.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://vxx.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mkv.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zlm.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mwi.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wfx.chenzaomai.com

[D05] 访问与修改元素
来源：http://els.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vjj.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fgn.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xci.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://pjn.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://epp.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://cdz.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qzh.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sgk.52xcode.cn

[D06] 数组长度
来源：http://jvb.xylfe.cn

Py:   len(arr)
来源：http://gmq.sjlbkw.cn

PHP:  count($arr);
来源：http://wfj.zdbjq.cn

JS:   arr.length
来源：http://jeu.tanke756.top

TS:   arr.length
来源：http://bdy.ywan-chungtsiang.top

Java: list.size();
来源：http://qww.jinqigfzy.top

Go:   len(arr)
来源：http://sgh.ydzc1.top

Ruby: arr.length; arr.size
来源：http://mnx.jqgfzy.top

C#:   list.Count;
来源：http://pzc.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://mpm.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jhn.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://egm.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://nrw.uphjek.com

TS:   arr.slice(1, 4);
来源：http://hlg.cashguo.top

Java: list.subList(1, 4);
来源：http://bis.pengpengdd.cyou

Go:   arr[1:4]
来源：http://gmc.nanxinkj.top

Ruby: arr[1, 3]
来源：http://yld.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://jgq.yongpay.top

[D08] 合并两个数组
来源：http://iyn.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://chk.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://rey.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ozh.meibo888.top

TS:   [...a, ...b];
来源：http://nqi.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uiz.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://edg.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://uyv.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://bye.cqqwz.cn

[D09] 排序（升序）
来源：http://jqt.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://yaz.ivvv.top

PHP:  sort($arr);
来源：http://xhe.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rps.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mhk.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mxa.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dzf.ivvv.top

Ruby: arr.sort
来源：http://qbh.hcnkem.com

C#:   list.Sort();
来源：http://tug.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://kzm.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fnq.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvi.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mmz.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://brf.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uyb.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ris.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://doa.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kwy.vqdsnc.cn

[D11] 反转数组
来源：http://zrb.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://iwk.sweek.top

PHP:  array_reverse($arr);
来源：http://vce.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://duk.tian-w.cn

TS:   [...arr].reverse();
来源：http://rpx.yuanzhike.top

Java: Collections.reverse(list);
来源：http://nxl.pycfn.com

Go:   slices.Reverse(arr)
来源：http://rxu.shuidangran.top

Ruby: arr.reverse
来源：http://ewy.hammf.cn

C#:   list.Reverse();
来源：http://nse.cashguo.top

[D12] 查找元素下标
来源：http://hvp.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://fmp.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lsj.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nes.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pli.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://btz.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://elr.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://buk.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://rom.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://xbf.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ajt.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://frw.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://hxg.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://kyd.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oeh.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://spg.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bef.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zft.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://kxl.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kie.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybw.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://lfw.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://mbr.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sxh.cucudq.cn

Go:   // 手写循环
来源：http://dqe.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lqv.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mzi.hfpthk.cn

[D15] 去重
来源：http://vay.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ckb.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://dpr.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://sdr.redwolf501.top

TS:   [...new Set(arr)]
来源：http://cmq.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vcj.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://cfh.andypj.xyz

Ruby: arr.uniq
来源：http://txn.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://bga.nanxinkj.top

[D16] 求和与平均值
来源：http://lnc.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zev.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zmg.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iam.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aor.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://plg.tarul.cn

Go:   // 手写循环累加
来源：http://svj.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dff.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://ipr.xylfe.cn

[D17] 最大值与最小值
来源：http://ohk.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://jeq.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://sxc.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rhn.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://sxi.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wxr.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rqs.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://ako.yongpay.top

C#:   list.Max();  list.Min()
来源：http://gyb.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://fqu.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayf.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://kdl.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rug.jinghuilouyu.cn

TS:   nested.flat();
来源：http://lcq.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jup.jqgfzy.top

Go:   // 手写双层循环
来源：http://svo.ctjpmb.com

Ruby: nested.flatten
来源：http://qcj.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lnb.shangyingyoupin.top

[D19] 按字段分组
来源：http://kxa.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sib.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zeh.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpf.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hpv.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vpq.yj20258.top

Go:   // 手写 map[string][]T
来源：http://ibp.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yqa.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ytr.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://xcl.xylfe.cn

Py:   Counter(arr)
来源：http://cmm.hnqzz.top

PHP:  array_count_values($arr);
来源：http://ymm.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwi.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxx.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://okh.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://sxf.cdnleiting.top

Ruby: arr.tally
来源：http://krf.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yxx.redwolf501.top

[D21] 判断是否包含某元素
来源：http://hhm.ydjk.org.cn

Py:   x in arr
来源：http://bfu.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://auq.tianlin.xyz

JS:   arr.includes(x)
来源：http://uvl.xinyue.icu

TS:   arr.includes(x)
来源：http://vni.tian-w.cn

Java: list.contains(x)
来源：http://clo.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://gwz.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://czf.guowangkeji.top

C#:   list.Contains(x)
来源：http://epo.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://lsy.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tsf.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hhw.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mji.hnqzz.top

TS:   [...arr];
来源：http://igl.hcnkem.com

Java: new ArrayList<>(list);
来源：http://xid.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://kui.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://lhu.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://srs.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://goa.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gpt.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://krx.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzg.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zjn.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://koi.yuxming.cn

Go:   // 手写循环
来源：http://igs.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://myo.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dxf.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://vit.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sab.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ccf.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zaz.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://afp.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://avi.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wlf.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fkg.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xcw.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://mbc.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cso.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aql.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mzk.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://chh.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gms.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ger.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lis.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cix.xylfe.cn

[D26] 数组转字符串
来源：http://cfe.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://rsn.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://nbc.shuidangran.top

JS:   arr.join(", ")
来源：http://gbq.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://rrz.xinyue.icu

Java: String.join(", ", list)
来源：http://uhz.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://krf.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://qih.ivvv.top

C#:   string.Join(", ", list)
来源：http://nzx.havefunace.top

================================================================================
来源：http://gbe.zhijiandao.cn

E. 字符串处理
来源：http://cfs.chenzaomai.com

================================================================================
来源：http://wup.yanxiufei.cn

[E01] 拼接字符串
来源：http://kjh.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mcm.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xvz.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iei.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvh.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gyr.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ovl.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oxn.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ors.xuanzx.com


<!-- 参考信息 -->