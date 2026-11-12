代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://amt.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://myg.chenzaomai.com

Java: import java.util.List;
来源：http://bik.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://weo.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://gya.gaohongyu789.top

C#:   using System.Text;
来源：http://ngi.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://igv.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://xqq.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://urg.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://brn.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://cuc.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pve.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://gwz.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://vdq.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mmy.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://kni.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eoh.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oud.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cud.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hja.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://pyn.xinyue.icu

Go:   func add(a, b int) int
来源：http://tic.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjf.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qdd.zhiwuduotai.top

[C14] 泛型函数
来源：http://tcu.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vfh.hysaishi.cn

PHP:  // 无泛型
来源：http://iqk.cdnleiting.top

JS:   // 无泛型
来源：http://lub.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sul.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://apy.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ojn.hfpthk.cn

Ruby: # 无泛型
来源：http://jvf.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qyr.ybcxt.top

[C15] 解构 / 展开参数
来源：http://mvq.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nmr.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://skl.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://flf.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zly.jqgfzy.top

Java: // 无解构
来源：http://yyo.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://tpn.chenjidiqi.icu

Ruby: a, b = pair
来源：http://qrz.yonumen.top

C#:   var (a, b) = pair;
来源：http://mcm.tanke756.top

[C16] 函数 / 方法重载
来源：http://oej.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ckk.zycfv.cn

PHP:  // 无重载
来源：http://sho.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uhl.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://sdk.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xhj.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://qrn.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://hzj.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://abk.yanxiufei.cn

================================================================================
来源：http://xvm.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://vcv.xziqi.cn

================================================================================
来源：http://xdx.nwbrower.top

[D01] 创建数组 / 列表
来源：http://uuh.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jhb.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rfz.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://frz.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rxd.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xru.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://jrm.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://huu.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nwt.yfazqb.com

[D02] 追加元素到末尾
来源：http://evo.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zot.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ild.zhixingplan.top

JS:   arr.push(4);
来源：http://dem.0kj1m.cn

TS:   arr.push(4);
来源：http://nlv.aizwys.cn

Java: list.add(4);
来源：http://opw.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://fxb.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://uno.yonumen.top

C#:   list.Add(4);
来源：http://ipl.tanke756.top

[D03] 在指定位置插入元素
来源：http://fmf.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://rgf.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gcz.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wjo.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://rfu.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://iix.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://vbk.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwb.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://dpi.zhijiandao.cn

[D04] 删除元素
来源：http://ews.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zbd.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gmp.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aml.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://fgs.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iit.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lll.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vfe.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qmo.yj20258888.top

[D05] 访问与修改元素
来源：http://wkw.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hrh.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nbh.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgk.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://iqo.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://mgz.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://eet.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lah.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ixb.haohaochexian.top

[D06] 数组长度
来源：http://dki.quarkkingdee.top

Py:   len(arr)
来源：http://bel.bjfxy.top

PHP:  count($arr);
来源：http://ado.yonumen.top

JS:   arr.length
来源：http://aqt.daria6918.cn

TS:   arr.length
来源：http://fyn.yanxiufei.cn

Java: list.size();
来源：http://ifr.chenzaomai.com

Go:   len(arr)
来源：http://kba.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://paz.jinqigufen.top

C#:   list.Count;
来源：http://rgx.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://irb.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hdg.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ryv.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://jvy.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://hiz.yonumen.top

Java: list.subList(1, 4);
来源：http://gff.jianghu66.top

Go:   arr[1:4]
来源：http://sqp.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://quj.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://yfv.zhiwuduotai.top

[D08] 合并两个数组
来源：http://fdp.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://rby.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://iyj.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://vix.hammf.cn

TS:   [...a, ...b];
来源：http://uih.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tzk.aibaodan.cn

Go:   append(a, b...)
来源：http://tga.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://eic.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://ocp.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://tyy.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://mmp.bbcook.cn

PHP:  sort($arr);
来源：http://bnh.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bhe.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://brn.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kzh.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ygm.mhx1999.top

Ruby: arr.sort
来源：http://qob.cashguo.top

C#:   list.Sort();
来源：http://ymm.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ldf.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tkw.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eca.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kyp.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlk.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://igq.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sik.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yip.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kuq.vqdsnc.cn

[D11] 反转数组
来源：http://ovj.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dnx.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://gin.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hee.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://rpn.ehwqpu.com

Java: Collections.reverse(list);
来源：http://nhx.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://tzz.jqgfzy.top

Ruby: arr.reverse
来源：http://grs.yfazqb.com

C#:   list.Reverse();
来源：http://ebs.hnxiangtu.top

[D12] 查找元素下标
来源：http://prh.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://bik.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qhb.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wla.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gry.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nzl.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://bpf.yanxiufei.cn

Ruby: arr.index(x)
来源：http://jwu.ybcxt.top

C#:   list.IndexOf(x);
来源：http://xpo.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://xwz.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aya.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://reu.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://dps.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://sar.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rik.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hvg.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://xtq.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ouk.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://vfd.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xhg.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ste.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://yvg.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://avf.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ncg.wangdashe.top

Go:   // 手写循环
来源：http://gzt.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://cfj.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tor.ctjpmb.com

[D15] 去重
来源：http://pmd.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gek.hammf.cn

PHP:  array_unique($arr);
来源：http://tmz.iojbl.cn

JS:   [...new Set(arr)]
来源：http://bpd.aizwys.cn

TS:   [...new Set(arr)]
来源：http://vhf.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxl.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://rnb.tianlin.xyz

Ruby: arr.uniq
来源：http://qnn.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://qba.fktsv.cn

[D16] 求和与平均值
来源：http://ein.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqb.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hyl.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lkp.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzh.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zcg.ppjwa.cn

Go:   // 手写循环累加
来源：http://hcm.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fod.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://poq.hnqzz.top

[D17] 最大值与最小值
来源：http://ymf.cashguo.top

Py:   max(arr);  min(arr)
来源：http://dtr.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://hdd.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fff.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://eza.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mzn.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fkn.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://yxt.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://kxo.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://jwk.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ftr.yonumen.top

PHP:  array_merge(...$nested);
来源：http://atu.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://opn.cheryme.top

TS:   nested.flat();
来源：http://ytx.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pfs.yj202588.top

Go:   // 手写双层循环
来源：http://htv.tanke756.top

Ruby: nested.flatten
来源：http://fnp.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fdf.52xcode.cn

[D19] 按字段分组
来源：http://vru.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://arm.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uus.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypn.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://iwa.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gif.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://ber.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://shn.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nay.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://kjj.vehdjk.com

Py:   Counter(arr)
来源：http://zuj.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://iep.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyr.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mvq.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vps.fehbvm.com

Go:   // 手写 map[T]int
来源：http://juj.smart0.xyz

Ruby: arr.tally
来源：http://wjt.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sue.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://bdq.jinghuilouyu.cn

Py:   x in arr
来源：http://xlk.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://kpc.nanxuanxn.top

JS:   arr.includes(x)
来源：http://uts.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://bom.jqgufenzy.top

Java: list.contains(x)
来源：http://oxd.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://nhk.ydzc1.top

Ruby: arr.include?(x)
来源：http://epc.tanke756.top

C#:   list.Contains(x)
来源：http://ure.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://msk.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lvw.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wqd.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://viw.tian-w.cn

TS:   [...arr];
来源：http://ygk.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://wck.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://cje.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://mwg.chenlongwang.top

C#:   new List<int>(list);
来源：http://ipr.jianghu66.top

[D23] reduce 累积计算
来源：http://uxy.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lal.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oxi.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ram.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hag.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xge.cashguo.top

Go:   // 手写循环
来源：http://eyp.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://odw.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mjr.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://fsp.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://deb.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gxl.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xmh.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dzl.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rrm.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wcm.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ybe.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zth.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://mms.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oir.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ywo.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ljc.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eaf.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://egi.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lbb.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pgp.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://npu.ydzc1.top

[D26] 数组转字符串
来源：http://fzo.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://mrn.cheryme.top

PHP:  implode(", ", $arr);
来源：http://fsx.nanxinkj.top

JS:   arr.join(", ")
来源：http://igc.yj20258.top

TS:   arr.join(", ")
来源：http://pat.yuanzhike.top

Java: String.join(", ", list)
来源：http://vol.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://exq.zhengqikj.top

Ruby: arr.join(", ")
来源：http://zld.ivvv.top

C#:   string.Join(", ", list)
来源：http://jau.cucudq.cn

================================================================================
来源：http://nho.sjlbkw.cn

E. 字符串处理
来源：http://kml.ehwqpu.com

================================================================================
来源：http://dyy.yuanzhike.top

[E01] 拼接字符串
来源：http://vfy.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eqw.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pij.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dqy.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://izr.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://duh.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://olx.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qoa.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ryb.zdbjq.cn


<!-- 参考信息 -->