代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://yhy.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sis.shuidangran.top

Java: import java.util.List;
来源：http://drz.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ftz.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://dno.cqqwz.cn

C#:   using System.Text;
来源：http://odh.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://iby.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://gfn.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://rft.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://fah.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://cfk.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tsx.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://xzu.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://jvr.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qkt.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://lcq.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lds.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uht.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pxt.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zzi.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://baz.zhixingplan.top

Go:   func add(a, b int) int
来源：http://ytw.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fip.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://obr.0kj1m.cn

[C14] 泛型函数
来源：http://bcx.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkd.redwolf501.top

PHP:  // 无泛型
来源：http://wwv.hongshengwenyu.top

JS:   // 无泛型
来源：http://bhy.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nyz.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://puf.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pjs.c1oappe.top

Ruby: # 无泛型
来源：http://umw.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ult.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://onn.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acg.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://vzu.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cfl.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iii.iojbl.cn

Java: // 无解构
来源：http://fkl.52xcode.cn

Go:   // 无解构
来源：http://uns.yonumen.top

Ruby: a, b = pair
来源：http://aek.sysykeji.top

C#:   var (a, b) = pair;
来源：http://zwl.havefunace.top

[C16] 函数 / 方法重载
来源：http://alr.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ecr.vqdsnc.cn

PHP:  // 无重载
来源：http://vmf.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://eyb.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://bsx.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zgc.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://atf.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://uuc.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ehs.yuanzhike.top

================================================================================
来源：http://zet.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://ymk.quarkkingdee.top

================================================================================
来源：http://niq.guannengcc.top

[D01] 创建数组 / 列表
来源：http://fbd.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yfo.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wqf.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lvl.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wnn.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://elf.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://iro.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://upb.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ylg.yj20258.top

[D02] 追加元素到末尾
来源：http://zrc.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rma.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xgb.daxiang520.top

JS:   arr.push(4);
来源：http://lok.shuidangran.top

TS:   arr.push(4);
来源：http://wfs.hnqzz.top

Java: list.add(4);
来源：http://tju.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://lxi.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://dgc.yj20258888.top

C#:   list.Add(4);
来源：http://eew.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://txc.hammf.cn

Py:   arr.insert(0, 0)
来源：http://ncv.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rkv.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pvg.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://imd.yuxming.cn

Java: list.add(0, 0);
来源：http://tfm.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://wqo.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ojw.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://nzv.tian-w.cn

[D04] 删除元素
来源：http://kcj.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lcx.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ocv.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qke.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://pln.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nwl.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ysb.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqv.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nem.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://jky.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ieh.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rzf.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fio.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://kwq.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://skm.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://fiy.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fvh.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lrl.zhengqikj.top

[D06] 数组长度
来源：http://rda.xuanzx.com

Py:   len(arr)
来源：http://nxg.yfazqb.com

PHP:  count($arr);
来源：http://ngp.zycfv.cn

JS:   arr.length
来源：http://kpr.nwbrower.top

TS:   arr.length
来源：http://qhq.chenlongwang.top

Java: list.size();
来源：http://cva.cucudq.cn

Go:   len(arr)
来源：http://jdy.vehdjk.com

Ruby: arr.length; arr.size
来源：http://fqy.jinyuanbaomall.cn

C#:   list.Count;
来源：http://rlq.fktsv.cn

[D07] 切片 / 取子数组
来源：http://cuu.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kxn.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://grj.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://mcj.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://pto.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://tgq.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://gug.yj202588.top

Ruby: arr[1, 3]
来源：http://thn.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://imj.zhoulong.xyz

[D08] 合并两个数组
来源：http://emw.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://cno.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://res.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yyt.gzhubu.top

TS:   [...a, ...b];
来源：http://xaf.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pkk.guowangkeji.top

Go:   append(a, b...)
来源：http://zzl.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://tob.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://acf.birdmap.top

[D09] 排序（升序）
来源：http://fea.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://epk.xuanzx.com

PHP:  sort($arr);
来源：http://vgl.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dxr.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pgo.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zte.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pie.hywenlv.cn

Ruby: arr.sort
来源：http://gki.cucudq.cn

C#:   list.Sort();
来源：http://dqm.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mgg.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rop.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lgr.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://msv.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://emw.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ihs.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kva.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nww.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lqy.shuidangran.top

[D11] 反转数组
来源：http://bij.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://ciu.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://nxm.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uhc.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://xzg.52xcode.cn

Java: Collections.reverse(list);
来源：http://zfw.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://pqa.fktsv.cn

Ruby: arr.reverse
来源：http://xbx.shzxlz.cn

C#:   list.Reverse();
来源：http://axx.aizwys.cn

[D12] 查找元素下标
来源：http://cto.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://jiw.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mhj.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blg.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jrg.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tti.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://xpu.yj202588.top

Ruby: arr.index(x)
来源：http://kxp.andypj.xyz

C#:   list.IndexOf(x);
来源：http://ank.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://otk.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hbx.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zxs.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://ohm.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://qcr.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xsp.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wzj.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://hdx.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://owg.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://mhb.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wes.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rmj.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://jrc.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://crs.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ahw.nanxinkj.top

Go:   // 手写循环
来源：http://sph.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://csx.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vgf.birdmap.top

[D15] 去重
来源：http://ydq.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ucm.pycfn.com

PHP:  array_unique($arr);
来源：http://rnc.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://ktl.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://wfv.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jsq.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://wuk.jqgufenzy.top

Ruby: arr.uniq
来源：http://nem.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://vhu.tian-w.cn

[D16] 求和与平均值
来源：http://lrh.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kem.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://syj.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbi.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://izw.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hjk.meibo888.top

Go:   // 手写循环累加
来源：http://lxc.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://asa.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://vrn.tian-w.cn

[D17] 最大值与最小值
来源：http://dst.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://unu.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://inj.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://evz.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://esz.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dnw.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nrr.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://ybt.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://fds.tarul.cn

[D18] 扁平化嵌套数组
来源：http://ibb.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tuj.cashguo.top

PHP:  array_merge(...$nested);
来源：http://vcd.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvh.sjlbkw.cn

TS:   nested.flat();
来源：http://ktp.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nsk.cdnleiting.top

Go:   // 手写双层循环
来源：http://sdt.shangyingyoupin.top

Ruby: nested.flatten
来源：http://kyd.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://knt.ivvv.top

[D19] 按字段分组
来源：http://ubs.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://suu.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zeq.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mvo.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eym.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ash.meibo888.top

Go:   // 手写 map[string][]T
来源：http://kcg.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yhc.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dzw.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://ifo.redwolf501.top

Py:   Counter(arr)
来源：http://hcv.hammf.cn

PHP:  array_count_values($arr);
来源：http://xkx.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghg.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vgm.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gdj.gzhubu.top

Go:   // 手写 map[T]int
来源：http://gza.jiagoushi.top

Ruby: arr.tally
来源：http://xmy.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wqy.ybcxt.top

[D21] 判断是否包含某元素
来源：http://eue.fengsongda.top

Py:   x in arr
来源：http://vop.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://vzc.chenzaomai.com

JS:   arr.includes(x)
来源：http://rzp.svipenyu.cn

TS:   arr.includes(x)
来源：http://khz.nanxinkj.top

Java: list.contains(x)
来源：http://dqa.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://wjc.smart0.xyz

Ruby: arr.include?(x)
来源：http://mdk.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://wvt.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://xtt.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://izi.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dhz.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fue.ivvv.top

TS:   [...arr];
来源：http://tjg.vehdjk.com

Java: new ArrayList<>(list);
来源：http://dja.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://zgh.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://dlw.c1oappe.top

C#:   new List<int>(list);
来源：http://ore.yj20258.top

[D23] reduce 累积计算
来源：http://fqr.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xyg.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dhw.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpo.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ccg.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qfj.hesvh.cn

Go:   // 手写循环
来源：http://iat.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yvb.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xcr.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://ijl.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nvi.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdx.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cws.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rsw.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bvy.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wka.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yry.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nlw.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://zai.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ctp.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zjv.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xbp.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ovt.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lji.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lit.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rox.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tuj.sjlbkw.cn

[D26] 数组转字符串
来源：http://gxn.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://mqk.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://lri.yanxiufei.cn

JS:   arr.join(", ")
来源：http://oyx.ydzc1.top

TS:   arr.join(", ")
来源：http://exo.cdnleiting.top

Java: String.join(", ", list)
来源：http://jzr.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://nkh.aizwys.cn

Ruby: arr.join(", ")
来源：http://wig.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://aat.xingfuxueyuan.xyz

================================================================================
来源：http://jcv.xuanzx.com

E. 字符串处理
来源：http://zbn.yvedp.cn

================================================================================
来源：http://xre.ctjpmb.com

[E01] 拼接字符串
来源：http://wmf.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qoj.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iyn.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpi.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tbo.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nin.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hkq.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bsp.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ojn.jinghuilouyu.cn


<!-- 参考信息 -->