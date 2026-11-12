代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mmg.hnqzz.top

TS:   [...a, ...b];
来源：http://nyb.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aok.gotoacloud.top

Go:   append(a, b...)
来源：http://zuj.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://hwo.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://ecc.chenzaomai.com

[D09] 排序（升序）
来源：http://vbh.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://csd.zhoulong.xyz

PHP:  sort($arr);
来源：http://obj.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ugq.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://nkm.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zen.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ihk.guannengcc.top

Ruby: arr.sort
来源：http://qcl.guowangkeji.top

C#:   list.Sort();
来源：http://otb.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dmb.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tlz.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jch.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://imd.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vng.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jfr.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kjp.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zqb.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vid.vqdsnc.cn

[D11] 反转数组
来源：http://rbe.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ioe.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://tsm.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sjh.meibo888.top

TS:   [...arr].reverse();
来源：http://gtm.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://rtp.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://kcb.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://nli.mhx1999.top

C#:   list.Reverse();
来源：http://wow.nanxinkj.top

[D12] 查找元素下标
来源：http://qer.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://vtg.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qpb.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wob.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mhx.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ruz.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://yis.316326.xyz

Ruby: arr.index(x)
来源：http://pyv.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://mag.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://cxq.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fbu.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tpn.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://uxl.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://edh.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyn.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mjb.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://ddf.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://koq.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://okl.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vks.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tqh.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://vos.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://jjv.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://kpm.jinghuilouyu.cn

Go:   // 手写循环
来源：http://efr.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ifp.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ujl.chenjidiqi.icu

[D15] 去重
来源：http://reu.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nnb.zdqjudy.top

PHP:  array_unique($arr);
来源：http://dwt.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://dsx.sxryk.cn

TS:   [...new Set(arr)]
来源：http://scv.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mcz.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://irz.zhengqikj.top

Ruby: arr.uniq
来源：http://acl.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://vyb.guannengcc.top

[D16] 求和与平均值
来源：http://jpo.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://boj.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uvv.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://umg.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydm.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://net.zdqjudy.top

Go:   // 手写循环累加
来源：http://lqw.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://duz.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://zmk.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://gel.meibo888.top

Py:   max(arr);  min(arr)
来源：http://okv.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://hht.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xyv.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://fxn.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lej.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ttg.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://cjn.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://teb.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://wwn.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vsv.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://agi.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yve.kuanghao11.cn

TS:   nested.flat();
来源：http://nat.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cem.cheryme.top

Go:   // 手写双层循环
来源：http://vij.zdqjudy.top

Ruby: nested.flatten
来源：http://rnm.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xkr.quarkkingdee.top

[D19] 按字段分组
来源：http://jrg.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ins.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bkb.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nxe.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gqp.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mzp.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://gnr.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tmu.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://def.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://xab.dashuyun.cn

Py:   Counter(arr)
来源：http://eyp.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://vzr.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mda.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zlu.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ajw.ybcxt.top

Go:   // 手写 map[T]int
来源：http://mbx.zycfv.cn

Ruby: arr.tally
来源：http://eyp.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jua.hesvh.cn

[D21] 判断是否包含某元素
来源：http://ssp.shzxlz.cn

Py:   x in arr
来源：http://aya.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://qyd.dianchejie.cn

JS:   arr.includes(x)
来源：http://vzz.shzxlz.cn

TS:   arr.includes(x)
来源：http://xrk.yueranfly.top

Java: list.contains(x)
来源：http://lgg.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://qay.birdmap.top

Ruby: arr.include?(x)
来源：http://kov.quarkkingdee.top

C#:   list.Contains(x)
来源：http://lbr.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://gpo.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yjq.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gzw.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://skm.sufxvd.cn

TS:   [...arr];
来源：http://ukw.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://gqj.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jfr.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://ojq.aizwys.cn

C#:   new List<int>(list);
来源：http://jpo.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://xeo.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nns.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yfk.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qox.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfi.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gnc.daxiang520.top

Go:   // 手写循环
来源：http://ivf.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hfb.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oqi.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://qbj.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uql.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwc.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nnq.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hka.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wfj.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fik.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tzn.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tgj.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://kzr.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://asw.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jnx.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xit.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nzo.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ami.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iva.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cym.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://onw.yj20258888.top

[D26] 数组转字符串
来源：http://gxa.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://psk.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://tez.yonumen.top

JS:   arr.join(", ")
来源：http://the.fehbvm.com

TS:   arr.join(", ")
来源：http://imb.aibaodan.cn

Java: String.join(", ", list)
来源：http://ivq.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://xkf.vehdjk.com

Ruby: arr.join(", ")
来源：http://hnu.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://dse.zhiwuduotai.top

================================================================================
来源：http://nms.gogol.net.cn

E. 字符串处理
来源：http://ivm.zhongyouzk.top

================================================================================
来源：http://lfu.jyoumei.cn

[E01] 拼接字符串
来源：http://byr.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gii.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eka.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hrk.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvs.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzv.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://drn.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ijd.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gyu.yj20258.top

[E02] 重复字符串
来源：http://kjl.dashuyun.cn

Py:   "ab" * 3
来源：http://nwb.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://act.cashguo.top

JS:   "ab".repeat(3)
来源：http://lkz.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://vxj.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://sfz.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://lbk.yvedp.cn

Ruby: "ab" * 3
来源：http://qub.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ecd.dianchejie.cn

[E03] 截取子串
来源：http://vuf.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jll.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qaz.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvw.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://cwk.jiagoushi.top

Java: s.substring(1, 4)
来源：http://tma.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oya.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jej.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://bdr.hywenlv.cn

[E04] 查找子串位置
来源：http://bld.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://goj.smart0.xyz

PHP:  strpos($s, "x");
来源：http://oxc.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rlc.hesvh.cn

TS:   s.indexOf("x")
来源：http://bzv.xuanzx.com

Java: s.indexOf("x")
来源：http://ime.havefunace.top

Go:   strings.Index(s, "x")
来源：http://gaf.quarkkingdee.top

Ruby: s.index("x")
来源：http://tqi.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://vod.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cej.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gzs.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pol.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhc.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wia.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oam.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oac.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lnq.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ehu.wangshuangyany.cn

[E06] 替换子串
来源：http://stx.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mor.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://cnn.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ttd.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://nqu.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovm.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://abo.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xbe.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://jcw.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://gge.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ite.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vlk.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aob.shuidangran.top

TS:   s.split(",")
来源：http://bus.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gxs.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lnp.tarul.cn

Ruby: s.split(",");  s.split
来源：http://ond.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wio.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://itm.ybcxt.top

Py:   ",".join(items)
来源：http://zdg.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://yqe.jlsjyb.cn

JS:   items.join(",")
来源：http://iyh.zhixingplan.top

TS:   items.join(",")
来源：http://nzw.xinyue.icu

Java: String.join(",", items)
来源：http://qwp.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://sbe.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://avr.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://pcu.fengsongda.top

[E09] 去除所有空白字符
来源：http://kxp.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bae.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rjr.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://nle.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://ljp.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xmj.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vkf.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://qrv.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lnk.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://jzh.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ans.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mfo.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://fww.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://jej.yuxming.cn

Java: String.format("%03d", 7)
来源：http://ffk.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://izq.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oop.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://noe.zhongyouzk.top

[E11] 反转字符串
来源：http://dtj.zhengqikj.top

Py:   s[::-1]
来源：http://edl.jyoumei.cn

PHP:  strrev($s);
来源：http://vad.tanke756.top

JS:   [...s].reverse().join("")
来源：http://bok.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://tdm.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zkw.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uxe.zhoulong.xyz

Ruby: s.reverse
来源：http://xhy.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://wav.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://zod.tanke756.top

Py:   s.count("a")
来源：http://tlb.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://wrj.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://uyb.yfazqb.com

TS:   s.split("a").length - 1
来源：http://vih.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://urv.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://rjl.hfpthk.cn

Ruby: s.count("a")
来源：http://stw.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://rjj.cheryme.top

[E13] 逐字符遍历
来源：http://mbj.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://bfp.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aio.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wib.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://baw.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fvk.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nxz.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gcr.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xmw.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://qdr.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcp.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://npz.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hwn.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aym.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ltx.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bgs.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://djd.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pku.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://mgo.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hld.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rea.jlsjyb.cn


<!-- 参考信息 -->