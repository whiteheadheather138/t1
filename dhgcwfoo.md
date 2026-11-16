代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mpw.yuxming.cn

TS:   [...a, ...b];
来源：http://qbh.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pmo.52xcode.cn

Go:   append(a, b...)
来源：http://mxi.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://lpm.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://ayh.cheryme.top

[D09] 排序（升序）
来源：http://qeo.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://naa.zhijiandao.cn

PHP:  sort($arr);
来源：http://ydf.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cod.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ylo.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tpa.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xic.yonumen.top

Ruby: arr.sort
来源：http://zoj.hnqzz.top

C#:   list.Sort();
来源：http://cdr.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dav.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvb.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggr.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hft.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://awr.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gkg.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbr.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vcv.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://djn.bjfxy.top

[D11] 反转数组
来源：http://kei.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://fbn.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://vbt.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://urv.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://kru.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://coh.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://thg.jianghu66.top

Ruby: arr.reverse
来源：http://msg.sjlbkw.cn

C#:   list.Reverse();
来源：http://tah.vehdjk.com

[D12] 查找元素下标
来源：http://gdn.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://vzs.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://akm.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jxw.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uhc.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mtg.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://wyi.yfazqb.com

Ruby: arr.index(x)
来源：http://xmo.nwbrower.top

C#:   list.IndexOf(x);
来源：http://zao.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://nof.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yxb.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://imu.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://uxk.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://tws.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pxt.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aci.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://yph.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kqm.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://liy.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://irx.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tuj.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://uya.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://ahl.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vfe.zhongyouzk.top

Go:   // 手写循环
来源：http://qsi.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://zph.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gyo.shuidangran.top

[D15] 去重
来源：http://cpg.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://otb.yonumen.top

PHP:  array_unique($arr);
来源：http://sgp.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://lns.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://zzs.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vzq.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wsh.aizwys.cn

Ruby: arr.uniq
来源：http://mqz.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://ajq.dianchejie.cn

[D16] 求和与平均值
来源：http://zrc.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://txp.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oql.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxd.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iih.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vvr.smart0.xyz

Go:   // 手写循环累加
来源：http://yui.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://clr.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://gmd.shuidangran.top

[D17] 最大值与最小值
来源：http://zia.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://oqx.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://mum.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://emg.smart0.xyz

TS:   Math.max(...arr);
来源：http://law.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zws.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xhm.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://syb.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://uyh.meibo888.top

[D18] 扁平化嵌套数组
来源：http://xkb.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cyr.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://ypc.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sgv.tianlin.xyz

TS:   nested.flat();
来源：http://stg.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vbm.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://uoe.jinqigfzy.top

Ruby: nested.flatten
来源：http://kzv.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fmj.meibo888.top

[D19] 按字段分组
来源：http://xmy.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qex.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zoo.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xau.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kwe.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufv.meibo888.top

Go:   // 手写 map[string][]T
来源：http://chc.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kwx.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cre.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://qqe.jqgfzy.top

Py:   Counter(arr)
来源：http://mmh.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://cuv.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epp.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dph.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://waq.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://tod.fktsv.cn

Ruby: arr.tally
来源：http://xhq.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://agy.yueranfly.top

[D21] 判断是否包含某元素
来源：http://gdy.kuanghao11.cn

Py:   x in arr
来源：http://wqa.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://xjl.havefunace.top

JS:   arr.includes(x)
来源：http://dxw.havefunace.top

TS:   arr.includes(x)
来源：http://mqi.feifeiyinyue.top

Java: list.contains(x)
来源：http://neg.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://sdw.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://nsb.jyoumei.cn

C#:   list.Contains(x)
来源：http://qwa.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://ses.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pnl.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://giz.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fcp.yueranfly.top

TS:   [...arr];
来源：http://vrb.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://mtl.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://afk.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://hbm.mhx1999.top

C#:   new List<int>(list);
来源：http://gvx.hfpthk.cn

[D23] reduce 累积计算
来源：http://gqt.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xgs.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ucm.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfa.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxq.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://srj.0kj1m.cn

Go:   // 手写循环
来源：http://mbt.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qsi.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gsw.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://krd.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jfc.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uqs.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nih.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uuz.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sxv.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gac.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zln.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://auh.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://idb.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ekf.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://adj.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ljp.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jzz.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hsf.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kcd.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://btl.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://psa.sweek.top

[D26] 数组转字符串
来源：http://fiu.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://qyj.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://rto.dashuyun.cn

JS:   arr.join(", ")
来源：http://pqi.bjfxy.top

TS:   arr.join(", ")
来源：http://whe.ehwqpu.com

Java: String.join(", ", list)
来源：http://hdn.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://plp.cqqwz.cn

Ruby: arr.join(", ")
来源：http://yss.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://uug.zhiwuduotai.top

================================================================================
来源：http://idz.dianchejie.cn

E. 字符串处理
来源：http://yyn.mhx1999.top

================================================================================
来源：http://wgv.zhiwuduotai.top

[E01] 拼接字符串
来源：http://ill.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rmc.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fiw.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mvb.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfm.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ojg.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wav.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dnm.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mqr.hysaishi.cn

[E02] 重复字符串
来源：http://tfi.shuidangran.top

Py:   "ab" * 3
来源：http://pdr.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://atg.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://xdf.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://inq.0kj1m.cn

Java: "ab".repeat(3)
来源：http://tbi.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://ztv.shuidangran.top

Ruby: "ab" * 3
来源：http://eme.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://grw.cashguo.top

[E03] 截取子串
来源：http://snx.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zik.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yeh.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://spe.yfazqb.com

TS:   s.slice(1, 4)
来源：http://cat.birdmap.top

Java: s.substring(1, 4)
来源：http://exu.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bnl.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tde.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://por.redwolf501.top

[E04] 查找子串位置
来源：http://dto.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://tlv.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://kue.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rra.yj202588.top

TS:   s.indexOf("x")
来源：http://msu.sysykeji.top

Java: s.indexOf("x")
来源：http://axh.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://qwi.cdnleiting.top

Ruby: s.index("x")
来源：http://wxm.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://cvf.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jht.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcu.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bub.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://epx.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vja.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uby.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ysk.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ipk.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oax.fktsv.cn

[E06] 替换子串
来源：http://idi.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xoe.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://dqq.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://phv.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://lks.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://say.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tsr.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rrh.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://zdb.hesvh.cn

[E07] 按分隔符拆分
来源：http://uyw.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nrg.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://usk.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mvz.jlsjyb.cn

TS:   s.split(",")
来源：http://tsf.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hxp.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uts.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://hnr.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hnq.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://kgd.zdbjq.cn

Py:   ",".join(items)
来源：http://esq.shuidangran.top

PHP:  implode(",", $items);
来源：http://aff.zycfv.cn

JS:   items.join(",")
来源：http://fnz.cashguo.top

TS:   items.join(",")
来源：http://vak.yuanzhike.top

Java: String.join(",", items)
来源：http://szy.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://ogs.yvedp.cn

Ruby: items.join(",")
来源：http://brt.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://uhm.havefunace.top

[E09] 去除所有空白字符
来源：http://zud.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwu.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://etz.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://mrc.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://bge.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://ipt.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aey.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://ajb.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sfo.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://ppr.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hua.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rva.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://psw.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://sod.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://trd.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nbq.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jtw.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pji.guannengcc.top

[E11] 反转字符串
来源：http://lcd.guannengcc.top

Py:   s[::-1]
来源：http://cpa.cheryme.top

PHP:  strrev($s);
来源：http://cwa.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://ohz.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://pao.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jog.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://syw.haohaochexian.top

Ruby: s.reverse
来源：http://tdy.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ucx.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://nke.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://tbm.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://pfn.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://jwe.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://oua.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cys.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://gqw.vqdsnc.cn

Ruby: s.count("a")
来源：http://npg.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://zmd.iojbl.cn

[E13] 逐字符遍历
来源：http://hrm.316326.xyz

Py:   for ch in s: print(ch)
来源：http://boo.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zhy.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gkc.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ruh.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xvc.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mcc.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gej.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://atk.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://dvp.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yle.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://stp.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jfj.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mvl.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bpo.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ryc.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfr.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nih.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://tob.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hev.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyo.xinyue.icu


<!-- 参考信息 -->