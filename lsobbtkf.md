代发 wailian999

C#:   块级作用域
来源：http://gzv.chenzaomai.com

[C11] 模块导入与导出
来源：http://ywd.nanxinkj.top

Py:   from module import func
来源：http://wzt.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nbe.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ufe.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hsx.yanxiufei.cn

Java: import java.util.List;
来源：http://zca.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fia.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://rmx.quarkkingdee.top

C#:   using System.Text;
来源：http://wgj.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://rds.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://bhm.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://tbg.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://hzm.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://isr.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qyv.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://sns.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://muw.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tbc.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://zsq.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jca.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gyy.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nmq.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vge.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://gjx.yj202588.top

Go:   func add(a, b int) int
来源：http://cht.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://few.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eyr.jyoumei.cn

[C14] 泛型函数
来源：http://dzo.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://izp.tianlin.xyz

PHP:  // 无泛型
来源：http://deb.jqgufenzy.top

JS:   // 无泛型
来源：http://ofz.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wvj.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hff.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jvd.yueranfly.top

Ruby: # 无泛型
来源：http://ybb.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tfh.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://anb.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czi.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://nsz.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://upv.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzf.bbcook.cn

Java: // 无解构
来源：http://rve.kuanghao11.cn

Go:   // 无解构
来源：http://pgc.jyoumei.cn

Ruby: a, b = pair
来源：http://lbu.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://swt.yfazqb.com

[C16] 函数 / 方法重载
来源：http://eeg.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zfc.shuidangran.top

PHP:  // 无重载
来源：http://uqy.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://amu.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://dmn.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zwr.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://fkz.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://ubx.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gak.yvedp.cn

================================================================================
来源：http://ahy.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://pds.yueranfly.top

================================================================================
来源：http://rkv.c1oappe.top

[D01] 创建数组 / 列表
来源：http://cot.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://azx.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lzq.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ceo.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://axa.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://khz.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://phc.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://yvv.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gmt.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://phf.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lgs.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hhg.wangshuangyany.cn

JS:   arr.push(4);
来源：http://zgz.gotoacloud.top

TS:   arr.push(4);
来源：http://oeh.xziqi.cn

Java: list.add(4);
来源：http://ria.tanke756.top

Go:   arr = append(arr, 4)
来源：http://wtt.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://rqb.tianlin.xyz

C#:   list.Add(4);
来源：http://udn.sxryk.cn

[D03] 在指定位置插入元素
来源：http://pus.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://kjh.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://miq.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hrn.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://odn.nwbrower.top

Java: list.add(0, 0);
来源：http://pci.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jfh.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://znb.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://gfi.snrcjt.cn

[D04] 删除元素
来源：http://wkf.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://utm.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qip.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ptw.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://vzn.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vsj.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tcj.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bqv.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://alw.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://yoc.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbo.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://smn.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hax.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://etd.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://vpp.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://mfn.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lni.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pgr.jqgfzy.top

[D06] 数组长度
来源：http://ldt.jyoumei.cn

Py:   len(arr)
来源：http://uyy.jianghu66.top

PHP:  count($arr);
来源：http://jmt.andypj.xyz

JS:   arr.length
来源：http://bol.yueranfly.top

TS:   arr.length
来源：http://gfk.nanxuanxn.top

Java: list.size();
来源：http://tmu.yueranfly.top

Go:   len(arr)
来源：http://nvg.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://lmk.zdbjq.cn

C#:   list.Count;
来源：http://alu.yj20258888.top

[D07] 切片 / 取子数组
来源：http://gin.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dtj.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://yil.yj20258.top

JS:   arr.slice(1, 4);
来源：http://tgy.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://twx.jianghu66.top

Java: list.subList(1, 4);
来源：http://dqa.ybcxt.top

Go:   arr[1:4]
来源：http://rta.cqqwz.cn

Ruby: arr[1, 3]
来源：http://guz.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://pdh.jinqigfzy.top

[D08] 合并两个数组
来源：http://cva.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://dwp.yj202588.top

PHP:  array_merge($a, $b);
来源：http://rcb.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kyz.aizwys.cn

TS:   [...a, ...b];
来源：http://kse.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://usu.zhongyouzk.top

Go:   append(a, b...)
来源：http://wce.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://jix.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://xqi.tarul.cn

[D09] 排序（升序）
来源：http://ciz.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://qvt.uphjek.com

PHP:  sort($arr);
来源：http://baj.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nzc.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xlm.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nzi.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hku.gzhubu.top

Ruby: arr.sort
来源：http://jvc.sxryk.cn

C#:   list.Sort();
来源：http://nfk.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qro.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pha.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aye.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://egf.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ywk.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egq.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zsv.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://byo.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ues.sxryk.cn

[D11] 反转数组
来源：http://akk.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://umr.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://rwc.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fbu.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://iru.xinyue.icu

Java: Collections.reverse(list);
来源：http://qyh.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://urq.yangfankeji.com

Ruby: arr.reverse
来源：http://xbx.quarkkingdee.top

C#:   list.Reverse();
来源：http://vbl.pengpengdd.cyou

[D12] 查找元素下标
来源：http://ebd.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://npu.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lmv.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tot.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://laj.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jtt.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://bbp.hysaishi.cn

Ruby: arr.index(x)
来源：http://jzw.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://ofr.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://kwm.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lku.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tqd.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://ekx.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://owy.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rcq.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bez.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://ipc.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dtu.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://skx.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dou.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://amu.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://fjy.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://zbn.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://izu.52xcode.cn

Go:   // 手写循环
来源：http://tnk.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://obh.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://khd.cdnleiting.top

[D15] 去重
来源：http://xwd.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aww.hysaishi.cn

PHP:  array_unique($arr);
来源：http://epz.xinyue.icu

JS:   [...new Set(arr)]
来源：http://swr.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://udb.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rur.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://gos.yuanzhike.top

Ruby: arr.uniq
来源：http://fat.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://byz.hysaishi.cn

[D16] 求和与平均值
来源：http://tht.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zed.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iwm.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gga.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvp.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://irc.yuanzhike.top

Go:   // 手写循环累加
来源：http://apg.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cmx.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://hqq.yangfankeji.com

[D17] 最大值与最小值
来源：http://dnz.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://xby.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://acw.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ulu.epnwcf.com

TS:   Math.max(...arr);
来源：http://psz.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dew.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fog.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://pwk.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://hiv.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://yjs.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://enm.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://xuv.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aum.hammf.cn

TS:   nested.flat();
来源：http://ezl.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zpm.sxryk.cn

Go:   // 手写双层循环
来源：http://bgn.fktsv.cn

Ruby: nested.flatten
来源：http://npt.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yhr.hesvh.cn

[D19] 按字段分组
来源：http://ghl.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ukr.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zod.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ydv.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://utz.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cbu.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://avg.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jrq.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hlb.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://kjd.9152youxi.cn

Py:   Counter(arr)
来源：http://udm.daxiang520.top

PHP:  array_count_values($arr);
来源：http://rjc.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lfu.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwb.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fqq.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://rqy.jlsjyb.cn

Ruby: arr.tally
来源：http://mzk.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gyq.havefunace.top

[D21] 判断是否包含某元素
来源：http://oze.fengsongda.top

Py:   x in arr
来源：http://okf.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://msa.zdqjudy.top

JS:   arr.includes(x)
来源：http://lup.havefunace.top

TS:   arr.includes(x)
来源：http://bfj.yj20258888.top

Java: list.contains(x)
来源：http://wil.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://vat.haohaochexian.top

Ruby: arr.include?(x)
来源：http://mhy.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://jcu.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://gtq.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uel.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uzx.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://klu.yanxiufei.cn

TS:   [...arr];
来源：http://gow.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://hoe.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kmw.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://kqy.zhixingplan.top

C#:   new List<int>(list);
来源：http://vzt.cheryme.top

[D23] reduce 累积计算
来源：http://khe.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jnr.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npo.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mnv.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jtx.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxg.sysykeji.top

Go:   // 手写循环
来源：http://uqd.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zlr.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kei.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://icc.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vrp.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sig.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vmx.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rml.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fyk.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hcm.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gat.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oix.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://lps.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zyp.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vpm.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kzm.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xst.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yqz.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uyc.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ubi.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gan.yj202588.top

[D26] 数组转字符串
来源：http://wdz.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://usu.tanke756.top

PHP:  implode(", ", $arr);
来源：http://ftd.ppjwa.cn

JS:   arr.join(", ")
来源：http://ftm.tarul.cn

TS:   arr.join(", ")
来源：http://yuw.zhongyouzk.top

Java: String.join(", ", list)
来源：http://qjg.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://miq.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://iyh.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://ejk.nwbrower.top

================================================================================
来源：http://yvx.kuanghao11.cn

E. 字符串处理
来源：http://hop.aizwys.cn

================================================================================
来源：http://rbx.jlsjyb.cn

[E01] 拼接字符串
来源：http://efq.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bwl.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dbs.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rjk.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://apn.wangdashe.top


<!-- 参考信息 -->