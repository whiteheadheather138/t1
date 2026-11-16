代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://gis.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://jmm.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ame.hesvh.cn

[D02] 追加元素到末尾
来源：http://ypb.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ecy.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qmn.tianlin.xyz

JS:   arr.push(4);
来源：http://nuj.yangfankeji.com

TS:   arr.push(4);
来源：http://sjm.pengpengdd.cyou

Java: list.add(4);
来源：http://azg.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://wjj.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://ghw.gotoacloud.top

C#:   list.Add(4);
来源：http://uzg.fehbvm.com

[D03] 在指定位置插入元素
来源：http://wsj.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://sfe.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oci.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://azt.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://kws.cashguo.top

Java: list.add(0, 0);
来源：http://cvc.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://vkl.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kpx.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://hed.yueranfly.top

[D04] 删除元素
来源：http://taz.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://peg.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vlw.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ced.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://mja.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ebn.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dxz.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zyd.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://okb.jqgfzy.top

[D05] 访问与修改元素
来源：http://ssa.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://czz.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jto.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jik.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://jqz.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://anx.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://aaf.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nux.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxe.zhixingplan.top

[D06] 数组长度
来源：http://pub.shanyushiyangkeji.top

Py:   len(arr)
来源：http://yhe.nanxinkj.top

PHP:  count($arr);
来源：http://ldg.ybcxt.top

JS:   arr.length
来源：http://hjs.yfazqb.com

TS:   arr.length
来源：http://rcf.shzxlz.cn

Java: list.size();
来源：http://dtc.cashguo.top

Go:   len(arr)
来源：http://wlk.tanke756.top

Ruby: arr.length; arr.size
来源：http://qjc.cheryme.top

C#:   list.Count;
来源：http://ank.meibo888.top

[D07] 切片 / 取子数组
来源：http://qqi.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cbt.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://stq.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://ake.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://dpw.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://rqd.dashuyun.cn

Go:   arr[1:4]
来源：http://xbi.hesvh.cn

Ruby: arr[1, 3]
来源：http://htv.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://tih.ybcxt.top

[D08] 合并两个数组
来源：http://eev.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://kso.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://ahu.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dkx.cqqwz.cn

TS:   [...a, ...b];
来源：http://laf.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jws.yj20258888.top

Go:   append(a, b...)
来源：http://cdx.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://rwp.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://sfu.yj20258888.top

[D09] 排序（升序）
来源：http://mca.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://bwr.yj202588.top

PHP:  sort($arr);
来源：http://rgi.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kfi.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eku.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nlo.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upu.tarul.cn

Ruby: arr.sort
来源：http://ruu.shuidangran.top

C#:   list.Sort();
来源：http://jcz.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yqc.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://flp.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://euo.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltf.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tqg.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xhq.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lva.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bnq.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vdk.aizwys.cn

[D11] 反转数组
来源：http://qak.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://evg.hnqzz.top

PHP:  array_reverse($arr);
来源：http://sif.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zks.zhengqikj.top

TS:   [...arr].reverse();
来源：http://oae.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://zcd.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://emo.zhiwuduotai.top

Ruby: arr.reverse
来源：http://zsb.quarkkingdee.top

C#:   list.Reverse();
来源：http://ava.gaohongyu789.top

[D12] 查找元素下标
来源：http://veu.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://kzm.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jcn.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yed.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okx.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dfq.cashguo.top

Go:   slices.Index(arr, x)
来源：http://zon.iojbl.cn

Ruby: arr.index(x)
来源：http://bjz.hnqzz.top

C#:   list.IndexOf(x);
来源：http://azn.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://dhc.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qcv.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jjm.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://brg.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://zwg.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rij.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://poe.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://yee.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fiq.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://qpf.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hre.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zis.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://sct.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://aht.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lrh.zdbjq.cn

Go:   // 手写循环
来源：http://fjl.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://hox.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gdo.zhijiandao.cn

[D15] 去重
来源：http://pvm.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mjz.sufxvd.cn

PHP:  array_unique($arr);
来源：http://ciq.yj202588.top

JS:   [...new Set(arr)]
来源：http://rhz.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://joe.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xea.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tfj.fengsongda.top

Ruby: arr.uniq
来源：http://vqv.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://pwo.sxryk.cn

[D16] 求和与平均值
来源：http://qfa.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zns.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cpv.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://msa.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ukz.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kya.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://pwa.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eel.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://sux.mhx1999.top

[D17] 最大值与最小值
来源：http://nio.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://qln.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://epz.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iwt.yuanzhike.top

TS:   Math.max(...arr);
来源：http://tcf.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://inv.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://loz.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://nty.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://kto.sweek.top

[D18] 扁平化嵌套数组
来源：http://grv.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sbp.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://bzg.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bjg.yongpay.top

TS:   nested.flat();
来源：http://okp.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ysd.yfazqb.com

Go:   // 手写双层循环
来源：http://mzp.jiagoushi.top

Ruby: nested.flatten
来源：http://sqy.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vwe.shzxlz.cn

[D19] 按字段分组
来源：http://vmh.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jek.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pxl.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pqb.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ogu.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vrs.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://ifa.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xsa.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bqx.yonumen.top

[D20] 统计每个元素出现次数
来源：http://kju.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://ucc.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://mni.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ofi.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oij.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qad.guannengcc.top

Go:   // 手写 map[T]int
来源：http://gvc.tianlin.xyz

Ruby: arr.tally
来源：http://rrl.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nze.havefunace.top

[D21] 判断是否包含某元素
来源：http://gce.jinqigufen.top

Py:   x in arr
来源：http://xwa.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://pwc.zhixingplan.top

JS:   arr.includes(x)
来源：http://yfx.hcnkem.com

TS:   arr.includes(x)
来源：http://dyu.yongpay.top

Java: list.contains(x)
来源：http://ylb.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://wig.uphjek.com

Ruby: arr.include?(x)
来源：http://fmv.mhx1999.top

C#:   list.Contains(x)
来源：http://qmd.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://nmk.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jzk.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cih.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fnp.ybcxt.top

TS:   [...arr];
来源：http://gft.yj20258888.top

Java: new ArrayList<>(list);
来源：http://gwc.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://avc.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://udh.fengsongda.top

C#:   new List<int>(list);
来源：http://amc.haohaochexian.top

[D23] reduce 累积计算
来源：http://dxq.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfi.aibaodan.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aid.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dfm.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szc.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fxg.xylfe.cn

Go:   // 手写循环
来源：http://jlh.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eeg.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://naq.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://hmj.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rkt.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ezx.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jhm.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cyc.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://elx.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ilk.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hsf.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kjx.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://swq.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eko.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zwy.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ylc.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fka.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bnz.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tsx.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fsz.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wje.cheryme.top

[D26] 数组转字符串
来源：http://kfw.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://zlr.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://fhz.wangdashe.top

JS:   arr.join(", ")
来源：http://pxf.yj20258.top

TS:   arr.join(", ")
来源：http://mtx.yuxming.cn

Java: String.join(", ", list)
来源：http://jnf.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://yuu.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://umn.daria6918.cn

C#:   string.Join(", ", list)
来源：http://bcs.bjfxy.top

================================================================================
来源：http://zey.ehwqpu.com

E. 字符串处理
来源：http://lkh.hesvh.cn

================================================================================
来源：http://fhv.hammf.cn

[E01] 拼接字符串
来源：http://zjb.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qyx.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://krk.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jvo.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lly.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jot.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rpb.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iyn.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jgt.hammf.cn

[E02] 重复字符串
来源：http://raz.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://yuu.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://lec.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://quh.yj202588.top

TS:   "ab".repeat(3)
来源：http://nff.aibaodan.cn

Java: "ab".repeat(3)
来源：http://igw.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://jxt.epnwcf.com

Ruby: "ab" * 3
来源：http://ijh.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nog.mhx1999.top

[E03] 截取子串
来源：http://goj.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://frw.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hwk.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://anf.52xcode.cn

TS:   s.slice(1, 4)
来源：http://ntp.mhx1999.top

Java: s.substring(1, 4)
来源：http://xym.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rpl.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://xnl.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://fyz.yonumen.top

[E04] 查找子串位置
来源：http://fxb.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://cbt.meibo888.top

PHP:  strpos($s, "x");
来源：http://zff.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qqp.pycfn.com

TS:   s.indexOf("x")
来源：http://nar.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://pwk.pycfn.com

Go:   strings.Index(s, "x")
来源：http://htz.52xcode.cn

Ruby: s.index("x")
来源：http://wbl.shuidangran.top

C#:   s.IndexOf("x")
来源：http://uxt.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lim.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://khl.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://msl.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffz.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://spr.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwo.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dwd.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lbe.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ucl.wangdashe.top

[E06] 替换子串
来源：http://wjc.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sfv.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://icr.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gny.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://pos.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jgn.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sei.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fvi.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://qlr.xuanzx.com

[E07] 按分隔符拆分
来源：http://qgq.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jov.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tpn.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yrp.52xcode.cn

TS:   s.split(",")
来源：http://foz.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://xck.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xpl.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://ybb.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vrp.hammf.cn

[E08] 数组按分隔符合并
来源：http://kro.zhengqikj.top

Py:   ",".join(items)
来源：http://ytx.hywenlv.cn

PHP:  implode(",", $items);
来源：http://qsp.daxiang520.top

JS:   items.join(",")
来源：http://sli.52xcode.cn

TS:   items.join(",")
来源：http://yia.zycfv.cn

Java: String.join(",", items)
来源：http://eed.yfazqb.com


<!-- 参考信息 -->