代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tjs.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oyb.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zny.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://brd.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://agh.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://puu.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hnp.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://iyd.cqqwz.cn

[C14] 泛型函数
来源：http://mhg.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xje.xuetiantiany.cn

PHP:  // 无泛型
来源：http://qyx.cashguo.top

JS:   // 无泛型
来源：http://yts.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wpo.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aln.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iay.yangfankeji.com

Ruby: # 无泛型
来源：http://psf.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iga.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://snb.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pjx.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://dmk.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fen.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ngs.dashuyun.cn

Java: // 无解构
来源：http://xha.feifeiyinyue.top

Go:   // 无解构
来源：http://loc.c1oappe.top

Ruby: a, b = pair
来源：http://reg.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://xen.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://fao.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://juu.wangdashe.top

PHP:  // 无重载
来源：http://rvl.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kub.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://bnx.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://ndv.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://onw.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://mlq.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xsh.shzxlz.cn

================================================================================
来源：http://qvr.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://ngc.fehbvm.com

================================================================================
来源：http://hig.havefunace.top

[D01] 创建数组 / 列表
来源：http://vci.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wqi.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zyr.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gta.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvr.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozx.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://tpa.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://kny.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ket.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://fqf.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dve.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dgc.vqdsnc.cn

JS:   arr.push(4);
来源：http://eqw.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://zbe.ctjpmb.com

Java: list.add(4);
来源：http://ven.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://mmk.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://xks.ydzc1.top

C#:   list.Add(4);
来源：http://jxy.cashguo.top

[D03] 在指定位置插入元素
来源：http://anr.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://gtn.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uqp.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbd.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://cct.sxryk.cn

Java: list.add(0, 0);
来源：http://gyp.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://ass.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kqq.tanke756.top

C#:   list.Insert(0, 0);
来源：http://agk.316326.xyz

[D04] 删除元素
来源：http://lte.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qbb.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yib.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqe.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://zzo.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://brq.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tvp.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fdx.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uyt.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://vov.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qls.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kyr.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aqc.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://nax.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://dge.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://psr.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldr.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://exj.bbcook.cn

[D06] 数组长度
来源：http://muz.tian-w.cn

Py:   len(arr)
来源：http://coz.bjfxy.top

PHP:  count($arr);
来源：http://stm.svipenyu.cn

JS:   arr.length
来源：http://taq.yj202588.top

TS:   arr.length
来源：http://ygt.yuanzhike.top

Java: list.size();
来源：http://otk.xuanzx.com

Go:   len(arr)
来源：http://qad.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://txn.c1oappe.top

C#:   list.Count;
来源：http://ipi.yj20258888.top

[D07] 切片 / 取子数组
来源：http://meo.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dzx.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://jdo.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://pdw.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://hek.hnqzz.top

Java: list.subList(1, 4);
来源：http://vts.hnxiangtu.top

Go:   arr[1:4]
来源：http://nun.yangfankeji.com

Ruby: arr[1, 3]
来源：http://bse.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://rya.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://dlq.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://lsb.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://mqr.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://zkd.ehwqpu.com

TS:   [...a, ...b];
来源：http://vat.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hzt.gotoacloud.top

Go:   append(a, b...)
来源：http://fcs.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://yur.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://nrz.haohaochexian.top

[D09] 排序（升序）
来源：http://xhx.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://tjh.gzhubu.top

PHP:  sort($arr);
来源：http://npq.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifa.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://bvy.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iej.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nhb.chenzaomai.com

Ruby: arr.sort
来源：http://jpr.ctjpmb.com

C#:   list.Sort();
来源：http://iex.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tjg.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dns.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fsn.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndy.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vki.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://osd.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eiv.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnn.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hrz.hysaishi.cn

[D11] 反转数组
来源：http://cpk.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jjr.yueranfly.top

PHP:  array_reverse($arr);
来源：http://nyr.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uub.0kj1m.cn

TS:   [...arr].reverse();
来源：http://sdg.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://eyt.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://gab.yfazqb.com

Ruby: arr.reverse
来源：http://coa.wangshuangyany.cn

C#:   list.Reverse();
来源：http://xve.0kj1m.cn

[D12] 查找元素下标
来源：http://hpb.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://lmy.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tfv.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wvn.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjc.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpv.birdmap.top

Go:   slices.Index(arr, x)
来源：http://mfd.cqqwz.cn

Ruby: arr.index(x)
来源：http://dpw.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://djb.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://mgr.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wvi.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ejw.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://xns.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://oig.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://alo.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njy.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://qno.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ilq.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://gzg.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mfh.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mex.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://obb.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://wrl.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mkx.tanke756.top

Go:   // 手写循环
来源：http://jgp.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hht.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rzz.yj202588.top

[D15] 去重
来源：http://wbn.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hnb.cdnleiting.top

PHP:  array_unique($arr);
来源：http://qkh.havefunace.top

JS:   [...new Set(arr)]
来源：http://xgv.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://cxs.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://krh.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://bfd.chenlongwang.top

Ruby: arr.uniq
来源：http://vgm.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://npt.gaohongyu789.top

[D16] 求和与平均值
来源：http://lod.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fks.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://frr.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bfz.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvx.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xbz.zhijiandao.cn

Go:   // 手写循环累加
来源：http://hpz.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zso.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://qil.sysykeji.top

[D17] 最大值与最小值
来源：http://ngy.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://smf.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://zoy.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xmi.snrcjt.cn

TS:   Math.max(...arr);
来源：http://utu.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://vla.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kkw.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://coe.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://rth.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://asy.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ufj.tanke756.top

PHP:  array_merge(...$nested);
来源：http://ggs.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbk.vqdsnc.cn

TS:   nested.flat();
来源：http://urg.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pij.jinqigufen.top

Go:   // 手写双层循环
来源：http://tye.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://ahq.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wwq.hysaishi.cn

[D19] 按字段分组
来源：http://gfr.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xtx.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aay.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zrg.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yih.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ehw.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://ewv.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oue.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://akn.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://niw.sysykeji.top

Py:   Counter(arr)
来源：http://afi.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://ihq.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dei.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wkn.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rrf.fzhhl.top

Go:   // 手写 map[T]int
来源：http://xdk.sysykeji.top

Ruby: arr.tally
来源：http://csn.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kiy.xziqi.cn

[D21] 判断是否包含某元素
来源：http://ngk.jyoumei.cn

Py:   x in arr
来源：http://sly.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://shm.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://dkt.smart0.xyz

TS:   arr.includes(x)
来源：http://msy.svipenyu.cn

Java: list.contains(x)
来源：http://orx.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://ror.daria6918.cn

Ruby: arr.include?(x)
来源：http://xyg.chenzaomai.com

C#:   list.Contains(x)
来源：http://jyx.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://ycg.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://biu.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lwr.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rih.ydzc1.top

TS:   [...arr];
来源：http://fdw.tanke756.top

Java: new ArrayList<>(list);
来源：http://jyv.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://vll.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://hgy.xylfe.cn

C#:   new List<int>(list);
来源：http://qjb.guowangkeji.top

[D23] reduce 累积计算
来源：http://ztz.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ilx.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ami.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obz.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://urq.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://asx.hcnkem.com

Go:   // 手写循环
来源：http://nty.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://znt.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dty.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://vaw.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zwt.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hbr.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vse.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dqc.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jmb.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kbo.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mam.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lnm.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://fao.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ezg.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pbv.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fml.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://okx.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://enj.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vzn.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fza.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://snq.cdnleiting.top

[D26] 数组转字符串
来源：http://dlf.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://qsk.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://zho.uphjek.com

JS:   arr.join(", ")
来源：http://tlu.fehbvm.com

TS:   arr.join(", ")
来源：http://ubw.jinqigufen.top

Java: String.join(", ", list)
来源：http://egh.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://lgc.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://jgb.iojbl.cn

C#:   string.Join(", ", list)
来源：http://xmf.shuidangran.top

================================================================================
来源：http://njj.smart0.xyz

E. 字符串处理
来源：http://has.fehbvm.com

================================================================================
来源：http://ukc.shangyingyoupin.top

[E01] 拼接字符串
来源：http://ock.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gfa.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qzp.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bir.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bsk.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tvj.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://egs.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xyk.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tre.feifeiyinyue.top

[E02] 重复字符串
来源：http://sbu.sweek.top

Py:   "ab" * 3
来源：http://fvz.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://qzb.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://gqw.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://zeg.tian-w.cn

Java: "ab".repeat(3)
来源：http://nry.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://uzy.shzxlz.cn

Ruby: "ab" * 3
来源：http://hek.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hmy.ybcxt.top

[E03] 截取子串
来源：http://cdl.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nlk.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vta.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gfg.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://jbd.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://wai.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nmh.nanxuanxn.top


<!-- 参考信息 -->