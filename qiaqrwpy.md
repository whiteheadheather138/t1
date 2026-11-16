代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://ojp.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://ijm.gaohongyu789.top

[D09] 排序（升序）
来源：http://wei.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://edq.yangfankeji.com

PHP:  sort($arr);
来源：http://mwq.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zsv.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tya.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://shd.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://onq.jianghu66.top

Ruby: arr.sort
来源：http://brd.xuetiantiany.cn

C#:   list.Sort();
来源：http://zky.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vxc.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bii.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cir.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bzt.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yut.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ugu.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipl.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uwl.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://egf.yuxming.cn

[D11] 反转数组
来源：http://pit.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://mmz.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://dsy.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryk.haohaochexian.top

TS:   [...arr].reverse();
来源：http://yvh.redwolf501.top

Java: Collections.reverse(list);
来源：http://ibt.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://xtd.wangshuangyany.cn

Ruby: arr.reverse
来源：http://ysu.jiagoushi.top

C#:   list.Reverse();
来源：http://gil.ehwqpu.com

[D12] 查找元素下标
来源：http://ine.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://hex.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ydj.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jun.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://egh.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ivr.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://emn.fengsongda.top

Ruby: arr.index(x)
来源：http://uij.redwolf501.top

C#:   list.IndexOf(x);
来源：http://map.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://jcp.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oxc.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kwj.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://gru.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://vmg.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kbj.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rxd.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sbx.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://trs.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://yrr.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mmx.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jap.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://xyy.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://koi.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vbc.sysykeji.top

Go:   // 手写循环
来源：http://drc.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://dha.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xxq.meibo888.top

[D15] 去重
来源：http://teb.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dsc.yangfankeji.com

PHP:  array_unique($arr);
来源：http://ejc.316326.xyz

JS:   [...new Set(arr)]
来源：http://anf.hesvh.cn

TS:   [...new Set(arr)]
来源：http://cxp.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://umi.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://uks.redwolf501.top

Ruby: arr.uniq
来源：http://pgn.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://gwz.gogol.net.cn

[D16] 求和与平均值
来源：http://shs.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ilm.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qzb.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kzz.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oex.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tke.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://ziv.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dfs.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://rwk.yj202588.top

[D17] 最大值与最小值
来源：http://wvl.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://mbd.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://zpy.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qyc.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://wak.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rae.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eui.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://szv.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://mvb.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://hva.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://slr.yonumen.top

PHP:  array_merge(...$nested);
来源：http://hkp.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://grt.cheryme.top

TS:   nested.flat();
来源：http://wtp.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qqe.smart0.xyz

Go:   // 手写双层循环
来源：http://nsq.sjlbkw.cn

Ruby: nested.flatten
来源：http://sgp.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hxg.iojbl.cn

[D19] 按字段分组
来源：http://nww.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://umf.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wrf.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xmt.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bnf.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tpb.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://yas.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://inc.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bzp.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://rwp.jinqigfzy.top

Py:   Counter(arr)
来源：http://eby.sxryk.cn

PHP:  array_count_values($arr);
来源：http://jld.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://duv.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyj.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://udd.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://biv.9152youxi.cn

Ruby: arr.tally
来源：http://zmj.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://urv.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://nwy.ydjk.org.cn

Py:   x in arr
来源：http://jrl.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://mzv.hammf.cn

JS:   arr.includes(x)
来源：http://shl.sxryk.cn

TS:   arr.includes(x)
来源：http://oid.shuidangran.top

Java: list.contains(x)
来源：http://hxm.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://ydg.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://wkz.wangdashe.top

C#:   list.Contains(x)
来源：http://ehz.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://vdc.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rzi.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://var.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://efl.gzhubu.top

TS:   [...arr];
来源：http://zcx.uphjek.com

Java: new ArrayList<>(list);
来源：http://mvw.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://meh.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://ehb.havefunace.top

C#:   new List<int>(list);
来源：http://ivp.jianghu66.top

[D23] reduce 累积计算
来源：http://uon.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ofa.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lvf.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mwi.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgd.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fsi.zhengqikj.top

Go:   // 手写循环
来源：http://fpf.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ezj.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jox.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://hau.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vwb.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qtc.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://own.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qwq.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xif.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aol.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pow.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hro.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://yrq.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ahs.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gex.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qqw.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://thf.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rnp.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tjr.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pel.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dce.jqgufenzy.top

[D26] 数组转字符串
来源：http://pmz.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://jzd.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://jus.tanke756.top

JS:   arr.join(", ")
来源：http://mrw.ppjwa.cn

TS:   arr.join(", ")
来源：http://yzp.tianlin.xyz

Java: String.join(", ", list)
来源：http://eis.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://fvb.gotoacloud.top

Ruby: arr.join(", ")
来源：http://dwx.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://zpq.fzhhl.top

================================================================================
来源：http://rcr.tarul.cn

E. 字符串处理
来源：http://eps.hysaishi.cn

================================================================================
来源：http://enj.gzhubu.top

[E01] 拼接字符串
来源：http://kni.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ran.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dtx.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cgg.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cag.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ind.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mun.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wvv.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vvy.shzxlz.cn

[E02] 重复字符串
来源：http://wse.tian-w.cn

Py:   "ab" * 3
来源：http://hyc.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://xuo.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://pnh.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://mlv.ivvv.top

Java: "ab".repeat(3)
来源：http://juo.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://ovo.wangdashe.top

Ruby: "ab" * 3
来源：http://lmn.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://huc.yangfankeji.com

[E03] 截取子串
来源：http://nld.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eqn.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zkg.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sdg.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://xpf.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://zcb.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qbf.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://fau.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://kll.guannengcc.top

[E04] 查找子串位置
来源：http://knl.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://arv.c1oappe.top

PHP:  strpos($s, "x");
来源：http://cmb.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://scb.svipenyu.cn

TS:   s.indexOf("x")
来源：http://tzw.gogol.net.cn

Java: s.indexOf("x")
来源：http://woj.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://mqs.tarul.cn

Ruby: s.index("x")
来源：http://goo.pycfn.com

C#:   s.IndexOf("x")
来源：http://udr.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pjo.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ycc.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://idp.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eei.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://cgq.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xaj.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jae.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jaq.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wmi.sxryk.cn

[E06] 替换子串
来源：http://upt.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wjk.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://nrl.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oab.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://crz.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wef.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yyc.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://way.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://vog.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://yvr.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vya.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zzw.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zmn.gotoacloud.top

TS:   s.split(",")
来源：http://shm.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://auu.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://big.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://pmd.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ntj.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://cpo.bjfxy.top

Py:   ",".join(items)
来源：http://icc.zycfv.cn

PHP:  implode(",", $items);
来源：http://zoi.yfazqb.com

JS:   items.join(",")
来源：http://wml.fengsongda.top

TS:   items.join(",")
来源：http://afb.c1oappe.top

Java: String.join(",", items)
来源：http://tco.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://djx.jyoumei.cn

Ruby: items.join(",")
来源：http://qrx.aibaodan.cn

C#:   string.Join(",", items)
来源：http://qpn.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://ntc.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vlo.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vrm.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ddb.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://zmc.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rsk.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yzv.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://muf.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vjm.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://bsm.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gim.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://auf.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://lzd.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://qan.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://kwn.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xhc.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://djy.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://owy.hcnkem.com

[E11] 反转字符串
来源：http://cml.chenjidiqi.icu

Py:   s[::-1]
来源：http://tnu.tanke756.top

PHP:  strrev($s);
来源：http://fdk.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://qdl.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://dve.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://idq.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://iac.cdnleiting.top

Ruby: s.reverse
来源：http://wcv.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://xzg.cucudq.cn

[E12] 统计某字符出现次数
来源：http://old.pengpengdd.cyou

Py:   s.count("a")
来源：http://que.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://fsr.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://nwk.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://gfg.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yov.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://vta.quarkkingdee.top

Ruby: s.count("a")
来源：http://tzr.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://xdi.cdnleiting.top

[E13] 逐字符遍历
来源：http://upa.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://ocq.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wxf.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://fky.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zel.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ydx.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tht.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://spq.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bko.epnwcf.com

[E14] URL 编码与 Base64
来源：http://iri.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ymk.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zib.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qvr.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kmv.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uzx.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hfy.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gfq.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jfb.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://trm.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fpa.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pzt.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://peg.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nda.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mtq.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ilw.zhengqikj.top


<!-- 参考信息 -->