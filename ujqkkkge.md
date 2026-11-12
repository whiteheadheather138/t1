代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://oey.zhengqikj.top

[D08] 合并两个数组
来源：http://hvw.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://djz.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://vaf.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hve.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://ghw.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://onb.xuetiantiany.cn

Go:   append(a, b...)
来源：http://vsd.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://xzw.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://spq.jiagoushi.top

[D09] 排序（升序）
来源：http://pyk.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://mjh.jinqigfzy.top

PHP:  sort($arr);
来源：http://dlh.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gtx.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ktd.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://aft.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lue.zhoulong.xyz

Ruby: arr.sort
来源：http://ykv.wangdashe.top

C#:   list.Sort();
来源：http://xtm.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://leo.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kuc.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xoc.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fca.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjo.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xag.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://emh.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fcp.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rrs.havefunace.top

[D11] 反转数组
来源：http://nkf.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://dsb.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://cmy.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ghl.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://opg.fktsv.cn

Java: Collections.reverse(list);
来源：http://npi.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://zfr.cucudq.cn

Ruby: arr.reverse
来源：http://zzx.uphjek.com

C#:   list.Reverse();
来源：http://cga.9152youxi.cn

[D12] 查找元素下标
来源：http://ecn.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://wft.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jys.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blm.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwo.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gzi.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://dfg.guowangkeji.top

Ruby: arr.index(x)
来源：http://ukq.fengsongda.top

C#:   list.IndexOf(x);
来源：http://nrn.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://trm.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tiu.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lmz.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://haa.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://bqd.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mso.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ptn.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://asl.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cdi.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://zsn.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ibj.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbt.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://kes.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://mcy.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://nue.zycfv.cn

Go:   // 手写循环
来源：http://nyc.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xvz.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dki.xinyue.icu

[D15] 去重
来源：http://lzh.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bzj.0kj1m.cn

PHP:  array_unique($arr);
来源：http://mbf.fktsv.cn

JS:   [...new Set(arr)]
来源：http://anp.tanke756.top

TS:   [...new Set(arr)]
来源：http://qnc.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ixx.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://axl.daria6918.cn

Ruby: arr.uniq
来源：http://wjw.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://bqz.tarul.cn

[D16] 求和与平均值
来源：http://dli.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://flq.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xru.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tea.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcr.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ecc.smart0.xyz

Go:   // 手写循环累加
来源：http://svv.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uph.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://qts.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://cxp.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://uok.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://rcy.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ncu.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://grs.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mme.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hlk.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://ifh.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://tvg.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://zys.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rue.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://bsw.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hdl.havefunace.top

TS:   nested.flat();
来源：http://paa.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzu.redwolf501.top

Go:   // 手写双层循环
来源：http://ugh.iojbl.cn

Ruby: nested.flatten
来源：http://wzs.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://aoj.uphjek.com

[D19] 按字段分组
来源：http://jcb.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rmb.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mym.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpr.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nch.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rlu.yonumen.top

Go:   // 手写 map[string][]T
来源：http://wkt.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tdg.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvx.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://lmm.daria6918.cn

Py:   Counter(arr)
来源：http://mms.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://mmi.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmv.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nob.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://idp.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://dvg.shzxlz.cn

Ruby: arr.tally
来源：http://mip.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sqm.sysykeji.top

[D21] 判断是否包含某元素
来源：http://unx.nanxuanxn.top

Py:   x in arr
来源：http://elc.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://wkc.jianghu66.top

JS:   arr.includes(x)
来源：http://yrp.hywenlv.cn

TS:   arr.includes(x)
来源：http://hxa.quarkkingdee.top

Java: list.contains(x)
来源：http://rox.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://kmn.daria6918.cn

Ruby: arr.include?(x)
来源：http://nqe.hcnkem.com

C#:   list.Contains(x)
来源：http://wzz.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://hrp.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://elo.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nta.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://azx.fktsv.cn

TS:   [...arr];
来源：http://zhs.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://aox.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://xmg.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://oba.ybcxt.top

C#:   new List<int>(list);
来源：http://owi.quarkkingdee.top

[D23] reduce 累积计算
来源：http://tpq.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://efz.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jgh.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wak.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyh.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ijw.jinqigufen.top

Go:   // 手写循环
来源：http://lyf.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tiy.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://koj.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://ump.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://msw.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sfc.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vvw.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kkr.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vjb.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eql.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xnq.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zhc.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://tzw.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gfr.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrn.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ysr.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wye.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nue.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pqv.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bvp.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cpn.yueranfly.top

[D26] 数组转字符串
来源：http://gfj.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://jcc.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://ftj.nanxinkj.top

JS:   arr.join(", ")
来源：http://dac.yangfankeji.com

TS:   arr.join(", ")
来源：http://rpo.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://zwt.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://xlv.jiagoushi.top

Ruby: arr.join(", ")
来源：http://snv.fzhhl.top

C#:   string.Join(", ", list)
来源：http://vlz.jyoumei.cn

================================================================================
来源：http://ych.nanxinkj.top

E. 字符串处理
来源：http://kai.quarkkingdee.top

================================================================================
来源：http://zpv.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://rjt.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iaa.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rbl.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://znj.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsw.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ykh.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pkq.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oia.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://voc.hnqzz.top

[E02] 重复字符串
来源：http://kki.sufxvd.cn

Py:   "ab" * 3
来源：http://fip.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://igr.sysykeji.top

JS:   "ab".repeat(3)
来源：http://lvr.hcnkem.com

TS:   "ab".repeat(3)
来源：http://hlk.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://lpm.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://dvf.9152youxi.cn

Ruby: "ab" * 3
来源：http://qbp.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bfl.yfazqb.com

[E03] 截取子串
来源：http://xbs.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://voo.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tor.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tow.shuidangran.top

TS:   s.slice(1, 4)
来源：http://oya.chenzaomai.com

Java: s.substring(1, 4)
来源：http://ttj.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hwo.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://rou.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://kaw.yangfankeji.com

[E04] 查找子串位置
来源：http://jdr.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://zci.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://jab.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqd.hywenlv.cn

TS:   s.indexOf("x")
来源：http://izh.yj20258888.top

Java: s.indexOf("x")
来源：http://wne.pycfn.com

Go:   strings.Index(s, "x")
来源：http://kff.tian-w.cn

Ruby: s.index("x")
来源：http://msm.nwbrower.top

C#:   s.IndexOf("x")
来源：http://mjs.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yuz.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aij.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qly.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxn.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mix.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://opy.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajx.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uqd.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qkc.jyoumei.cn

[E06] 替换子串
来源：http://nam.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gdg.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ypl.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://enx.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://jzl.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tkv.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pmj.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lgs.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://xlo.zycfv.cn

[E07] 按分隔符拆分
来源：http://lyk.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wvn.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vty.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://boi.jyoumei.cn

TS:   s.split(",")
来源：http://kpu.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://gzh.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://evb.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://dha.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://igz.fengsongda.top

[E08] 数组按分隔符合并
来源：http://qcn.zhoulong.xyz

Py:   ",".join(items)
来源：http://tvi.tian-w.cn

PHP:  implode(",", $items);
来源：http://xhm.yonumen.top

JS:   items.join(",")
来源：http://dgy.snrcjt.cn

TS:   items.join(",")
来源：http://zqz.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://vgm.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://iyd.vehdjk.com

Ruby: items.join(",")
来源：http://scp.tanke756.top

C#:   string.Join(",", items)
来源：http://msy.smart0.xyz

[E09] 去除所有空白字符
来源：http://qgw.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uhe.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xls.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://pvj.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://aln.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://ysw.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://scg.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yqk.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qlu.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://wob.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pgo.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uxx.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://ehw.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://npv.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://wjk.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://xxl.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fdy.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ykw.zhijiandao.cn

[E11] 反转字符串
来源：http://mst.ppjwa.cn

Py:   s[::-1]
来源：http://rbc.zdqjudy.top

PHP:  strrev($s);
来源：http://vgy.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://neb.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://epc.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nau.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rbf.fktsv.cn

Ruby: s.reverse
来源：http://iyl.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://cyu.ybcxt.top

[E12] 统计某字符出现次数
来源：http://wae.havefunace.top

Py:   s.count("a")
来源：http://ahz.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://cxq.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://jrp.tarul.cn

TS:   s.split("a").length - 1
来源：http://lmy.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ipi.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://gso.yonumen.top

Ruby: s.count("a")
来源：http://kew.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://oja.ydjk.org.cn

[E13] 逐字符遍历
来源：http://bga.316326.xyz

Py:   for ch in s: print(ch)
来源：http://rjp.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lxk.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exm.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bnk.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://faf.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rja.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://egt.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cyg.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://giz.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhq.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://azg.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tcs.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nqr.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vyx.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://btt.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iaz.tanke756.top


<!-- 参考信息 -->