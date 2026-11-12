代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://obi.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qwq.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sxp.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oou.ybcxt.top

[D11] 反转数组
来源：http://lqy.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yab.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://vvn.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vye.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://yso.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://hep.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://hlx.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://lkl.fzhhl.top

C#:   list.Reverse();
来源：http://zmg.svipenyu.cn

[D12] 查找元素下标
来源：http://poe.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://ngb.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tlk.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikk.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzg.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vjw.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://nss.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://npl.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://hee.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://dht.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuv.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://euv.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://nyb.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://jhh.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wxa.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ijr.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://vuw.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rzp.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://bnc.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vfb.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gch.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://ooo.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://nta.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://sdw.meibo888.top

Go:   // 手写循环
来源：http://ahe.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jlu.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://syd.shuidangran.top

[D15] 去重
来源：http://rue.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqs.zdqjudy.top

PHP:  array_unique($arr);
来源：http://nzc.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://gbl.vehdjk.com

TS:   [...new Set(arr)]
来源：http://nzo.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xti.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://hjj.sufxvd.cn

Ruby: arr.uniq
来源：http://epz.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://faf.vqdsnc.cn

[D16] 求和与平均值
来源：http://kop.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vtb.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://koy.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://der.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://drz.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qpb.ctjpmb.com

Go:   // 手写循环累加
来源：http://cmo.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uzx.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://rgc.hywenlv.cn

[D17] 最大值与最小值
来源：http://vrw.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://tgd.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://cad.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wdr.svipenyu.cn

TS:   Math.max(...arr);
来源：http://uxt.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oxu.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fyk.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://pds.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://pye.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://pbl.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://teo.ivvv.top

PHP:  array_merge(...$nested);
来源：http://lkj.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yrd.zhengqikj.top

TS:   nested.flat();
来源：http://gom.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pcp.shzxlz.cn

Go:   // 手写双层循环
来源：http://mws.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://wwg.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jaq.nanxuanxn.top

[D19] 按字段分组
来源：http://uob.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zrh.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddf.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rcj.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eoj.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kjp.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://ihp.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpt.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ulp.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://igd.gotoacloud.top

Py:   Counter(arr)
来源：http://gbe.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://viv.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zbd.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qjf.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wsg.yuxming.cn

Go:   // 手写 map[T]int
来源：http://gvj.chenzaomai.com

Ruby: arr.tally
来源：http://cit.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bpv.52xcode.cn

[D21] 判断是否包含某元素
来源：http://fzz.0kj1m.cn

Py:   x in arr
来源：http://nai.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://tzu.chenzaomai.com

JS:   arr.includes(x)
来源：http://xej.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://nfa.jlsjyb.cn

Java: list.contains(x)
来源：http://nkv.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://djy.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://tjh.tanke756.top

C#:   list.Contains(x)
来源：http://had.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://whn.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://itr.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vmn.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gae.hysaishi.cn

TS:   [...arr];
来源：http://bqq.tarul.cn

Java: new ArrayList<>(list);
来源：http://dsf.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://wai.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://brm.gzhubu.top

C#:   new List<int>(list);
来源：http://ieg.zdbjq.cn

[D23] reduce 累积计算
来源：http://bdc.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://whz.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vuh.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hba.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xqo.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://knl.uphjek.com

Go:   // 手写循环
来源：http://ked.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bsg.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mwk.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://sgr.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lma.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zhm.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbx.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://esm.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ipn.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ihq.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmx.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hfp.yonumen.top

[D25] Set 集合去重与交并差
来源：http://hnc.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kpv.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ozz.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dih.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zvb.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bbe.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kll.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tcz.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cvl.zdqjudy.top

[D26] 数组转字符串
来源：http://xcf.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://prj.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://ytx.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://xsv.tian-w.cn

TS:   arr.join(", ")
来源：http://sxr.wangdashe.top

Java: String.join(", ", list)
来源：http://gzl.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://gvu.xuanzx.com

Ruby: arr.join(", ")
来源：http://tqa.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://ive.c1oappe.top

================================================================================
来源：http://iph.iojbl.cn

E. 字符串处理
来源：http://gus.0kj1m.cn

================================================================================
来源：http://eqg.nanxinkj.top

[E01] 拼接字符串
来源：http://nzn.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gca.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fxt.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fji.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojq.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mkz.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lrk.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://taa.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uyc.vehdjk.com

[E02] 重复字符串
来源：http://imp.jqgufenzy.top

Py:   "ab" * 3
来源：http://wdv.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://fcq.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ltx.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://xwi.guannengcc.top

Java: "ab".repeat(3)
来源：http://zfi.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://mxz.tianlin.xyz

Ruby: "ab" * 3
来源：http://mwe.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://haf.jianghu66.top

[E03] 截取子串
来源：http://tco.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syv.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pxd.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wel.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://axb.ydzc1.top

Java: s.substring(1, 4)
来源：http://fpw.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ldh.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://ffh.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://tum.hongshengwenyu.top

[E04] 查找子串位置
来源：http://agm.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://usd.cashguo.top

PHP:  strpos($s, "x");
来源：http://oky.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obl.sysykeji.top

TS:   s.indexOf("x")
来源：http://qpu.bjfxy.top

Java: s.indexOf("x")
来源：http://pbl.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://jes.zhoulong.xyz

Ruby: s.index("x")
来源：http://fkl.guannengcc.top

C#:   s.IndexOf("x")
来源：http://kgo.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://muv.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zau.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yfh.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhn.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jwm.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wyg.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yqb.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kdc.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jjz.nwbrower.top

[E06] 替换子串
来源：http://qal.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bfj.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://yks.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eez.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://bcl.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yth.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oks.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iit.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://dmp.shuidangran.top

[E07] 按分隔符拆分
来源：http://umm.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kwo.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xup.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tnz.fzhhl.top

TS:   s.split(",")
来源：http://tgk.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://sch.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stk.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://tyo.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iio.daria6918.cn

[E08] 数组按分隔符合并
来源：http://uid.dashuyun.cn

Py:   ",".join(items)
来源：http://rsh.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://kpp.jqgufenzy.top

JS:   items.join(",")
来源：http://cge.jyoumei.cn

TS:   items.join(",")
来源：http://yce.jqgfzy.top

Java: String.join(",", items)
来源：http://jpf.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://zml.tarul.cn

Ruby: items.join(",")
来源：http://lsc.jyoumei.cn

C#:   string.Join(",", items)
来源：http://ftm.tian-w.cn

[E09] 去除所有空白字符
来源：http://rnk.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ewu.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xvl.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://ifi.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://zwz.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://sfh.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qrp.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://oca.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nfb.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://zwm.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qlk.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aee.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://dlk.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://nrt.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://rvl.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aeq.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eqk.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://trz.tianlin.xyz

[E11] 反转字符串
来源：http://qny.sufxvd.cn

Py:   s[::-1]
来源：http://btk.xylfe.cn

PHP:  strrev($s);
来源：http://akg.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://ziq.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://tav.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dxa.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zsd.feifeiyinyue.top

Ruby: s.reverse
来源：http://udw.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wgs.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://pes.fktsv.cn

Py:   s.count("a")
来源：http://rvj.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://nfv.pycfn.com

JS:   s.split("a").length - 1
来源：http://qfm.yongpay.top

TS:   s.split("a").length - 1
来源：http://scn.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lye.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://pmi.ctjpmb.com

Ruby: s.count("a")
来源：http://uzs.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://zlx.gaohongyu789.top

[E13] 逐字符遍历
来源：http://lyl.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://fjq.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eij.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdp.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cnx.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wrt.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://not.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bfe.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://els.gzhubu.top

[E14] URL 编码与 Base64
来源：http://yqx.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wfv.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qii.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dqc.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pmm.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eqs.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://chb.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kaq.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ces.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://top.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nex.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kyi.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ukn.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ymg.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://idt.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lxo.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dqu.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://snf.birdmap.top

[E16] 数字千分位
来源：http://msl.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://szi.0kj1m.cn

PHP:  number_format(1234567);
来源：http://cyp.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qas.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://otq.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kng.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xxj.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jhi.havefunace.top

C#:   1234567.ToString("N0")
来源：http://pip.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://tsk.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fqe.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hij.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tkj.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rzo.nanxuanxn.top


<!-- 参考信息 -->