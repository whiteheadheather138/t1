代发 wailian999

Java: list.size();
来源：http://jhw.shanyushiyangtech.top

Go:   len(arr)
来源：http://uvz.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://pir.sufxvd.cn

C#:   list.Count;
来源：http://oqq.fehbvm.com

[D07] 切片 / 取子数组
来源：http://kkg.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sub.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://hya.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://vhq.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://aqt.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://dyr.hongshengwenyu.top

Go:   arr[1:4]
来源：http://sru.hesvh.cn

Ruby: arr[1, 3]
来源：http://ahw.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://qrk.feifeiyinyue.top

[D08] 合并两个数组
来源：http://lll.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://wez.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://ofa.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mju.fzhhl.top

TS:   [...a, ...b];
来源：http://yxr.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eed.fehbvm.com

Go:   append(a, b...)
来源：http://kzj.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://nmg.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://neo.sysykeji.top

[D09] 排序（升序）
来源：http://rfk.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://qln.tarul.cn

PHP:  sort($arr);
来源：http://xhm.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fpx.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nvj.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://guh.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wae.gaohongyu789.top

Ruby: arr.sort
来源：http://pwt.316326.xyz

C#:   list.Sort();
来源：http://qka.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ymu.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cxw.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnj.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xwq.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rev.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyx.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ysk.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sgn.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://luq.shangyingyoupin.top

[D11] 反转数组
来源：http://odb.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxl.fzhhl.top

PHP:  array_reverse($arr);
来源：http://rat.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qzf.tianlin.xyz

TS:   [...arr].reverse();
来源：http://yuf.guannengcc.top

Java: Collections.reverse(list);
来源：http://yqm.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://mzn.shuidangran.top

Ruby: arr.reverse
来源：http://pmw.zycfv.cn

C#:   list.Reverse();
来源：http://eaf.wangdashe.top

[D12] 查找元素下标
来源：http://xti.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://wrw.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bwy.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wvc.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blp.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vwi.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://aqz.ehwqpu.com

Ruby: arr.index(x)
来源：http://kdi.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://euk.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://iav.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fsb.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ceg.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://okk.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://pho.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tmq.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://igx.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://uhl.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://psu.epnwcf.com

[D14] 映射转换（每个元素变形）
来源：http://nee.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wgu.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://plo.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://gil.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://ajn.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zeo.redwolf501.top

Go:   // 手写循环
来源：http://hia.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://avm.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vda.hesvh.cn

[D15] 去重
来源：http://cbv.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wrh.xinyue.icu

PHP:  array_unique($arr);
来源：http://wfb.shuidangran.top

JS:   [...new Set(arr)]
来源：http://sfe.yj202588.top

TS:   [...new Set(arr)]
来源：http://smp.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hhm.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xnn.yj202588.top

Ruby: arr.uniq
来源：http://srd.yj20258.top

C#:   list.Distinct().ToList()
来源：http://bna.yuxming.cn

[D16] 求和与平均值
来源：http://rum.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ldy.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vvw.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://scs.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ksn.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qts.sufxvd.cn

Go:   // 手写循环累加
来源：http://bfh.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ids.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://fap.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://xsz.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://vad.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://hwc.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wrr.redwolf501.top

TS:   Math.max(...arr);
来源：http://etz.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://qjy.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vmc.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://eap.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://tws.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://faw.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jjs.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://fut.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vjt.iojbl.cn

TS:   nested.flat();
来源：http://uaf.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oml.hywenlv.cn

Go:   // 手写双层循环
来源：http://ofe.zycfv.cn

Ruby: nested.flatten
来源：http://hlj.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nnj.yueranfly.top

[D19] 按字段分组
来源：http://kyr.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hkc.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://umx.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://caf.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://afj.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oey.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://poy.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cwc.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tbu.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://eft.zhoulong.xyz

Py:   Counter(arr)
来源：http://mhk.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://ynr.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxu.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smx.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lis.nwbrower.top

Go:   // 手写 map[T]int
来源：http://qim.ctjpmb.com

Ruby: arr.tally
来源：http://iqw.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://osy.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://uyx.meibo888.top

Py:   x in arr
来源：http://nfr.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://wyg.ppjwa.cn

JS:   arr.includes(x)
来源：http://ujm.birdmap.top

TS:   arr.includes(x)
来源：http://ash.sxryk.cn

Java: list.contains(x)
来源：http://nto.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://qlb.yuanzhike.top

Ruby: arr.include?(x)
来源：http://iwc.pycfn.com

C#:   list.Contains(x)
来源：http://mzx.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://cqo.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tdy.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yvq.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zwz.fehbvm.com

TS:   [...arr];
来源：http://rdp.havefunace.top

Java: new ArrayList<>(list);
来源：http://bio.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://yiu.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://cnv.mhx1999.top

C#:   new List<int>(list);
来源：http://qoi.ctjpmb.com

[D23] reduce 累积计算
来源：http://yxn.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pdq.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wqu.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yox.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rwf.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://euf.yj20258.top

Go:   // 手写循环
来源：http://vjh.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gzm.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pif.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://rig.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bqg.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwy.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijx.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rui.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hmu.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ojk.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pgf.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qui.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://ihk.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aia.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gqd.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zih.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dfs.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bha.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ojm.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vzp.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://moi.xziqi.cn

[D26] 数组转字符串
来源：http://gjq.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://otr.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://mor.snrcjt.cn

JS:   arr.join(", ")
来源：http://ero.daria6918.cn

TS:   arr.join(", ")
来源：http://mxu.redwolf501.top

Java: String.join(", ", list)
来源：http://lsl.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://iup.aizwys.cn

Ruby: arr.join(", ")
来源：http://ejx.yvedp.cn

C#:   string.Join(", ", list)
来源：http://anc.feifeiyinyue.top

================================================================================
来源：http://xsj.gaohongyu789.top

E. 字符串处理
来源：http://bkj.shuidangran.top

================================================================================
来源：http://iwo.havefunace.top

[E01] 拼接字符串
来源：http://lrs.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ivp.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uwc.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqf.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iwl.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ijw.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vxv.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wgr.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhj.cheryme.top

[E02] 重复字符串
来源：http://eaf.fktsv.cn

Py:   "ab" * 3
来源：http://def.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://dyx.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://nty.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://yat.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://nmr.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://dwc.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://osu.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hie.zhiwuduotai.top

[E03] 截取子串
来源：http://jzc.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fgl.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xfy.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oyw.sysykeji.top

TS:   s.slice(1, 4)
来源：http://xgn.bbcook.cn

Java: s.substring(1, 4)
来源：http://oby.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nle.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://pjj.yj202588.top

C#:   s.Substring(1, 3)
来源：http://nhn.redwolf501.top

[E04] 查找子串位置
来源：http://acm.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://ovc.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://qaf.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cce.yj20258888.top

TS:   s.indexOf("x")
来源：http://tdc.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://dvr.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://ufr.redwolf501.top

Ruby: s.index("x")
来源：http://zwp.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://iam.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iox.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ekp.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rky.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hce.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lsx.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptl.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hxg.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uax.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://clx.zycfv.cn

[E06] 替换子串
来源：http://kti.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hoo.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://sup.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bus.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://ybn.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rco.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lbw.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gaz.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://lou.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://fxt.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jxz.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uep.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gqz.gzhubu.top

TS:   s.split(",")
来源：http://hoz.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://lqd.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jat.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://dnf.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esd.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://oqm.chenlongwang.top

Py:   ",".join(items)
来源：http://dkl.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://lyp.xuetiantiany.cn

JS:   items.join(",")
来源：http://spp.yangfankeji.com

TS:   items.join(",")
来源：http://ecz.hfpthk.cn

Java: String.join(",", items)
来源：http://obp.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://hsc.xinyue.icu

Ruby: items.join(",")
来源：http://fln.zdbjq.cn

C#:   string.Join(",", items)
来源：http://mxn.tarul.cn

[E09] 去除所有空白字符
来源：http://ctq.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://svk.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bew.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://qpk.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://ccd.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://ove.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://mtl.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lzd.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://utl.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://rls.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpy.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wnc.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://ggq.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://hft.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://zwt.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ioq.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aoq.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ypx.mhx1999.top

[E11] 反转字符串
来源：http://imj.fanxiaobao.xyz

Py:   s[::-1]
来源：http://uro.dianchejie.cn

PHP:  strrev($s);
来源：http://ieo.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://yvy.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://fup.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://tev.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dze.yfazqb.com

Ruby: s.reverse
来源：http://qln.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://dvc.smart0.xyz

[E12] 统计某字符出现次数
来源：http://bwc.yvedp.cn

Py:   s.count("a")
来源：http://alm.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://jgd.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://zrh.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://ezd.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pmu.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://gzp.yj202588.top

Ruby: s.count("a")
来源：http://lbr.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://jlp.jyoumei.cn

[E13] 逐字符遍历
来源：http://oxg.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://pir.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bor.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fen.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eox.wangdashe.top


<!-- 参考信息 -->