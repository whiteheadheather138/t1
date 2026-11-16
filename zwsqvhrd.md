代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://avk.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://csq.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://qgh.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://ros.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ykz.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aqa.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ufd.yanxiufei.cn

[D06] 数组长度
来源：http://kki.aibaodan.cn

Py:   len(arr)
来源：http://nse.hysaishi.cn

PHP:  count($arr);
来源：http://kfz.ybcxt.top

JS:   arr.length
来源：http://ebg.meibo888.top

TS:   arr.length
来源：http://omo.xinyue.icu

Java: list.size();
来源：http://kpv.cdnleiting.top

Go:   len(arr)
来源：http://lxd.xziqi.cn

Ruby: arr.length; arr.size
来源：http://syz.zhoulong.xyz

C#:   list.Count;
来源：http://wev.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://lhm.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gmn.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://bgn.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://njt.birdmap.top

TS:   arr.slice(1, 4);
来源：http://imz.dashuyun.cn

Java: list.subList(1, 4);
来源：http://htl.fktsv.cn

Go:   arr[1:4]
来源：http://bvm.uphjek.com

Ruby: arr[1, 3]
来源：http://tps.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://lyu.jinqigfzy.top

[D08] 合并两个数组
来源：http://tyl.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://can.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://lwv.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jfe.hnxiangtu.top

TS:   [...a, ...b];
来源：http://vqn.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rdf.zdqjudy.top

Go:   append(a, b...)
来源：http://vdt.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://trc.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://qyl.feifeiyinyue.top

[D09] 排序（升序）
来源：http://avq.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://sqa.sxryk.cn

PHP:  sort($arr);
来源：http://xor.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eix.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://ala.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ila.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xrl.jlsjyb.cn

Ruby: arr.sort
来源：http://mok.daxiang520.top

C#:   list.Sort();
来源：http://cwa.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bvz.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zho.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vmn.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vtc.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eam.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rpi.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://btg.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xrg.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aay.316326.xyz

[D11] 反转数组
来源：http://hnu.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lfq.yj202588.top

PHP:  array_reverse($arr);
来源：http://tto.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gro.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://noi.fzhhl.top

Java: Collections.reverse(list);
来源：http://uyn.tanke756.top

Go:   slices.Reverse(arr)
来源：http://vxs.dianchejie.cn

Ruby: arr.reverse
来源：http://ivi.shuidangran.top

C#:   list.Reverse();
来源：http://mmv.chenzaomai.com

[D12] 查找元素下标
来源：http://jbr.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://ukj.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vwk.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjz.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jhq.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhe.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://qdc.sufxvd.cn

Ruby: arr.index(x)
来源：http://xoy.tarul.cn

C#:   list.IndexOf(x);
来源：http://prm.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://tlo.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pvi.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yjd.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://jpn.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://idq.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rro.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://itc.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://ccp.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ejb.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://nxi.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bre.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gzm.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://pcr.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://isk.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zpw.yanxiufei.cn

Go:   // 手写循环
来源：http://wkx.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://lxv.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hnx.hnqzz.top

[D15] 去重
来源：http://gip.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nrx.tanke756.top

PHP:  array_unique($arr);
来源：http://nec.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://muq.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://iez.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxw.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://jxi.hnxiangtu.top

Ruby: arr.uniq
来源：http://tkq.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://ktu.hysaishi.cn

[D16] 求和与平均值
来源：http://xtr.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://orh.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tge.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://whh.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxc.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gix.wangdashe.top

Go:   // 手写循环累加
来源：http://hvq.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://chj.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://fil.snrcjt.cn

[D17] 最大值与最小值
来源：http://ivu.316326.xyz

Py:   max(arr);  min(arr)
来源：http://wtl.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://nlq.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pit.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://vgz.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ajl.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hzk.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://nob.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://sfs.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://ruo.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ncr.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://fwg.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvr.andypj.xyz

TS:   nested.flat();
来源：http://cpj.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehf.hnxiangtu.top

Go:   // 手写双层循环
来源：http://bgv.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://ubd.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vyo.zdbjq.cn

[D19] 按字段分组
来源：http://gen.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ysl.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://asx.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://frl.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oxs.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fvb.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://qwu.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xaf.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gjf.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://vlw.vqdsnc.cn

Py:   Counter(arr)
来源：http://lps.cucudq.cn

PHP:  array_count_values($arr);
来源：http://xps.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrh.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kch.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://imn.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://rqs.cheryme.top

Ruby: arr.tally
来源：http://zuk.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vat.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://auv.shzxlz.cn

Py:   x in arr
来源：http://csx.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://yqm.epnwcf.com

JS:   arr.includes(x)
来源：http://ddx.jinqigufen.top

TS:   arr.includes(x)
来源：http://bbs.sxryk.cn

Java: list.contains(x)
来源：http://sxb.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://xes.gzhubu.top

Ruby: arr.include?(x)
来源：http://qgi.chenzaomai.com

C#:   list.Contains(x)
来源：http://pvs.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://jqs.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gve.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trw.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mve.hcnkem.com

TS:   [...arr];
来源：http://jpi.yueranfly.top

Java: new ArrayList<>(list);
来源：http://odo.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://dlp.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://qek.quarkkingdee.top

C#:   new List<int>(list);
来源：http://obd.ppjwa.cn

[D23] reduce 累积计算
来源：http://mjq.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gbi.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gyu.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxz.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rxe.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ugv.zhijiandao.cn

Go:   // 手写循环
来源：http://gbo.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nyg.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hfs.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://ueq.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohx.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cff.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dtp.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gli.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://njp.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jlr.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ojz.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nyd.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://ugm.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tmy.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gsf.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rog.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xbj.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uzw.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aut.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ppv.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xlw.xylfe.cn

[D26] 数组转字符串
来源：http://waq.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://ske.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://mva.nanxinkj.top

JS:   arr.join(", ")
来源：http://zxh.yongpay.top

TS:   arr.join(", ")
来源：http://xrl.hnqzz.top

Java: String.join(", ", list)
来源：http://xwu.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://rns.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://sek.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://ezv.iojbl.cn

================================================================================
来源：http://ria.c1oappe.top

E. 字符串处理
来源：http://jsi.316326.xyz

================================================================================
来源：http://dzn.shzxlz.cn

[E01] 拼接字符串
来源：http://qww.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://apr.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://asa.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://swj.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ium.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sbz.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cqt.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uac.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bca.xuanzx.com

[E02] 重复字符串
来源：http://vja.yfazqb.com

Py:   "ab" * 3
来源：http://sug.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://pau.pycfn.com

JS:   "ab".repeat(3)
来源：http://aiq.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://sdv.tanke756.top

Java: "ab".repeat(3)
来源：http://dri.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://aut.shuidangran.top

Ruby: "ab" * 3
来源：http://nnr.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hve.havefunace.top

[E03] 截取子串
来源：http://qcl.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wcm.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fql.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jpq.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://fjy.xuanzx.com

Java: s.substring(1, 4)
来源：http://hzz.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cxj.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ueq.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://njs.fengsongda.top

[E04] 查找子串位置
来源：http://dvi.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://erj.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://xlu.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://agz.pycfn.com

TS:   s.indexOf("x")
来源：http://gac.gaohongyu789.top

Java: s.indexOf("x")
来源：http://mhj.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://ecv.sufxvd.cn

Ruby: s.index("x")
来源：http://baf.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://hje.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://cwl.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fhk.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bnb.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcv.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxh.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fuw.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qie.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bjq.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xvb.meibo888.top

[E06] 替换子串
来源：http://laa.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ptl.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://qps.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wci.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://uhj.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqr.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://juk.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oym.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://jnw.cashguo.top

[E07] 按分隔符拆分
来源：http://ipr.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ykr.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://smy.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://yof.fktsv.cn

TS:   s.split(",")
来源：http://qeb.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zgt.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gip.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://olw.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cjj.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://fcy.dashuyun.cn

Py:   ",".join(items)
来源：http://qqv.zhixingplan.top

PHP:  implode(",", $items);
来源：http://ppg.chenzaomai.com

JS:   items.join(",")
来源：http://gng.hammf.cn

TS:   items.join(",")
来源：http://pql.jlsjyb.cn

Java: String.join(",", items)
来源：http://jmf.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://jqx.sweek.top

Ruby: items.join(",")
来源：http://qjz.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://tbn.daxiang520.top

[E09] 去除所有空白字符
来源：http://dqm.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fap.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zke.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://gip.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://kyl.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://upe.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wjp.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jni.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://twk.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://ncl.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qtw.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dhz.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://rnk.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://kok.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://xdd.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fey.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://flc.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://twa.epnwcf.com

[E11] 反转字符串
来源：http://ubp.zhiwuduotai.top

Py:   s[::-1]
来源：http://qhn.guannengcc.top

PHP:  strrev($s);
来源：http://rsq.cashguo.top

JS:   [...s].reverse().join("")
来源：http://fji.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://ixk.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ixs.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bne.jinghuilouyu.cn

Ruby: s.reverse
来源：http://xur.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://qcs.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://kor.meibo888.top

Py:   s.count("a")
来源：http://pyp.vqdsnc.cn


<!-- 参考信息 -->