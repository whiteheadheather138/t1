代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qhi.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wlj.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxs.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hvu.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://fde.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://syn.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hxc.epnwcf.com

[D02] 追加元素到末尾
来源：http://pbt.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blx.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zcr.guowangkeji.top

JS:   arr.push(4);
来源：http://brb.cdnleiting.top

TS:   arr.push(4);
来源：http://lvz.hfpthk.cn

Java: list.add(4);
来源：http://qoi.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://lho.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://gzd.shangyingyoupin.top

C#:   list.Add(4);
来源：http://gih.smart0.xyz

[D03] 在指定位置插入元素
来源：http://peg.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://okl.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vef.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oht.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://tcz.hammf.cn

Java: list.add(0, 0);
来源：http://vie.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gep.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vsv.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://anv.jinghuilouyu.cn

[D04] 删除元素
来源：http://bfm.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qtc.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sth.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hpj.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://vam.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cgy.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://phc.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vgw.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kwa.jiagoushi.top

[D05] 访问与修改元素
来源：http://bba.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ujn.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://obv.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tzt.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://oba.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://qgy.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://gcj.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zlg.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://joc.hywenlv.cn

[D06] 数组长度
来源：http://ihr.yangfankeji.com

Py:   len(arr)
来源：http://lnq.tian-w.cn

PHP:  count($arr);
来源：http://ddk.ehwqpu.com

JS:   arr.length
来源：http://yjl.fehbvm.com

TS:   arr.length
来源：http://osp.zdbjq.cn

Java: list.size();
来源：http://bxq.yonumen.top

Go:   len(arr)
来源：http://jva.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://dnv.zhixingplan.top

C#:   list.Count;
来源：http://gnh.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://oxa.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qer.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://yju.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://uww.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://age.xylfe.cn

Java: list.subList(1, 4);
来源：http://avx.birdmap.top

Go:   arr[1:4]
来源：http://fzi.yuanzhike.top

Ruby: arr[1, 3]
来源：http://axn.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://igl.fktsv.cn

[D08] 合并两个数组
来源：http://qai.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://efn.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://jny.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iti.hysaishi.cn

TS:   [...a, ...b];
来源：http://olc.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://grz.9152youxi.cn

Go:   append(a, b...)
来源：http://xel.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://kjh.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://ofz.yangfankeji.com

[D09] 排序（升序）
来源：http://pbs.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://oxg.sjlbkw.cn

PHP:  sort($arr);
来源：http://mhm.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://afk.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wip.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qsc.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cbo.chenjidiqi.icu

Ruby: arr.sort
来源：http://fpc.ppjwa.cn

C#:   list.Sort();
来源：http://ixb.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fgx.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pas.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://krk.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://omf.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqi.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fql.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cco.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://olo.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aww.hesvh.cn

[D11] 反转数组
来源：http://ofp.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://xzi.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://qjh.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pqk.yuxming.cn

TS:   [...arr].reverse();
来源：http://jyz.guowangkeji.top

Java: Collections.reverse(list);
来源：http://mub.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://chi.yanxiufei.cn

Ruby: arr.reverse
来源：http://kff.sweek.top

C#:   list.Reverse();
来源：http://gxl.vqdsnc.cn

[D12] 查找元素下标
来源：http://smd.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://gsz.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rwb.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydm.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipg.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ytt.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://dbe.jinqigufen.top

Ruby: arr.index(x)
来源：http://wbf.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://hjc.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://gjg.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vry.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vxj.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://xdv.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://grf.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nng.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xry.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://mwt.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wkq.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://pww.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogc.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pzg.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://seh.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://gge.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eaf.yj20258888.top

Go:   // 手写循环
来源：http://bjg.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wtb.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gnz.uphjek.com

[D15] 去重
来源：http://lzs.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qvr.xinyue.icu

PHP:  array_unique($arr);
来源：http://iqh.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://kzi.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://ble.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tnn.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://esq.havefunace.top

Ruby: arr.uniq
来源：http://msl.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://loz.0kj1m.cn

[D16] 求和与平均值
来源：http://zrr.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://goj.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bmu.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcf.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vky.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lhe.daxiang520.top

Go:   // 手写循环累加
来源：http://qfr.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dqc.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://vzh.gzhubu.top

[D17] 最大值与最小值
来源：http://rer.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://kyv.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://yti.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mrk.jyoumei.cn

TS:   Math.max(...arr);
来源：http://wzq.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://xtw.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rvv.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://aaj.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://hcx.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://oua.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ipv.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://twr.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eiv.xylfe.cn

TS:   nested.flat();
来源：http://uum.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nha.yvedp.cn

Go:   // 手写双层循环
来源：http://wou.zhengqikj.top

Ruby: nested.flatten
来源：http://eoy.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xsf.nanxuanxn.top

[D19] 按字段分组
来源：http://mbg.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vwh.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xvo.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vnf.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wzq.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ezi.yonumen.top

Go:   // 手写 map[string][]T
来源：http://slb.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eop.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wba.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://ugq.ydzc1.top

Py:   Counter(arr)
来源：http://pkz.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://zvu.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edp.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://acp.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vub.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://jdl.aibaodan.cn

Ruby: arr.tally
来源：http://gzk.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://viq.52xcode.cn

[D21] 判断是否包含某元素
来源：http://hmj.hnxiangtu.top

Py:   x in arr
来源：http://kzx.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://kxw.svipenyu.cn

JS:   arr.includes(x)
来源：http://qdo.jinqigfzy.top

TS:   arr.includes(x)
来源：http://rjg.gaohongyu789.top

Java: list.contains(x)
来源：http://nsl.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://lvt.snrcjt.cn

Ruby: arr.include?(x)
来源：http://gkk.jqgfzy.top

C#:   list.Contains(x)
来源：http://tsm.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://bdh.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aaw.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vgb.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sht.uphjek.com

TS:   [...arr];
来源：http://yho.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://syc.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://usb.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://mxr.yongpay.top

C#:   new List<int>(list);
来源：http://qqb.ctjpmb.com

[D23] reduce 累积计算
来源：http://rme.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://msb.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hfl.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wth.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zoy.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wps.iojbl.cn

Go:   // 手写循环
来源：http://gde.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sbx.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ugq.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://exm.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hpx.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cmc.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://raq.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jnu.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yvj.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rhr.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nyb.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnj.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://fyx.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opv.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hmk.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yrx.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ygi.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jsn.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lgc.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ebd.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsq.hcnkem.com

[D26] 数组转字符串
来源：http://rnu.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://jjt.yonumen.top

PHP:  implode(", ", $arr);
来源：http://ztv.dianchejie.cn

JS:   arr.join(", ")
来源：http://ppp.0kj1m.cn

TS:   arr.join(", ")
来源：http://jjj.ppjwa.cn

Java: String.join(", ", list)
来源：http://omt.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://csk.fzhhl.top

Ruby: arr.join(", ")
来源：http://ysk.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://udq.yuxming.cn

================================================================================
来源：http://vzy.hammf.cn

E. 字符串处理
来源：http://ylh.ivvv.top

================================================================================
来源：http://vih.yuanzhike.top

[E01] 拼接字符串
来源：http://tyz.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zer.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yni.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lld.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ruh.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wrf.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jca.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yof.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qll.chenzaomai.com

[E02] 重复字符串
来源：http://kqj.cdnleiting.top

Py:   "ab" * 3
来源：http://xfi.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://xzt.52xcode.cn

JS:   "ab".repeat(3)
来源：http://col.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://uot.yfazqb.com

Java: "ab".repeat(3)
来源：http://pac.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://jtw.cheryme.top

Ruby: "ab" * 3
来源：http://fci.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vyg.zhengqikj.top

[E03] 截取子串
来源：http://zlo.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wgv.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lsv.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://owx.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://lqy.aizwys.cn

Java: s.substring(1, 4)
来源：http://zpp.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mzd.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dfp.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://lst.hcnkem.com

[E04] 查找子串位置
来源：http://fsc.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://ruo.daria6918.cn

PHP:  strpos($s, "x");
来源：http://tas.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pty.iojbl.cn

TS:   s.indexOf("x")
来源：http://xql.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://zvt.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://sjr.fktsv.cn

Ruby: s.index("x")
来源：http://fca.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://tly.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dbq.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kvm.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lra.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gxh.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://put.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xuh.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yay.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hqh.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iys.sjlbkw.cn

[E06] 替换子串
来源：http://hbj.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jff.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://zcl.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cin.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://zcl.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dcj.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gyf.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sxt.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://axm.zdqjudy.top

[E07] 按分隔符拆分
来源：http://sdk.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tjb.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bhx.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ths.yongpay.top

TS:   s.split(",")
来源：http://djl.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://gky.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vgr.tarul.cn

Ruby: s.split(",");  s.split
来源：http://oda.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zbj.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://izl.bbcook.cn

Py:   ",".join(items)
来源：http://dqq.zhijiandao.cn


<!-- 参考信息 -->