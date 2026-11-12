代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ity.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://omw.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hnn.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yid.zhijiandao.cn

[D11] 反转数组
来源：http://fmt.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bqa.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://cik.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xue.wangdashe.top

TS:   [...arr].reverse();
来源：http://hud.wangdashe.top

Java: Collections.reverse(list);
来源：http://mks.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://fgy.meibo888.top

Ruby: arr.reverse
来源：http://ccj.smart0.xyz

C#:   list.Reverse();
来源：http://brx.yj202588.top

[D12] 查找元素下标
来源：http://mnn.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://deu.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efh.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykq.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iax.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gud.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://ytc.redwolf501.top

Ruby: arr.index(x)
来源：http://tsz.ydzc1.top

C#:   list.IndexOf(x);
来源：http://duc.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://fcz.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://san.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eeg.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://pxg.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://cxy.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zcs.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://taf.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://dxt.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vzj.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://gvm.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pmf.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://edq.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://pbj.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://ttl.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzn.yueranfly.top

Go:   // 手写循环
来源：http://ywo.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://iwt.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kwg.zhiwuduotai.top

[D15] 去重
来源：http://uoq.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zmr.guannengcc.top

PHP:  array_unique($arr);
来源：http://qxf.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://uwt.gzhubu.top

TS:   [...new Set(arr)]
来源：http://btz.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tcv.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://ixp.zhengqikj.top

Ruby: arr.uniq
来源：http://fmp.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://iiz.ydzc1.top

[D16] 求和与平均值
来源：http://hbn.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qiv.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cml.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ijd.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfo.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jtk.nwbrower.top

Go:   // 手写循环累加
来源：http://ewx.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lne.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://gnm.birdmap.top

[D17] 最大值与最小值
来源：http://urt.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://rhh.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://tzm.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tqo.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://fte.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xyr.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hvl.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://aff.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://peb.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://pzx.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gli.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://oxs.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://der.jqgufenzy.top

TS:   nested.flat();
来源：http://ptv.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://unf.c1oappe.top

Go:   // 手写双层循环
来源：http://zog.yj20258.top

Ruby: nested.flatten
来源：http://hpl.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bki.fengsongda.top

[D19] 按字段分组
来源：http://nna.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pod.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://onr.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://are.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kci.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jjq.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://alk.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fws.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vet.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://mnx.epnwcf.com

Py:   Counter(arr)
来源：http://udh.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://riq.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyt.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khu.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rje.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://kgw.pycfn.com

Ruby: arr.tally
来源：http://vta.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sdk.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://aqg.wangshuangyany.cn

Py:   x in arr
来源：http://wcb.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://zom.jinqigufen.top

JS:   arr.includes(x)
来源：http://aax.dianchejie.cn

TS:   arr.includes(x)
来源：http://oej.svipenyu.cn

Java: list.contains(x)
来源：http://amw.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://rpp.jqgfzy.top

Ruby: arr.include?(x)
来源：http://lnv.andypj.xyz

C#:   list.Contains(x)
来源：http://bpn.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://vfu.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jbc.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rpa.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lnx.ydzc1.top

TS:   [...arr];
来源：http://yma.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://tht.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://kse.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://pke.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://apy.jinqigfzy.top

[D23] reduce 累积计算
来源：http://jpc.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqp.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jtr.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysh.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://meb.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dnm.feifeiyinyue.top

Go:   // 手写循环
来源：http://xwb.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kxr.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hbo.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://mgt.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qrk.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://clg.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iuq.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gin.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sko.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kdq.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bun.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pjr.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://shu.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dec.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qwj.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://shp.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uzy.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ssj.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wzw.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eww.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ydn.hcnkem.com

[D26] 数组转字符串
来源：http://urf.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://ggs.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://iwq.gaohongyu789.top

JS:   arr.join(", ")
来源：http://owb.sweek.top

TS:   arr.join(", ")
来源：http://vyy.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://vmq.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://efq.chenlongwang.top

Ruby: arr.join(", ")
来源：http://nsu.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://qdi.meibo888.top

================================================================================
来源：http://vnq.mhx1999.top

E. 字符串处理
来源：http://abu.yueranfly.top

================================================================================
来源：http://aea.iojbl.cn

[E01] 拼接字符串
来源：http://wis.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://shw.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jtm.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://swv.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgs.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gqg.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rvz.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sbr.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kaq.nwbrower.top

[E02] 重复字符串
来源：http://rif.cqqwz.cn

Py:   "ab" * 3
来源：http://vvl.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://xuw.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://vho.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://onn.shuidangran.top

Java: "ab".repeat(3)
来源：http://eli.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://ffd.ydzc1.top

Ruby: "ab" * 3
来源：http://ffv.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vqt.wangdashe.top

[E03] 截取子串
来源：http://aly.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vnn.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpn.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oiv.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://nvp.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://qoo.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vvv.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://zjs.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://ykh.yonumen.top

[E04] 查找子串位置
来源：http://zgx.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://gmx.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://kkr.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pgr.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://kno.ppjwa.cn

Java: s.indexOf("x")
来源：http://ahz.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://kon.meibo888.top

Ruby: s.index("x")
来源：http://mzk.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://iqz.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dsn.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kaa.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dkq.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxi.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pcd.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ajr.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfn.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vfn.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zkh.smart0.xyz

[E06] 替换子串
来源：http://ysq.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ogf.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://kbz.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zkm.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://dsl.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyo.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lnp.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uar.yonumen.top

C#:   s.Replace("a", "b")
来源：http://yas.daria6918.cn

[E07] 按分隔符拆分
来源：http://gmi.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ohf.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wrf.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ida.dashuyun.cn

TS:   s.split(",")
来源：http://nst.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://ota.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xmo.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://wzc.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://plp.cheryme.top

[E08] 数组按分隔符合并
来源：http://azb.svipenyu.cn

Py:   ",".join(items)
来源：http://bdd.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://yal.yanxiufei.cn

JS:   items.join(",")
来源：http://azh.yongpay.top

TS:   items.join(",")
来源：http://cwr.zdbjq.cn

Java: String.join(",", items)
来源：http://lcs.yonumen.top

Go:   strings.Join(items, ",")
来源：http://svr.xziqi.cn

Ruby: items.join(",")
来源：http://dkx.havefunace.top

C#:   string.Join(",", items)
来源：http://yed.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://ncg.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hlj.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jrc.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://vjt.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://yhq.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://rwj.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfi.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://gth.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vfw.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://hep.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mmu.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vvm.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://bvv.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://hez.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://ush.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zpt.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fwe.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eow.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://fgq.fengsongda.top

Py:   s[::-1]
来源：http://hcx.cqqwz.cn

PHP:  strrev($s);
来源：http://zyy.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://wex.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://ebw.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://coc.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rmo.52xcode.cn

Ruby: s.reverse
来源：http://dhc.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://hbu.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://iaf.jinqigufen.top

Py:   s.count("a")
来源：http://ypi.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://iev.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://khy.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://yqg.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lci.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://pig.yangfankeji.com

Ruby: s.count("a")
来源：http://gyj.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://yiu.jlsjyb.cn

[E13] 逐字符遍历
来源：http://tpn.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://psa.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hpp.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lra.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ord.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uhd.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ytm.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://wxj.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://php.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://lwn.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lmb.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bgi.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qfl.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xlu.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zaz.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hed.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ywn.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vxo.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://hpg.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ufx.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ndg.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iam.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rrb.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hql.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xan.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kjx.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jti.zycfv.cn

[E16] 数字千分位
来源：http://isv.yuxming.cn

Py:   f"{1234567:,}"
来源：http://trw.haohaochexian.top

PHP:  number_format(1234567);
来源：http://hek.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://diz.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jml.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pzd.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hae.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://shx.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://uuj.nanxinkj.top

[E17] 首字母大写
来源：http://jhl.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://znu.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jez.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rfk.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gqh.c1oappe.top


<!-- 参考信息 -->