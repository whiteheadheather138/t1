代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://jex.zhijiandao.cn

TS:   [...a, ...b];
来源：http://bcz.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://llf.sufxvd.cn

Go:   append(a, b...)
来源：http://lsj.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://bqv.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://lwz.gzhubu.top

[D09] 排序（升序）
来源：http://jis.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://lkc.jiagoushi.top

PHP:  sort($arr);
来源：http://bik.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lgx.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oyq.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://chx.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cel.52xcode.cn

Ruby: arr.sort
来源：http://yrd.daria6918.cn

C#:   list.Sort();
来源：http://kjo.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xob.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uab.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qvc.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmw.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwn.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jyi.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ouf.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hel.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ykx.guannengcc.top

[D11] 反转数组
来源：http://fsl.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nem.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://cmx.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phz.ydzc1.top

TS:   [...arr].reverse();
来源：http://lex.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://lue.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://rcq.xuetiantiany.cn

Ruby: arr.reverse
来源：http://bai.quarkkingdee.top

C#:   list.Reverse();
来源：http://xqm.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://ifp.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://enb.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://smq.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cxc.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bye.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hom.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://nmo.zdqjudy.top

Ruby: arr.index(x)
来源：http://fwv.ybcxt.top

C#:   list.IndexOf(x);
来源：http://zad.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://bya.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uya.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbc.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://gio.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://mma.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://spv.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fzs.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ecx.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://apd.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://fko.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lsi.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzh.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://klc.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://ddb.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rsi.zdqjudy.top

Go:   // 手写循环
来源：http://fte.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://hig.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tcs.ivvv.top

[D15] 去重
来源：http://mwg.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eas.haohaochexian.top

PHP:  array_unique($arr);
来源：http://qgi.hcnkem.com

JS:   [...new Set(arr)]
来源：http://yux.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://owx.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cju.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lsi.hongshengwenyu.top

Ruby: arr.uniq
来源：http://srg.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://exk.feifeiyinyue.top

[D16] 求和与平均值
来源：http://ifv.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://daa.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://quw.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cys.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://czg.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://euk.ivvv.top

Go:   // 手写循环累加
来源：http://mgc.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wlu.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://mzv.yfazqb.com

[D17] 最大值与最小值
来源：http://gha.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://avw.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://tqs.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ove.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://wcs.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lod.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://grp.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://bxr.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://cdn.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://djh.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iri.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://gct.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hmh.tian-w.cn

TS:   nested.flat();
来源：http://sec.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://raq.chenlongwang.top

Go:   // 手写双层循环
来源：http://kti.52xcode.cn

Ruby: nested.flatten
来源：http://kkb.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kts.aizwys.cn

[D19] 按字段分组
来源：http://hak.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zdj.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bxo.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ycs.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zpv.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://goe.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://dlx.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://may.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vwy.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://feg.yj202588.top

Py:   Counter(arr)
来源：http://ztz.shuidangran.top

PHP:  array_count_values($arr);
来源：http://mgh.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xbc.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrb.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tnn.jianghu66.top

Go:   // 手写 map[T]int
来源：http://aaw.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://shq.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yss.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://ewb.aibaodan.cn

Py:   x in arr
来源：http://teb.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://ejh.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://hgf.ivvv.top

TS:   arr.includes(x)
来源：http://day.quarkkingdee.top

Java: list.contains(x)
来源：http://hya.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://fox.hfpthk.cn

Ruby: arr.include?(x)
来源：http://kvp.yangfankeji.com

C#:   list.Contains(x)
来源：http://qqu.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://muk.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tcq.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jni.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://znb.vqdsnc.cn

TS:   [...arr];
来源：http://ckh.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://lfb.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://aum.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://hlx.xylfe.cn

C#:   new List<int>(list);
来源：http://vsp.fktsv.cn

[D23] reduce 累积计算
来源：http://zwk.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tmp.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wpx.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idu.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bou.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://laf.aibaodan.cn

Go:   // 手写循环
来源：http://qxu.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pra.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ksm.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://xpk.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gfw.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vhk.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://epc.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptg.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nbw.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lah.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rdb.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://exy.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://dcu.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kzh.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://usg.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rbm.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axn.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ggx.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xyl.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ljw.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rgm.cashguo.top

[D26] 数组转字符串
来源：http://kor.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://yyk.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://mws.jinqigfzy.top

JS:   arr.join(", ")
来源：http://mba.havefunace.top

TS:   arr.join(", ")
来源：http://pbn.svipenyu.cn

Java: String.join(", ", list)
来源：http://izp.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://fmw.xziqi.cn

Ruby: arr.join(", ")
来源：http://qxq.yj202588.top

C#:   string.Join(", ", list)
来源：http://nks.jlsjyb.cn

================================================================================
来源：http://abs.dianchejie.cn

E. 字符串处理
来源：http://qmz.gaohongyu789.top

================================================================================
来源：http://szq.zhongyouzk.top

[E01] 拼接字符串
来源：http://skl.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zru.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qnk.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfv.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lla.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fpw.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fut.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uxb.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wuj.zhixingplan.top

[E02] 重复字符串
来源：http://jyf.nanxuanxn.top

Py:   "ab" * 3
来源：http://tox.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://qxr.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://zqf.meibo888.top

TS:   "ab".repeat(3)
来源：http://tiu.hcnkem.com

Java: "ab".repeat(3)
来源：http://uox.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zyy.sjlbkw.cn

Ruby: "ab" * 3
来源：http://jwf.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oid.hcnkem.com

[E03] 截取子串
来源：http://pmm.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mmd.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://phh.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://thg.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://wlp.gogol.net.cn

Java: s.substring(1, 4)
来源：http://jxx.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://squ.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rzd.yongpay.top

C#:   s.Substring(1, 3)
来源：http://slr.316326.xyz

[E04] 查找子串位置
来源：http://ivq.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://lri.316326.xyz

PHP:  strpos($s, "x");
来源：http://djo.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://din.zhixingplan.top

TS:   s.indexOf("x")
来源：http://pcm.hammf.cn

Java: s.indexOf("x")
来源：http://nhe.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://cug.52xcode.cn

Ruby: s.index("x")
来源：http://tzp.ydzc1.top

C#:   s.IndexOf("x")
来源：http://zmz.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jdr.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ept.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bxx.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywr.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://yeo.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lvo.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://inu.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vsl.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pqr.hnxiangtu.top

[E06] 替换子串
来源：http://bmo.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cyg.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://hsz.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lly.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://poa.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zdw.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aay.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mhw.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://qba.guowangkeji.top

[E07] 按分隔符拆分
来源：http://brn.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bll.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://djx.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qnc.jqgufenzy.top

TS:   s.split(",")
来源：http://qgw.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jxi.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vak.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://kmd.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zpb.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://vos.shzxlz.cn

Py:   ",".join(items)
来源：http://vdb.bbcook.cn

PHP:  implode(",", $items);
来源：http://olx.cucudq.cn

JS:   items.join(",")
来源：http://leb.jinghuilouyu.cn

TS:   items.join(",")
来源：http://ide.jlsjyb.cn

Java: String.join(",", items)
来源：http://qhp.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://mza.xylfe.cn

Ruby: items.join(",")
来源：http://kls.ppjwa.cn

C#:   string.Join(",", items)
来源：http://hhr.jiagoushi.top

[E09] 去除所有空白字符
来源：http://anq.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pxx.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uxw.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://anf.jianghu66.top

TS:   s.replace(/\s+/g, "")
来源：http://wsj.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://mts.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qoc.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://gew.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fww.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://uln.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nxe.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ily.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://agx.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://okd.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://uey.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ykk.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://okd.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxw.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://pjk.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://hby.sxryk.cn

PHP:  strrev($s);
来源：http://vpq.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://jzf.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://nhl.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hfn.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sug.bbcook.cn

Ruby: s.reverse
来源：http://hzk.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zjb.fktsv.cn

[E12] 统计某字符出现次数
来源：http://mcx.zhengqikj.top

Py:   s.count("a")
来源：http://yzr.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://slo.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://gmj.ydzc1.top

TS:   s.split("a").length - 1
来源：http://evi.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dqh.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://nad.hnxiangtu.top

Ruby: s.count("a")
来源：http://wnq.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://lve.hammf.cn

[E13] 逐字符遍历
来源：http://gvu.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://gxd.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rht.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yzo.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ztq.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kbh.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qej.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ofm.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iqw.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://mqj.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sai.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://suy.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uwu.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://alk.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uzh.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://knx.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xdd.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bjo.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://nrx.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gto.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uxj.yuxming.cn


<!-- 参考信息 -->