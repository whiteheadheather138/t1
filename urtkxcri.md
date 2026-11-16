代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://whe.jqgufenzy.top

C#:   using System.Text;
来源：http://bim.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://cho.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://aea.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://uru.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://xyq.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://wkj.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jfj.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://wwj.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://hiz.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eqz.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://mxk.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zzh.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tqk.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nwt.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://unt.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://xmf.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://sua.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://urj.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://xwh.epnwcf.com

[C14] 泛型函数
来源：http://zaw.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecr.c1oappe.top

PHP:  // 无泛型
来源：http://rjy.yonumen.top

JS:   // 无泛型
来源：http://ljk.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zxy.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sat.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://udi.9152youxi.cn

Ruby: # 无泛型
来源：http://ply.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dkv.yfazqb.com

[C15] 解构 / 展开参数
来源：http://wmc.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://axz.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://ftv.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tnu.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kom.haohaochexian.top

Java: // 无解构
来源：http://tco.52xcode.cn

Go:   // 无解构
来源：http://lgj.yvedp.cn

Ruby: a, b = pair
来源：http://slv.vehdjk.com

C#:   var (a, b) = pair;
来源：http://ggz.fktsv.cn

[C16] 函数 / 方法重载
来源：http://ist.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wqq.yj20258888.top

PHP:  // 无重载
来源：http://ywn.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yfc.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://nzk.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ccr.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://bye.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://kva.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pay.fzhhl.top

================================================================================
来源：http://gxd.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://ciq.cqqwz.cn

================================================================================
来源：http://ccd.ydzc1.top

[D01] 创建数组 / 列表
来源：http://fwc.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://luu.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://myj.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vzl.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://utk.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lxi.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://cqo.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://orn.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bob.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://jnh.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tdk.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zul.daxiang520.top

JS:   arr.push(4);
来源：http://xtt.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://mwd.gzhubu.top

Java: list.add(4);
来源：http://xlb.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://agn.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://bwq.dashuyun.cn

C#:   list.Add(4);
来源：http://nht.redwolf501.top

[D03] 在指定位置插入元素
来源：http://zfa.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://ngk.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://llo.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tmq.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://who.yj20258888.top

Java: list.add(0, 0);
来源：http://usx.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://esf.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lnk.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://cdh.guowangkeji.top

[D04] 删除元素
来源：http://nyu.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xdk.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vkp.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pkd.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://bhf.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://flb.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bdy.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lgu.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kni.yj202588.top

[D05] 访问与修改元素
来源：http://kaa.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jjw.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nws.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tcj.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://qsc.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://bxu.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://eek.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uol.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kov.jqgufenzy.top

[D06] 数组长度
来源：http://udo.yvedp.cn

Py:   len(arr)
来源：http://rqn.yuanzhike.top

PHP:  count($arr);
来源：http://wmu.tanke756.top

JS:   arr.length
来源：http://qip.ybcxt.top

TS:   arr.length
来源：http://knw.yangfankeji.com

Java: list.size();
来源：http://gmx.hfpthk.cn

Go:   len(arr)
来源：http://hbt.nwbrower.top

Ruby: arr.length; arr.size
来源：http://urg.jlsjyb.cn

C#:   list.Count;
来源：http://nwa.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://wgf.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kkh.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://tll.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://mkq.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://awp.xylfe.cn

Java: list.subList(1, 4);
来源：http://twu.jinqigufen.top

Go:   arr[1:4]
来源：http://onf.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://fgw.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://pqr.hnxiangtu.top

[D08] 合并两个数组
来源：http://zxe.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://yih.havefunace.top

PHP:  array_merge($a, $b);
来源：http://wrl.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wji.meibo888.top

TS:   [...a, ...b];
来源：http://oyz.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gyy.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://xlj.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://aqm.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://mum.ivvv.top

[D09] 排序（升序）
来源：http://alh.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://qpy.gzhubu.top

PHP:  sort($arr);
来源：http://kyb.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wwa.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gaa.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ddj.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vag.iojbl.cn

Ruby: arr.sort
来源：http://psj.pengpengdd.cyou

C#:   list.Sort();
来源：http://cvv.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hrd.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bvd.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sci.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hzr.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tiz.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hpc.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xyw.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xgx.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yuh.cheryme.top

[D11] 反转数组
来源：http://jqr.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://nre.fzhhl.top

PHP:  array_reverse($arr);
来源：http://vei.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bie.uphjek.com

TS:   [...arr].reverse();
来源：http://vyk.xinyue.icu

Java: Collections.reverse(list);
来源：http://sou.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://wds.pycfn.com

Ruby: arr.reverse
来源：http://uwo.aibaodan.cn

C#:   list.Reverse();
来源：http://yfv.0kj1m.cn

[D12] 查找元素下标
来源：http://svt.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://rbg.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wwu.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kig.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrw.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iiq.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://vpd.chenzaomai.com

Ruby: arr.index(x)
来源：http://sys.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://odx.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://abe.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bff.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xeo.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://igy.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://tpu.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hge.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dql.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://ltx.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tdy.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://eru.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vba.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iph.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://ody.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://voi.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://vhe.jyoumei.cn

Go:   // 手写循环
来源：http://ysw.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://mee.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://wgg.zhongyouzk.top

[D15] 去重
来源：http://kea.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bxo.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://bim.iojbl.cn

JS:   [...new Set(arr)]
来源：http://idp.yj202588.top

TS:   [...new Set(arr)]
来源：http://osw.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lnn.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://xny.meibo888.top

Ruby: arr.uniq
来源：http://pfu.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://nsg.nanxinkj.top

[D16] 求和与平均值
来源：http://bvj.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bkn.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yof.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zgj.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgl.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hfj.52xcode.cn

Go:   // 手写循环累加
来源：http://joa.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hih.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://fjn.vehdjk.com

[D17] 最大值与最小值
来源：http://wpn.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://sez.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://bls.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ydd.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://bzy.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fnq.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eko.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://uid.uphjek.com

C#:   list.Max();  list.Min()
来源：http://ftw.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://utc.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qns.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://nju.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybi.guannengcc.top

TS:   nested.flat();
来源：http://dat.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dbs.shzxlz.cn

Go:   // 手写双层循环
来源：http://seg.jiagoushi.top

Ruby: nested.flatten
来源：http://hul.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rqr.chenlongwang.top

[D19] 按字段分组
来源：http://tqa.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ycr.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iye.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kdk.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mwf.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yyi.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://uii.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpj.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mad.316326.xyz

[D20] 统计每个元素出现次数
来源：http://jhg.sysykeji.top

Py:   Counter(arr)
来源：http://pcu.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://oij.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uah.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jeo.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wji.yongpay.top

Go:   // 手写 map[T]int
来源：http://nec.yj202588.top

Ruby: arr.tally
来源：http://tcj.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yjm.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://fnp.jinqigufen.top

Py:   x in arr
来源：http://ozu.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://qgd.cheryme.top

JS:   arr.includes(x)
来源：http://nmz.c1oappe.top

TS:   arr.includes(x)
来源：http://uob.shuidangran.top

Java: list.contains(x)
来源：http://oso.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://mjg.hnqzz.top

Ruby: arr.include?(x)
来源：http://shu.svipenyu.cn

C#:   list.Contains(x)
来源：http://viz.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://uha.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vtf.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://awj.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wry.daxiang520.top

TS:   [...arr];
来源：http://rug.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://tez.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://huy.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://asc.ehwqpu.com

C#:   new List<int>(list);
来源：http://oyn.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://gmx.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://toi.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rsu.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evm.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ltt.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sri.mhx1999.top

Go:   // 手写循环
来源：http://afi.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qbg.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtl.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://qrh.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uge.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ipb.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dvq.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rwn.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yee.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzo.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://veu.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jfx.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://rri.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dan.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pwn.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://llr.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vmz.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wne.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://phv.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dvs.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://coy.yongpay.top

[D26] 数组转字符串
来源：http://vjw.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://vma.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://wzx.iojbl.cn

JS:   arr.join(", ")
来源：http://lhx.shzxlz.cn

TS:   arr.join(", ")
来源：http://hqk.316326.xyz

Java: String.join(", ", list)
来源：http://cgc.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://rvd.dianchejie.cn

Ruby: arr.join(", ")
来源：http://tgt.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://jkb.bjfxy.top

================================================================================
来源：http://pco.zhongyouzk.top

E. 字符串处理
来源：http://yjz.daxiang520.top

================================================================================
来源：http://efd.gaohongyu789.top

[E01] 拼接字符串
来源：http://jxd.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tkl.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ggg.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rop.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dbw.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ndy.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bou.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hfa.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lqw.jyoumei.cn

[E02] 重复字符串
来源：http://sqs.yanxiufei.cn

Py:   "ab" * 3
来源：http://ozv.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://vnc.yj20258.top

JS:   "ab".repeat(3)
来源：http://hhp.ydjk.org.cn


<!-- 参考信息 -->