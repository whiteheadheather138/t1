代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://nub.ydzc1.top

TS:   [...a, ...b];
来源：http://nku.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dkr.9152youxi.cn

Go:   append(a, b...)
来源：http://vbl.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://ljg.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://emb.havefunace.top

[D09] 排序（升序）
来源：http://kul.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://pno.jiagoushi.top

PHP:  sort($arr);
来源：http://swl.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cuo.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hek.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nze.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://huz.aizwys.cn

Ruby: arr.sort
来源：http://hcq.fehbvm.com

C#:   list.Sort();
来源：http://fkm.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qrg.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nug.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyk.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nnu.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lxy.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egb.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zkd.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nld.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://crv.dashuyun.cn

[D11] 反转数组
来源：http://ldt.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://tep.sweek.top

PHP:  array_reverse($arr);
来源：http://dgd.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xse.aizwys.cn

TS:   [...arr].reverse();
来源：http://aft.birdmap.top

Java: Collections.reverse(list);
来源：http://waz.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://uyu.fzhhl.top

Ruby: arr.reverse
来源：http://udz.hnxiangtu.top

C#:   list.Reverse();
来源：http://sxl.meibo888.top

[D12] 查找元素下标
来源：http://sgk.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://epw.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kmt.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnx.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwp.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cdi.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://esr.guowangkeji.top

Ruby: arr.index(x)
来源：http://ybw.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://lwu.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://uiz.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nif.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bcs.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://jdv.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://rpy.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ghd.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tdm.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://skf.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kbe.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://smc.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rpm.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pew.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://rik.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://fce.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rnv.52xcode.cn

Go:   // 手写循环
来源：http://tci.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rys.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://opx.sweek.top

[D15] 去重
来源：http://jdb.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lhp.yj20258.top

PHP:  array_unique($arr);
来源：http://saf.316326.xyz

JS:   [...new Set(arr)]
来源：http://doj.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://nke.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zca.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://yxy.birdmap.top

Ruby: arr.uniq
来源：http://akt.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://dlv.zhiwuduotai.top

[D16] 求和与平均值
来源：http://rdj.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cvg.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vno.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aed.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntc.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://guu.epnwcf.com

Go:   // 手写循环累加
来源：http://zjk.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gmk.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://rpa.aibaodan.cn

[D17] 最大值与最小值
来源：http://gah.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://bvu.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://gdy.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvb.ivvv.top

TS:   Math.max(...arr);
来源：http://fki.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://azj.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mtp.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://sth.yj202588.top

C#:   list.Max();  list.Min()
来源：http://cdp.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://wsp.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://npd.sweek.top

PHP:  array_merge(...$nested);
来源：http://jgr.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://msh.fzhhl.top

TS:   nested.flat();
来源：http://kyu.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iip.haohaochexian.top

Go:   // 手写双层循环
来源：http://olq.hesvh.cn

Ruby: nested.flatten
来源：http://yxj.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ryh.xylfe.cn

[D19] 按字段分组
来源：http://zxz.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ddw.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://myc.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xwd.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rmz.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kmn.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://wbm.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://wox.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iod.yj202588.top

[D20] 统计每个元素出现次数
来源：http://tqd.yj20258.top

Py:   Counter(arr)
来源：http://wzv.fktsv.cn

PHP:  array_count_values($arr);
来源：http://idg.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://txc.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iok.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bww.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://irm.jinqigufen.top

Ruby: arr.tally
来源：http://hog.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gcb.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://rqa.sweek.top

Py:   x in arr
来源：http://nlh.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://yiw.tian-w.cn

JS:   arr.includes(x)
来源：http://ndx.hnxiangtu.top

TS:   arr.includes(x)
来源：http://qym.hfpthk.cn

Java: list.contains(x)
来源：http://xcw.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://ayf.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://fnj.zhoulong.xyz

C#:   list.Contains(x)
来源：http://htw.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://ddc.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xvv.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pdo.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bmv.hysaishi.cn

TS:   [...arr];
来源：http://dwi.yj20258.top

Java: new ArrayList<>(list);
来源：http://iwj.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ejb.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://etk.fengsongda.top

C#:   new List<int>(list);
来源：http://lec.andypj.xyz

[D23] reduce 累积计算
来源：http://gti.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vxj.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hzq.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpa.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhg.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ddo.smart0.xyz

Go:   // 手写循环
来源：http://eec.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dle.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ryr.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://fca.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bnb.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aua.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ncq.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hel.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kyd.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kkz.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fhc.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://smr.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wpk.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qye.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://snm.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nbg.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ayc.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jsz.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dwr.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kcp.havefunace.top

[D26] 数组转字符串
来源：http://iqc.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://fqk.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://cpi.jianghu66.top

JS:   arr.join(", ")
来源：http://fsc.hnqzz.top

TS:   arr.join(", ")
来源：http://loq.chenlongwang.top

Java: String.join(", ", list)
来源：http://slw.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://hdc.fehbvm.com

Ruby: arr.join(", ")
来源：http://qvc.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://bza.sjlbkw.cn

================================================================================
来源：http://dyd.daria6918.cn

E. 字符串处理
来源：http://opd.nwbrower.top

================================================================================
来源：http://cht.gaohongyu789.top

[E01] 拼接字符串
来源：http://cwz.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fpr.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qeq.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qsj.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kdi.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qwp.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jiq.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ech.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pdw.316326.xyz

[E02] 重复字符串
来源：http://nsh.iojbl.cn

Py:   "ab" * 3
来源：http://jcj.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://iqg.yj20258.top

JS:   "ab".repeat(3)
来源：http://lbn.gzhubu.top

TS:   "ab".repeat(3)
来源：http://ebg.hfpthk.cn

Java: "ab".repeat(3)
来源：http://nuw.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://jsp.smart0.xyz

Ruby: "ab" * 3
来源：http://rsw.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mxc.sweek.top

[E03] 截取子串
来源：http://mcl.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gdq.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://otg.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sxz.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://fhx.sufxvd.cn

Java: s.substring(1, 4)
来源：http://pyw.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://skh.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://pkn.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://wvr.cucudq.cn

[E04] 查找子串位置
来源：http://bxx.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://oef.cheryme.top

PHP:  strpos($s, "x");
来源：http://vjv.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wgn.0kj1m.cn

TS:   s.indexOf("x")
来源：http://ilg.xinyue.icu

Java: s.indexOf("x")
来源：http://dyc.yongpay.top

Go:   strings.Index(s, "x")
来源：http://adg.hesvh.cn

Ruby: s.index("x")
来源：http://fbv.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://igk.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cre.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbt.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xrc.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zkd.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://urv.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bat.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tuj.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bvv.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kvu.cheryme.top

[E06] 替换子串
来源：http://xux.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rpq.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://aum.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bjd.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://xkm.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://abw.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://san.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tch.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://bpw.fzhhl.top

[E07] 按分隔符拆分
来源：http://dgz.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bvp.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ffe.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://beh.zhoulong.xyz

TS:   s.split(",")
来源：http://hms.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qeq.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://peh.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://qsf.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nti.iojbl.cn

[E08] 数组按分隔符合并
来源：http://odl.jiagoushi.top

Py:   ",".join(items)
来源：http://nrl.chenlongwang.top

PHP:  implode(",", $items);
来源：http://olp.xylfe.cn

JS:   items.join(",")
来源：http://xji.tanke756.top

TS:   items.join(",")
来源：http://xbz.chenzaomai.com

Java: String.join(",", items)
来源：http://igp.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://hrw.hcnkem.com

Ruby: items.join(",")
来源：http://lzq.bbcook.cn

C#:   string.Join(",", items)
来源：http://puq.hysaishi.cn

[E09] 去除所有空白字符
来源：http://cbi.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jqi.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://faw.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://poz.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://wzt.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://mvs.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jlt.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rop.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mqr.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://lri.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jmd.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uab.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://rgm.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://lte.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://kdi.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rjw.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jih.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ase.xinyue.icu

[E11] 反转字符串
来源：http://vqw.xuanzx.com

Py:   s[::-1]
来源：http://ooh.fehbvm.com

PHP:  strrev($s);
来源：http://zkb.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://szn.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://vcy.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wus.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ijz.cheryme.top

Ruby: s.reverse
来源：http://gch.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tlj.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://xth.jqgfzy.top

Py:   s.count("a")
来源：http://ing.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://elt.guannengcc.top

JS:   s.split("a").length - 1
来源：http://arb.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://dyv.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://psv.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://haq.hysaishi.cn

Ruby: s.count("a")
来源：http://dcz.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://wtr.bjfxy.top

[E13] 逐字符遍历
来源：http://kuw.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://mxk.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://owm.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fhl.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cxz.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ury.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wrd.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pom.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://etf.hammf.cn

[E14] URL 编码与 Base64
来源：http://svw.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xwg.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://tpx.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bwb.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rso.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iqq.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fbo.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cch.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wdt.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://urh.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://lzb.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oky.tarul.cn


<!-- 参考信息 -->