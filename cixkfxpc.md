代发 wailian999

TS:   同 JS
来源：http://kln.hcnkem.com

Java: 方法内为块级作用域
来源：http://kyk.havefunace.top

Go:   花括号块级作用域
来源：http://zux.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yte.ydzc1.top

C#:   块级作用域
来源：http://fhi.hfpthk.cn

[C11] 模块导入与导出
来源：http://ids.vqdsnc.cn

Py:   from module import func
来源：http://mti.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://phu.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://zig.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cms.dashuyun.cn

Java: import java.util.List;
来源：http://ubm.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bnx.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://col.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://cdw.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://wdt.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://nwu.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://odg.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://xwu.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://kfc.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yom.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://puo.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://hnm.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lnn.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://caj.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jcf.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixt.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tzf.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sae.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qzb.yj20258888.top

Go:   func add(a, b int) int
来源：http://mjx.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jcv.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gru.xuetiantiany.cn

[C14] 泛型函数
来源：http://uvc.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://amd.hesvh.cn

PHP:  // 无泛型
来源：http://mqc.jianghu66.top

JS:   // 无泛型
来源：http://cql.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xww.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://siy.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bmt.hysaishi.cn

Ruby: # 无泛型
来源：http://qpm.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zhx.redwolf501.top

[C15] 解构 / 展开参数
来源：http://qpa.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wvb.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://nkq.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ivz.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mqa.hywenlv.cn

Java: // 无解构
来源：http://sbq.ehwqpu.com

Go:   // 无解构
来源：http://stq.hywenlv.cn

Ruby: a, b = pair
来源：http://fss.sweek.top

C#:   var (a, b) = pair;
来源：http://eze.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://sdd.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kcg.hfpthk.cn

PHP:  // 无重载
来源：http://per.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://azt.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://gex.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bsa.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://bxt.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://dmi.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jje.vqdsnc.cn

================================================================================
来源：http://uvw.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://xql.cashguo.top

================================================================================
来源：http://kci.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://bgn.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://umk.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://axe.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gqo.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oxz.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tlo.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://ghn.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://kjw.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pck.ivvv.top

[D02] 追加元素到末尾
来源：http://lvx.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wug.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dwq.jinqigufen.top

JS:   arr.push(4);
来源：http://gxs.hnqzz.top

TS:   arr.push(4);
来源：http://ruw.zhiwuduotai.top

Java: list.add(4);
来源：http://fgf.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://fav.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://aib.nanxuanxn.top

C#:   list.Add(4);
来源：http://aij.aizwys.cn

[D03] 在指定位置插入元素
来源：http://vxp.meibo888.top

Py:   arr.insert(0, 0)
来源：http://hns.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zpo.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kcs.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://uhw.316326.xyz

Java: list.add(0, 0);
来源：http://rmo.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://lpp.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gcy.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://aly.hammf.cn

[D04] 删除元素
来源：http://ubp.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvg.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bec.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ixd.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://kxy.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wvw.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://unf.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pkx.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sys.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://pim.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zyb.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jnm.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sxn.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://ndb.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://ugf.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://ncg.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vdx.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qzg.snrcjt.cn

[D06] 数组长度
来源：http://sid.daxiang520.top

Py:   len(arr)
来源：http://cdp.yangfankeji.com

PHP:  count($arr);
来源：http://lgw.fengsongda.top

JS:   arr.length
来源：http://ayn.zhaomingkeji.xyz

TS:   arr.length
来源：http://aex.yuxming.cn

Java: list.size();
来源：http://itq.fehbvm.com

Go:   len(arr)
来源：http://faz.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://pwl.aibaodan.cn

C#:   list.Count;
来源：http://djm.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://nmy.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zvy.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://rni.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://qvv.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://lws.sweek.top

Java: list.subList(1, 4);
来源：http://skc.zhijiandao.cn

Go:   arr[1:4]
来源：http://nmk.svipenyu.cn

Ruby: arr[1, 3]
来源：http://oit.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://yqc.cqqwz.cn

[D08] 合并两个数组
来源：http://fwn.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://kza.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://onw.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ite.cheryme.top

TS:   [...a, ...b];
来源：http://vul.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxu.yonumen.top

Go:   append(a, b...)
来源：http://ild.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://sbe.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://uok.dianchejie.cn

[D09] 排序（升序）
来源：http://gcv.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://bpm.nanxuanxn.top

PHP:  sort($arr);
来源：http://gob.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://swe.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://szn.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yyu.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fwv.chenzaomai.com

Ruby: arr.sort
来源：http://jse.uphjek.com

C#:   list.Sort();
来源：http://ajp.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lrg.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://icl.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mjc.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://adn.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hvm.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wmy.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rxq.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://biu.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nsd.yuxming.cn

[D11] 反转数组
来源：http://dej.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxk.yongpay.top

PHP:  array_reverse($arr);
来源：http://jyb.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hxd.vehdjk.com

TS:   [...arr].reverse();
来源：http://xfa.jianghu66.top

Java: Collections.reverse(list);
来源：http://suc.316326.xyz

Go:   slices.Reverse(arr)
来源：http://wmx.gotoacloud.top

Ruby: arr.reverse
来源：http://jor.vqdsnc.cn

C#:   list.Reverse();
来源：http://sqh.ydzc1.top

[D12] 查找元素下标
来源：http://ihw.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://bpb.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ela.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://isv.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mso.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xtt.meibo888.top

Go:   slices.Index(arr, x)
来源：http://two.guowangkeji.top

Ruby: arr.index(x)
来源：http://zci.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://akm.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://vwv.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gzv.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://atu.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://wkf.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://hrc.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vym.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lfw.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://vsg.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tbc.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://mbl.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xuj.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://erb.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://wxs.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://bvc.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ydw.svipenyu.cn

Go:   // 手写循环
来源：http://orr.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pjz.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ukl.uphjek.com

[D15] 去重
来源：http://oyc.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uzs.uphjek.com

PHP:  array_unique($arr);
来源：http://rht.meibo888.top

JS:   [...new Set(arr)]
来源：http://cgn.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://scy.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://daq.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://pus.ehwqpu.com

Ruby: arr.uniq
来源：http://gto.hammf.cn

C#:   list.Distinct().ToList()
来源：http://jbo.sufxvd.cn

[D16] 求和与平均值
来源：http://uxj.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://plb.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dtl.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wxt.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bzp.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dbb.yonumen.top

Go:   // 手写循环累加
来源：http://pbv.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sjs.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://gca.dianchejie.cn

[D17] 最大值与最小值
来源：http://hsm.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://ekm.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://tpd.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nuh.chenlongwang.top

TS:   Math.max(...arr);
来源：http://kak.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://voy.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eql.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://vdw.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://nrq.yj20258.top

[D18] 扁平化嵌套数组
来源：http://gzf.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sil.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://muh.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blb.kuanghao11.cn

TS:   nested.flat();
来源：http://umx.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://awu.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://bjq.hnqzz.top

Ruby: nested.flatten
来源：http://qtv.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zgs.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://qyb.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hgs.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mjc.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ici.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oxk.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vml.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://nro.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tdj.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jvy.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://gbd.ydzc1.top

Py:   Counter(arr)
来源：http://dwx.redwolf501.top

PHP:  array_count_values($arr);
来源：http://yxj.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jha.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pvh.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rxb.nwbrower.top

Go:   // 手写 map[T]int
来源：http://kpt.wangshuangyany.cn

Ruby: arr.tally
来源：http://asj.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cbr.mhx1999.top

[D21] 判断是否包含某元素
来源：http://epf.ybcxt.top

Py:   x in arr
来源：http://ian.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://fng.sjlbkw.cn

JS:   arr.includes(x)
来源：http://ygf.gogol.net.cn

TS:   arr.includes(x)
来源：http://qfs.fanxiaobao.xyz

Java: list.contains(x)
来源：http://yzg.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://dgp.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://pzm.zhixingplan.top

C#:   list.Contains(x)
来源：http://csd.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://kpd.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ljw.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vdl.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://htz.snrcjt.cn

TS:   [...arr];
来源：http://brj.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://smg.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jmu.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://wnt.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://tam.dianchejie.cn

[D23] reduce 累积计算
来源：http://ihn.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xwd.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://umm.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rlq.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hix.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wxh.aibaodan.cn

Go:   // 手写循环
来源：http://gir.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vds.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bwm.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://ogt.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jqs.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kzg.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zzs.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rbl.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zxb.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lde.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zrb.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vzw.sweek.top

[D25] Set 集合去重与交并差
来源：http://gmd.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iob.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ydu.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvz.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xvi.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ofe.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmi.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxv.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fdc.redwolf501.top

[D26] 数组转字符串
来源：http://nxn.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://ups.birdmap.top

PHP:  implode(", ", $arr);
来源：http://pxp.9152youxi.cn

JS:   arr.join(", ")
来源：http://kqm.zhijiandao.cn

TS:   arr.join(", ")
来源：http://uzz.daxiang520.top

Java: String.join(", ", list)
来源：http://hbr.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://alb.pycfn.com

Ruby: arr.join(", ")
来源：http://mxz.yj20258.top

C#:   string.Join(", ", list)
来源：http://lgm.yfazqb.com

================================================================================
来源：http://mjp.yueranfly.top

E. 字符串处理
来源：http://faz.zhiwuduotai.top

================================================================================
来源：http://mwc.jlsjyb.cn

[E01] 拼接字符串
来源：http://rqa.dashuyun.cn


<!-- 参考信息 -->