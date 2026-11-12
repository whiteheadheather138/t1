代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://jxj.9152youxi.cn

[D08] 合并两个数组
来源：http://sgw.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://vew.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://kvr.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vzk.vehdjk.com

TS:   [...a, ...b];
来源：http://tbn.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://olx.sufxvd.cn

Go:   append(a, b...)
来源：http://blv.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://nfd.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://ruh.guowangkeji.top

[D09] 排序（升序）
来源：http://isn.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://nsz.xuetiantiany.cn

PHP:  sort($arr);
来源：http://pjn.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mik.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aql.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://iii.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xne.gzhubu.top

Ruby: arr.sort
来源：http://pnc.yj20258.top

C#:   list.Sort();
来源：http://ffe.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://txg.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xsv.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfh.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vye.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hwm.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://prz.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://glj.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bya.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rrm.fzhhl.top

[D11] 反转数组
来源：http://lca.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://jmj.yuxming.cn

PHP:  array_reverse($arr);
来源：http://xje.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zpy.sweek.top

TS:   [...arr].reverse();
来源：http://eex.sweek.top

Java: Collections.reverse(list);
来源：http://kmn.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://tlp.tarul.cn

Ruby: arr.reverse
来源：http://tot.quarkkingdee.top

C#:   list.Reverse();
来源：http://plk.yanxiufei.cn

[D12] 查找元素下标
来源：http://jap.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://dav.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ioj.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wvq.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldk.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dky.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://bpz.daria6918.cn

Ruby: arr.index(x)
来源：http://mdl.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://rdt.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://lvr.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aex.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ixz.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://ovw.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://txx.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jsc.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nrq.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://oev.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rkc.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://nwc.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://srf.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pgr.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://man.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://ety.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vgy.xinyue.icu

Go:   // 手写循环
来源：http://rdf.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://tpv.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://otf.ydzc1.top

[D15] 去重
来源：http://jwb.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kow.jyoumei.cn

PHP:  array_unique($arr);
来源：http://lmp.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://asb.hcnkem.com

TS:   [...new Set(arr)]
来源：http://otr.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cyc.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ihc.jiagoushi.top

Ruby: arr.uniq
来源：http://cfj.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://dfp.iojbl.cn

[D16] 求和与平均值
来源：http://ked.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bng.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hqh.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yto.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hnf.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mfl.zycfv.cn

Go:   // 手写循环累加
来源：http://ymh.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://apl.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://iwa.redwolf501.top

[D17] 最大值与最小值
来源：http://fwi.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://jxo.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://mqw.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://faf.yuxming.cn

TS:   Math.max(...arr);
来源：http://utw.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://tgw.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rpa.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://jck.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://sbd.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://iaj.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://quq.316326.xyz

PHP:  array_merge(...$nested);
来源：http://hia.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mot.havefunace.top

TS:   nested.flat();
来源：http://opl.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yva.xinyue.icu

Go:   // 手写双层循环
来源：http://wmw.aizwys.cn

Ruby: nested.flatten
来源：http://vty.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dpf.nanxuanxn.top

[D19] 按字段分组
来源：http://mba.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xho.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hgm.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xjw.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwk.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gnr.tarul.cn

Go:   // 手写 map[string][]T
来源：http://xrf.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://svl.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dtl.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://ejp.hesvh.cn

Py:   Counter(arr)
来源：http://zqh.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://aja.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://odx.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyn.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://grf.wangdashe.top

Go:   // 手写 map[T]int
来源：http://ivw.zhongyouzk.top

Ruby: arr.tally
来源：http://kgo.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmd.fktsv.cn

[D21] 判断是否包含某元素
来源：http://nnp.fzhhl.top

Py:   x in arr
来源：http://tmm.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://oge.cashguo.top

JS:   arr.includes(x)
来源：http://qpb.jlsjyb.cn

TS:   arr.includes(x)
来源：http://edt.nanxuanxn.top

Java: list.contains(x)
来源：http://xgy.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://glh.yongpay.top

Ruby: arr.include?(x)
来源：http://vrx.hywenlv.cn

C#:   list.Contains(x)
来源：http://olw.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://hkz.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dib.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rdc.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tgj.hammf.cn

TS:   [...arr];
来源：http://dmw.jianghu66.top

Java: new ArrayList<>(list);
来源：http://bjv.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bxs.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://kai.chenzaomai.com

C#:   new List<int>(list);
来源：http://mam.cashguo.top

[D23] reduce 累积计算
来源：http://ort.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://inm.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dby.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ixr.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vza.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://irw.mhx1999.top

Go:   // 手写循环
来源：http://nkn.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tgh.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zpd.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://ged.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jpb.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://goo.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://txv.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wby.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cez.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blh.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mxp.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://idi.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://mhy.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://khx.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cfl.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vys.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yyu.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ixl.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://coi.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qkv.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bay.fktsv.cn

[D26] 数组转字符串
来源：http://hiq.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://qvz.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://caq.jiagoushi.top

JS:   arr.join(", ")
来源：http://vik.redwolf501.top

TS:   arr.join(", ")
来源：http://gqi.yongpay.top

Java: String.join(", ", list)
来源：http://dgf.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://tat.nanxinkj.top

Ruby: arr.join(", ")
来源：http://rcg.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://shq.yonumen.top

================================================================================
来源：http://jql.vehdjk.com

E. 字符串处理
来源：http://zji.wangdashe.top

================================================================================
来源：http://mis.tarul.cn

[E01] 拼接字符串
来源：http://hji.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zud.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bkv.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dwj.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pds.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wwb.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjo.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qey.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cgk.nanxinkj.top

[E02] 重复字符串
来源：http://ojj.yangfankeji.com

Py:   "ab" * 3
来源：http://ont.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://wha.fengsongda.top

JS:   "ab".repeat(3)
来源：http://pnt.hnqzz.top

TS:   "ab".repeat(3)
来源：http://sgv.yj20258888.top

Java: "ab".repeat(3)
来源：http://ehk.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://dfj.sysykeji.top

Ruby: "ab" * 3
来源：http://ijy.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://crm.daria6918.cn

[E03] 截取子串
来源：http://jhx.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tjm.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dae.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vmj.vehdjk.com

TS:   s.slice(1, 4)
来源：http://dpr.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://jhj.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zlz.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://gwz.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://zch.aibaodan.cn

[E04] 查找子串位置
来源：http://zbv.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://pil.ybcxt.top

PHP:  strpos($s, "x");
来源：http://gew.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://akk.iojbl.cn

TS:   s.indexOf("x")
来源：http://tyn.quarkkingdee.top

Java: s.indexOf("x")
来源：http://pan.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://png.xuetiantiany.cn

Ruby: s.index("x")
来源：http://zlh.yj20258888.top

C#:   s.IndexOf("x")
来源：http://czl.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://luc.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://swn.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ohh.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avx.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wzv.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dfw.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jyr.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pht.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zvr.haohaochexian.top

[E06] 替换子串
来源：http://hsq.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jmj.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://pmp.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://und.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://isv.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhv.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://csp.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://msp.yj202588.top

C#:   s.Replace("a", "b")
来源：http://viu.bbcook.cn

[E07] 按分隔符拆分
来源：http://bmo.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wgq.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wql.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://eqg.sjlbkw.cn

TS:   s.split(",")
来源：http://koo.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://xab.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ein.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://dan.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vsc.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://cjq.zhoulong.xyz

Py:   ",".join(items)
来源：http://tlr.havefunace.top

PHP:  implode(",", $items);
来源：http://wga.daria6918.cn

JS:   items.join(",")
来源：http://hit.xuetiantiany.cn

TS:   items.join(",")
来源：http://ltk.vqdsnc.cn

Java: String.join(",", items)
来源：http://lct.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://dfi.pycfn.com

Ruby: items.join(",")
来源：http://hcp.yuanzhike.top

C#:   string.Join(",", items)
来源：http://qzz.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://nme.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldb.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vkc.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://vjr.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://edo.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://bvf.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfw.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://ykl.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvi.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://ikt.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgd.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vle.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://rhg.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://ynh.cucudq.cn

Java: String.format("%03d", 7)
来源：http://sgi.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://clx.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jlf.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://chg.vqdsnc.cn

[E11] 反转字符串
来源：http://vou.nwbrower.top

Py:   s[::-1]
来源：http://fxa.xziqi.cn

PHP:  strrev($s);
来源：http://yac.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://axx.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ugc.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mar.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gds.daxiang520.top

Ruby: s.reverse
来源：http://xaa.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://qoc.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://vsm.pengpengdd.cyou

Py:   s.count("a")
来源：http://mck.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://ceb.fktsv.cn

JS:   s.split("a").length - 1
来源：http://sxk.smart0.xyz

TS:   s.split("a").length - 1
来源：http://rsh.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://flo.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://znj.tianlin.xyz

Ruby: s.count("a")
来源：http://zxm.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://ncx.shuidangran.top

[E13] 逐字符遍历
来源：http://czj.meibo888.top

Py:   for ch in s: print(ch)
来源：http://mwc.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ult.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rma.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yey.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hlz.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qom.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sad.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ghv.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://qcr.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fsp.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hpj.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cxe.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://khu.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igv.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xwm.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://miq.shanyushiyangtech.top


<!-- 参考信息 -->