代发 wailian999

PHP:  sort($arr);
来源：http://myj.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lyp.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://edd.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://djb.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fos.kuanghao11.cn

Ruby: arr.sort
来源：http://bsw.snrcjt.cn

C#:   list.Sort();
来源：http://pdf.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://trz.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gno.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpw.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcn.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xmw.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://grq.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aqq.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rri.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cpc.ehwqpu.com

[D11] 反转数组
来源：http://mmk.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mse.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://mlr.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eho.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://cfy.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://zvr.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://noi.cucudq.cn

Ruby: arr.reverse
来源：http://pmf.sweek.top

C#:   list.Reverse();
来源：http://xav.xuetiantiany.cn

[D12] 查找元素下标
来源：http://qnz.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://npa.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ged.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gye.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wcd.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxb.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://erc.sysykeji.top

Ruby: arr.index(x)
来源：http://rzw.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://qyd.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://vpg.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oxn.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syy.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://auu.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://cmf.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smo.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zpn.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://jiq.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vjd.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://ypn.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iow.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://huh.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://ods.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://rpq.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ips.vqdsnc.cn

Go:   // 手写循环
来源：http://tad.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bbj.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ngp.316326.xyz

[D15] 去重
来源：http://sug.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qal.yonumen.top

PHP:  array_unique($arr);
来源：http://vle.vehdjk.com

JS:   [...new Set(arr)]
来源：http://aqd.fehbvm.com

TS:   [...new Set(arr)]
来源：http://oxj.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gtg.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ham.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://ndq.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://zix.ehwqpu.com

[D16] 求和与平均值
来源：http://uhf.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tbd.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dpt.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvh.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://edx.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qbs.hcnkem.com

Go:   // 手写循环累加
来源：http://hui.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hqc.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://cqz.yonumen.top

[D17] 最大值与最小值
来源：http://brs.yj20258.top

Py:   max(arr);  min(arr)
来源：http://xqg.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://ykv.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://quz.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://szd.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pst.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uyr.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://jrr.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://lhf.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://yxp.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayh.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://iti.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zaw.aibaodan.cn

TS:   nested.flat();
来源：http://vju.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uhh.nwbrower.top

Go:   // 手写双层循环
来源：http://wle.xuanzx.com

Ruby: nested.flatten
来源：http://xgr.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://uah.gzhubu.top

[D19] 按字段分组
来源：http://gaf.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tbd.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vxb.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zyx.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://llm.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rvd.yj202588.top

Go:   // 手写 map[string][]T
来源：http://yqd.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://old.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xnh.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://jrv.yj20258888.top

Py:   Counter(arr)
来源：http://gbi.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://sim.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sly.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://szc.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rrh.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://wid.sweek.top

Ruby: arr.tally
来源：http://ztz.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qlw.yj202588.top

[D21] 判断是否包含某元素
来源：http://gfd.meibo888.top

Py:   x in arr
来源：http://zxw.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://fzk.chenlongwang.top

JS:   arr.includes(x)
来源：http://ggu.zdqjudy.top

TS:   arr.includes(x)
来源：http://lvg.guowangkeji.top

Java: list.contains(x)
来源：http://xsm.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://rsf.cqqwz.cn

Ruby: arr.include?(x)
来源：http://fzr.yfazqb.com

C#:   list.Contains(x)
来源：http://vot.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://rgt.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vgt.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zui.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwk.fengsongda.top

TS:   [...arr];
来源：http://ztv.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://dyv.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://qmg.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://azn.yuanzhike.top

C#:   new List<int>(list);
来源：http://gyg.xylfe.cn

[D23] reduce 累积计算
来源：http://ypt.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://awz.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yfz.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jwh.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aip.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dbh.zhijiandao.cn

Go:   // 手写循环
来源：http://sdi.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rco.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jvb.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://ugn.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pwz.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pqj.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sgb.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tvw.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jik.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zhu.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ntj.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tbf.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://eyt.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qnm.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bzd.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ywn.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tya.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://luc.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bnu.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tdt.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://imf.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://tlr.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://qlq.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://spe.hnxiangtu.top

JS:   arr.join(", ")
来源：http://slb.hesvh.cn

TS:   arr.join(", ")
来源：http://nmy.sjlbkw.cn

Java: String.join(", ", list)
来源：http://uex.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://nbm.9152youxi.cn

Ruby: arr.join(", ")
来源：http://qzl.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://idl.chenzaomai.com

================================================================================
来源：http://url.hfpthk.cn

E. 字符串处理
来源：http://auk.zhengqikj.top

================================================================================
来源：http://gqj.jianghu66.top

[E01] 拼接字符串
来源：http://nsi.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cgm.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wdx.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tdr.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pty.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ijd.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://giz.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uir.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jiv.xziqi.cn

[E02] 重复字符串
来源：http://kyo.tian-w.cn

Py:   "ab" * 3
来源：http://dqq.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://fpm.ydzc1.top

JS:   "ab".repeat(3)
来源：http://plo.vehdjk.com

TS:   "ab".repeat(3)
来源：http://xik.vehdjk.com

Java: "ab".repeat(3)
来源：http://ryb.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://spz.havefunace.top

Ruby: "ab" * 3
来源：http://tar.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gfk.sweek.top

[E03] 截取子串
来源：http://zzv.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://egy.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://djs.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mnn.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://gfx.nanxinkj.top

Java: s.substring(1, 4)
来源：http://ylj.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aox.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zvx.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://ovb.dashuyun.cn

[E04] 查找子串位置
来源：http://the.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://nsy.cucudq.cn

PHP:  strpos($s, "x");
来源：http://mzf.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yjq.nwbrower.top

TS:   s.indexOf("x")
来源：http://yhn.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://pnc.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://kvz.chenlongwang.top

Ruby: s.index("x")
来源：http://nss.birdmap.top

C#:   s.IndexOf("x")
来源：http://nas.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zgk.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://veo.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://agp.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xta.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ndj.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kyo.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://obj.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://twi.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cjm.ctjpmb.com

[E06] 替换子串
来源：http://yfb.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lwc.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://wbt.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ghl.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://lpc.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvh.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xgq.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dql.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://hzx.xylfe.cn

[E07] 按分隔符拆分
来源：http://yux.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xyp.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fdm.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xfi.redwolf501.top

TS:   s.split(",")
来源：http://axh.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mab.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vuj.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://hhx.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kyt.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://fzk.quarkkingdee.top

Py:   ",".join(items)
来源：http://wfv.yangfankeji.com

PHP:  implode(",", $items);
来源：http://gzc.andypj.xyz

JS:   items.join(",")
来源：http://llr.daxiang520.top

TS:   items.join(",")
来源：http://ctw.svipenyu.cn

Java: String.join(",", items)
来源：http://kxl.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://uyv.hcnkem.com

Ruby: items.join(",")
来源：http://gtz.ybcxt.top

C#:   string.Join(",", items)
来源：http://gsw.yvedp.cn

[E09] 去除所有空白字符
来源：http://xdg.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uju.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qlz.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://seb.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://zpc.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://dnl.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://azj.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://jdr.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwu.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://ogr.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vho.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wqo.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://ijv.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://snw.nwbrower.top

Java: String.format("%03d", 7)
来源：http://wqp.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihz.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://znt.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://unx.smart0.xyz

[E11] 反转字符串
来源：http://usb.gotoacloud.top

Py:   s[::-1]
来源：http://hrl.cqqwz.cn

PHP:  strrev($s);
来源：http://agu.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://chr.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://boq.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iiy.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhw.gogol.net.cn

Ruby: s.reverse
来源：http://dcb.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://uhs.sweek.top

[E12] 统计某字符出现次数
来源：http://nyg.ybcxt.top

Py:   s.count("a")
来源：http://vzh.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://yks.hnqzz.top

JS:   s.split("a").length - 1
来源：http://twq.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://hbw.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hlp.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://xug.bbcook.cn

Ruby: s.count("a")
来源：http://qaw.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://lwv.yanxiufei.cn

[E13] 逐字符遍历
来源：http://cbv.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://vsf.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bgp.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgc.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://cmy.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vql.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fjz.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://bnm.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fyg.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://kha.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcv.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldt.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://smp.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cod.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nfj.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uon.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://psj.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gvk.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://irm.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tyi.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://weq.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qei.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://puq.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycm.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://epa.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cfr.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ouo.dashuyun.cn

[E16] 数字千分位
来源：http://nuh.cheryme.top

Py:   f"{1234567:,}"
来源：http://ury.zdbjq.cn


<!-- 参考信息 -->