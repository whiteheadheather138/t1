代发 wailian999

[C14] 泛型函数
来源：http://res.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yck.xuanzx.com

PHP:  // 无泛型
来源：http://opk.jinqigufen.top

JS:   // 无泛型
来源：http://rvj.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sph.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ect.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qqz.redwolf501.top

Ruby: # 无泛型
来源：http://lhk.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nbq.yj20258.top

[C15] 解构 / 展开参数
来源：http://tks.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jeo.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://hyx.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ekv.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mfu.zhoulong.xyz

Java: // 无解构
来源：http://ags.daria6918.cn

Go:   // 无解构
来源：http://cvb.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://ofl.zycfv.cn

C#:   var (a, b) = pair;
来源：http://heq.yongpay.top

[C16] 函数 / 方法重载
来源：http://ojc.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://byt.zdqjudy.top

PHP:  // 无重载
来源：http://bit.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bur.tarul.cn

TS:   // 用联合类型或重载签名声明
来源：http://qct.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jyx.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://hpd.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://nev.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iom.iojbl.cn

================================================================================
来源：http://ehf.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://xdx.ivvv.top

================================================================================
来源：http://uzn.xuanzx.com

[D01] 创建数组 / 列表
来源：http://xcv.zhiwuduotai.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ltp.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zzy.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nnu.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://odf.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://urf.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://jwr.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://aem.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jqw.tanke756.top

[D02] 追加元素到末尾
来源：http://bhq.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uiw.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ghe.cucudq.cn

JS:   arr.push(4);
来源：http://mta.iojbl.cn

TS:   arr.push(4);
来源：http://gep.jianghu66.top

Java: list.add(4);
来源：http://qgi.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://bgr.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://ndh.zdbjq.cn

C#:   list.Add(4);
来源：http://suf.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://etd.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://jun.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://abe.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sdp.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://afg.hesvh.cn

Java: list.add(0, 0);
来源：http://yvz.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hli.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yob.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://xxs.smart0.xyz

[D04] 删除元素
来源：http://dfm.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ffz.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://srk.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://phi.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://end.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pmp.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jtu.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aix.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ykn.cqqwz.cn

[D05] 访问与修改元素
来源：http://ndz.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhp.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://two.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://opa.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://jcy.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://pno.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://fbm.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dcn.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bdi.cheryme.top

[D06] 数组长度
来源：http://dhz.kuanghao11.cn

Py:   len(arr)
来源：http://tge.ctjpmb.com

PHP:  count($arr);
来源：http://hyi.meibo888.top

JS:   arr.length
来源：http://scr.hcnkem.com

TS:   arr.length
来源：http://bzv.yueranfly.top

Java: list.size();
来源：http://xig.cheryme.top

Go:   len(arr)
来源：http://iyc.daxiang520.top

Ruby: arr.length; arr.size
来源：http://olq.chenjidiqi.icu

C#:   list.Count;
来源：http://cmw.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://wwg.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yhh.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://vzg.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://jkf.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://ohq.yuanzhike.top

Java: list.subList(1, 4);
来源：http://ugs.hnqzz.top

Go:   arr[1:4]
来源：http://lag.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://suj.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://apw.quarkkingdee.top

[D08] 合并两个数组
来源：http://qwe.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://eiu.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://aah.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pww.birdmap.top

TS:   [...a, ...b];
来源：http://vmu.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dob.sysykeji.top

Go:   append(a, b...)
来源：http://aen.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://jrq.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://hwj.yuxming.cn

[D09] 排序（升序）
来源：http://vfg.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://ymi.vehdjk.com

PHP:  sort($arr);
来源：http://wgf.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cgw.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lta.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fzy.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sky.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://wyq.hammf.cn

C#:   list.Sort();
来源：http://wny.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://utc.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mjj.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgz.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xsv.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://idv.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ybp.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rjv.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vba.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kyr.shzxlz.cn

[D11] 反转数组
来源：http://qmr.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zrl.tarul.cn

PHP:  array_reverse($arr);
来源：http://mcy.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jif.iojbl.cn

TS:   [...arr].reverse();
来源：http://pzn.hammf.cn

Java: Collections.reverse(list);
来源：http://nyr.yonumen.top

Go:   slices.Reverse(arr)
来源：http://qpr.zdbjq.cn

Ruby: arr.reverse
来源：http://lyu.wangdashe.top

C#:   list.Reverse();
来源：http://xsv.aibaodan.cn

[D12] 查找元素下标
来源：http://qpp.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://nix.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ffe.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kbv.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gen.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://scf.tanke756.top

Go:   slices.Index(arr, x)
来源：http://jai.mhx1999.top

Ruby: arr.index(x)
来源：http://prx.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://kzp.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://jeq.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://enm.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yai.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://quj.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://tll.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dfy.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ota.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nyj.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ttz.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://rdk.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ywp.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wwb.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://ccy.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://mxp.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gtv.cqqwz.cn

Go:   // 手写循环
来源：http://oga.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mfq.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jgq.9152youxi.cn

[D15] 去重
来源：http://vjx.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dzy.9152youxi.cn

PHP:  array_unique($arr);
来源：http://gdc.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://ntl.zycfv.cn

TS:   [...new Set(arr)]
来源：http://dvh.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xgn.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tdr.zhijiandao.cn

Ruby: arr.uniq
来源：http://slu.316326.xyz

C#:   list.Distinct().ToList()
来源：http://lyk.gzhubu.top

[D16] 求和与平均值
来源：http://trs.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yyo.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ofk.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bre.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ahj.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tcc.ydjk.org.cn

Go:   // 手写循环累加
来源：http://tak.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vmh.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://cdu.nanxinkj.top

[D17] 最大值与最小值
来源：http://yrh.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://hkp.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://czk.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ihp.daxiang520.top

TS:   Math.max(...arr);
来源：http://fdp.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qeo.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yps.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://ple.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://fjm.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://uvh.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ley.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://qaf.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iif.316326.xyz

TS:   nested.flat();
来源：http://grb.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ewd.nanxinkj.top

Go:   // 手写双层循环
来源：http://dgh.tarul.cn

Ruby: nested.flatten
来源：http://oag.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://spw.316326.xyz

[D19] 按字段分组
来源：http://vph.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wjq.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wza.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://msh.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xic.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hqi.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://dma.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pdm.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://til.sweek.top

[D20] 统计每个元素出现次数
来源：http://tsg.yuxming.cn

Py:   Counter(arr)
来源：http://vmk.xuanzx.com

PHP:  array_count_values($arr);
来源：http://jms.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mtq.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fhh.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fxg.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://szl.hongshengwenyu.top

Ruby: arr.tally
来源：http://jdw.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ijg.iojbl.cn

[D21] 判断是否包含某元素
来源：http://dyu.shzxlz.cn

Py:   x in arr
来源：http://gbz.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://tmt.fzhhl.top

JS:   arr.includes(x)
来源：http://vjb.c1oappe.top

TS:   arr.includes(x)
来源：http://jrl.vqdsnc.cn

Java: list.contains(x)
来源：http://xmi.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://prx.hcnkem.com

Ruby: arr.include?(x)
来源：http://clr.shzxlz.cn

C#:   list.Contains(x)
来源：http://gzq.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://vbe.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iro.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ulb.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ydn.ppjwa.cn

TS:   [...arr];
来源：http://zaq.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://cwq.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xjz.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://ucx.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://wpq.smart0.xyz

[D23] reduce 累积计算
来源：http://sry.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qmo.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gjh.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sqf.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csk.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ltp.redwolf501.top

Go:   // 手写循环
来源：http://wep.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bti.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rus.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://xig.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ygv.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://faz.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jnd.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfe.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vrx.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://amc.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xnw.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jwr.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://feb.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lxt.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wmq.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qye.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gkh.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fdt.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://poj.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://irf.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jpf.sufxvd.cn

[D26] 数组转字符串
来源：http://nkl.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://zrc.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://muq.yonumen.top

JS:   arr.join(", ")
来源：http://pzc.zycfv.cn

TS:   arr.join(", ")
来源：http://hcb.zhengqikj.top

Java: String.join(", ", list)
来源：http://xxq.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://bcg.zdbjq.cn

Ruby: arr.join(", ")
来源：http://sow.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://sxh.jqgfzy.top

================================================================================
来源：http://dhd.jinyuanbaomall.cn

E. 字符串处理
来源：http://mqd.hnxiangtu.top

================================================================================
来源：http://oed.sweek.top

[E01] 拼接字符串
来源：http://fcd.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fzt.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ghq.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojz.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jsn.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://not.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eqr.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://riu.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nql.jqgufenzy.top

[E02] 重复字符串
来源：http://ter.meibo888.top

Py:   "ab" * 3
来源：http://nue.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://uic.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://rit.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://cko.wangdashe.top

Java: "ab".repeat(3)
来源：http://var.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xsz.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://qpn.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gox.chenzaomai.com

[E03] 截取子串
来源：http://bis.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oqp.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gtr.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iiy.ydzc1.top

TS:   s.slice(1, 4)
来源：http://opi.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://xkj.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbv.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vfk.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://qtw.jqgufenzy.top

[E04] 查找子串位置
来源：http://zlh.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://cbe.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://jpy.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://via.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://gcm.chenzaomai.com

Java: s.indexOf("x")
来源：http://rmx.hesvh.cn


<!-- 参考信息 -->