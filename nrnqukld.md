代发 wailian999

TS:   同 JS
来源：http://hod.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://pgz.ppjwa.cn

Go:   花括号块级作用域
来源：http://weu.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cim.sysykeji.top

C#:   块级作用域
来源：http://haw.hywenlv.cn

[C11] 模块导入与导出
来源：http://vbi.fengsongda.top

Py:   from module import func
来源：http://fsa.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nfu.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://mxc.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://het.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://cbh.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ckv.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://fpp.9152youxi.cn

C#:   using System.Text;
来源：http://rox.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://hcz.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://upl.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://vri.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://urb.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://wpv.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gbd.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://xem.sweek.top

Ruby: -> { puts "run" }.call
来源：http://dyb.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ccg.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://gos.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hwv.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgr.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lsl.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tva.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nou.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://mlj.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jeo.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://pux.havefunace.top

[C14] 泛型函数
来源：http://kdx.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dxw.0kj1m.cn

PHP:  // 无泛型
来源：http://nkx.hysaishi.cn

JS:   // 无泛型
来源：http://gye.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ckp.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://srd.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mln.ybcxt.top

Ruby: # 无泛型
来源：http://bkl.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uwh.sxryk.cn

[C15] 解构 / 展开参数
来源：http://abk.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ngo.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://esb.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ozz.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyh.uphjek.com

Java: // 无解构
来源：http://oht.jinqigfzy.top

Go:   // 无解构
来源：http://fsj.316326.xyz

Ruby: a, b = pair
来源：http://fmk.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://ahb.hesvh.cn

[C16] 函数 / 方法重载
来源：http://tse.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ijp.hywenlv.cn

PHP:  // 无重载
来源：http://cfl.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xpf.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://eeu.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vae.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://vff.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://bzh.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jnm.jqgfzy.top

================================================================================
来源：http://znp.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://mwi.andypj.xyz

================================================================================
来源：http://dzt.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://ccf.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mws.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oac.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bmm.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://otk.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lem.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://bxz.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://jxf.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rye.cashguo.top

[D02] 追加元素到末尾
来源：http://sfd.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vsc.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqb.fzhhl.top

JS:   arr.push(4);
来源：http://uog.hfpthk.cn

TS:   arr.push(4);
来源：http://nzn.zhixingplan.top

Java: list.add(4);
来源：http://epz.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://dtq.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://fii.ybcxt.top

C#:   list.Add(4);
来源：http://evq.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://rrl.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://hsq.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kub.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kpd.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://dtu.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://qdo.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://miq.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hsf.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://qpe.chenzaomai.com

[D04] 删除元素
来源：http://ozx.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sbl.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hzh.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pxw.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://rnt.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tzd.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qhy.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vot.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uot.smart0.xyz

[D05] 访问与修改元素
来源：http://omt.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://srv.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ptr.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ber.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wic.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://qgk.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://onp.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ppe.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://akj.ivvv.top

[D06] 数组长度
来源：http://scr.yongpay.top

Py:   len(arr)
来源：http://dmf.fengsongda.top

PHP:  count($arr);
来源：http://qke.redwolf501.top

JS:   arr.length
来源：http://fwm.jyoumei.cn

TS:   arr.length
来源：http://amj.ctjpmb.com

Java: list.size();
来源：http://jxp.yongpay.top

Go:   len(arr)
来源：http://nkg.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://onm.yueranfly.top

C#:   list.Count;
来源：http://evz.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://xlk.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sxx.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hzw.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://jlc.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://urm.mhx1999.top

Java: list.subList(1, 4);
来源：http://kmi.nanxinkj.top

Go:   arr[1:4]
来源：http://jfj.hesvh.cn

Ruby: arr[1, 3]
来源：http://gcg.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://lju.jyoumei.cn

[D08] 合并两个数组
来源：http://iar.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://zvn.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://utb.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fii.hfpthk.cn

TS:   [...a, ...b];
来源：http://ehi.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xzj.ctjpmb.com

Go:   append(a, b...)
来源：http://fek.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://ced.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://ggg.andypj.xyz

[D09] 排序（升序）
来源：http://pbg.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://oyn.yuxming.cn

PHP:  sort($arr);
来源：http://rxf.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wdm.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tcq.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rgo.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wbh.guannengcc.top

Ruby: arr.sort
来源：http://nzi.epnwcf.com

C#:   list.Sort();
来源：http://txw.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://toq.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://izc.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://orh.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dhu.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkn.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uao.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ofm.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://stw.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zdd.jiagoushi.top

[D11] 反转数组
来源：http://gnq.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fro.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://jpi.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rfk.uphjek.com

TS:   [...arr].reverse();
来源：http://jry.fehbvm.com

Java: Collections.reverse(list);
来源：http://fvy.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://ibu.yanxiufei.cn

Ruby: arr.reverse
来源：http://rra.yj20258.top

C#:   list.Reverse();
来源：http://bqi.hesvh.cn

[D12] 查找元素下标
来源：http://oca.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://dcc.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://syo.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgi.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgx.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yih.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://fto.jyoumei.cn

Ruby: arr.index(x)
来源：http://vrc.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://dot.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://nyl.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://keo.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kpj.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://cei.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://miu.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fji.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wqg.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://zhe.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hae.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://iae.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kfm.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kck.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://pny.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://vor.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://itp.cashguo.top

Go:   // 手写循环
来源：http://mzm.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nrq.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bht.yj202588.top

[D15] 去重
来源：http://dpr.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://run.dianchejie.cn

PHP:  array_unique($arr);
来源：http://phs.yonumen.top

JS:   [...new Set(arr)]
来源：http://xjv.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://xqm.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tyu.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cwr.cdnleiting.top

Ruby: arr.uniq
来源：http://ipf.pycfn.com

C#:   list.Distinct().ToList()
来源：http://dwc.cashguo.top

[D16] 求和与平均值
来源：http://pos.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fev.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tzv.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://axl.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gog.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wyk.feifeiyinyue.top

Go:   // 手写循环累加
来源：http://qzi.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://etd.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://awq.yvedp.cn

[D17] 最大值与最小值
来源：http://bik.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://vos.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://jfk.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gwn.guowangkeji.top

TS:   Math.max(...arr);
来源：http://asb.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://byv.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fhy.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://dbi.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://ygw.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://kfk.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gzm.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://pns.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://acl.pengpengdd.cyou

TS:   nested.flat();
来源：http://lqg.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nau.cqqwz.cn

Go:   // 手写双层循环
来源：http://qcf.jianghu66.top

Ruby: nested.flatten
来源：http://rbe.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgk.fengsongda.top

[D19] 按字段分组
来源：http://xsg.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hpn.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cxv.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xpk.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://awd.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ixs.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://fyl.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dcg.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wln.yonumen.top

[D20] 统计每个元素出现次数
来源：http://yyc.birdmap.top

Py:   Counter(arr)
来源：http://wot.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://lhc.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://adi.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zjt.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pka.meibo888.top

Go:   // 手写 map[T]int
来源：http://sui.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://iez.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hjw.vehdjk.com

[D21] 判断是否包含某元素
来源：http://bke.sjlbkw.cn

Py:   x in arr
来源：http://uzx.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://pnn.zhongyouzk.top

JS:   arr.includes(x)
来源：http://egq.jyoumei.cn

TS:   arr.includes(x)
来源：http://smu.redwolf501.top

Java: list.contains(x)
来源：http://yel.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://vea.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://eqx.sxryk.cn

C#:   list.Contains(x)
来源：http://ofe.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://gph.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kol.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vza.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwr.tarul.cn

TS:   [...arr];
来源：http://cwa.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://bkg.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gox.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://ykd.nwbrower.top

C#:   new List<int>(list);
来源：http://pvd.tianlin.xyz

[D23] reduce 累积计算
来源：http://efo.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tnr.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ges.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sch.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://orl.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ovl.0kj1m.cn

Go:   // 手写循环
来源：http://koy.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hvm.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lqx.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://vhu.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zfp.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zxx.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gya.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://crm.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vti.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kou.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://knv.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dsd.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://auk.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zrc.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sft.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mae.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://snh.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dau.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nhb.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lwn.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fwd.hammf.cn

[D26] 数组转字符串
来源：http://qvo.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://rew.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://tve.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://tim.ydzc1.top

TS:   arr.join(", ")
来源：http://uno.birdmap.top

Java: String.join(", ", list)
来源：http://yhj.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://ofe.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://lra.meibo888.top

C#:   string.Join(", ", list)
来源：http://prm.cashguo.top

================================================================================
来源：http://rvq.kuanghao11.cn

E. 字符串处理
来源：http://ubs.epnwcf.com

================================================================================
来源：http://sjr.gzhubu.top

[E01] 拼接字符串
来源：http://wdx.zhongyouzk.top


<!-- 参考信息 -->