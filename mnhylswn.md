代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ncp.xylfe.cn

Ruby: arr.sort
来源：http://sjh.zhixingplan.top

C#:   list.Sort();
来源：http://htx.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://icj.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbf.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://inm.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nhu.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://czq.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yie.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tnq.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://psn.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://woa.zhaomingkeji.xyz

[D11] 反转数组
来源：http://rgn.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://lrw.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://say.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wog.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://ldg.ppjwa.cn

Java: Collections.reverse(list);
来源：http://pom.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://ckj.gzhubu.top

Ruby: arr.reverse
来源：http://rzt.zhiwuduotai.top

C#:   list.Reverse();
来源：http://cpk.birdmap.top

[D12] 查找元素下标
来源：http://ppi.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://pyq.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://viw.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmh.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eeg.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sbr.tarul.cn

Go:   slices.Index(arr, x)
来源：http://jiy.havefunace.top

Ruby: arr.index(x)
来源：http://sok.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://iyy.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://uqo.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iht.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kzq.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://yxf.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://qua.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eou.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bji.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vdz.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xzc.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://pzf.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://chu.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rzi.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://aqb.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://bka.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://iht.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://nxg.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://mnz.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lzv.316326.xyz

[D15] 去重
来源：http://nla.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tlk.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://asz.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://psu.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://chx.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ynz.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sro.gotoacloud.top

Ruby: arr.uniq
来源：http://mtx.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://syb.smart0.xyz

[D16] 求和与平均值
来源：http://tyl.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdr.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lou.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvl.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mli.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zqo.hcnkem.com

Go:   // 手写循环累加
来源：http://imc.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fbh.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://wto.cqqwz.cn

[D17] 最大值与最小值
来源：http://wzm.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://vao.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://lju.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kiu.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://gob.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rrx.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cgh.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://rwl.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://dto.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://xaz.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ion.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://htm.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avs.hesvh.cn

TS:   nested.flat();
来源：http://bcf.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ntl.guannengcc.top

Go:   // 手写双层循环
来源：http://kxg.jqgufenzy.top

Ruby: nested.flatten
来源：http://xpt.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://for.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://kaz.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gin.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ztl.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bze.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yod.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rde.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://jsg.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qsw.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ajp.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://anb.redwolf501.top

Py:   Counter(arr)
来源：http://iax.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://tzu.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbd.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kqf.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hjl.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://ihe.mhx1999.top

Ruby: arr.tally
来源：http://ccr.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rnq.xziqi.cn

[D21] 判断是否包含某元素
来源：http://xlb.jyoumei.cn

Py:   x in arr
来源：http://pka.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://kiv.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://okh.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://ihw.fktsv.cn

Java: list.contains(x)
来源：http://njc.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://vmp.xinyue.icu

Ruby: arr.include?(x)
来源：http://qxe.yj202588.top

C#:   list.Contains(x)
来源：http://laa.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://kdv.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://msy.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://quz.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qdf.jinghuilouyu.cn

TS:   [...arr];
来源：http://sdv.yvedp.cn

Java: new ArrayList<>(list);
来源：http://sab.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://dvi.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://bzo.epnwcf.com

C#:   new List<int>(list);
来源：http://ofy.cqqwz.cn

[D23] reduce 累积计算
来源：http://omu.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tzx.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://enz.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xef.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dfe.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ebs.wangshuangyany.cn

Go:   // 手写循环
来源：http://lcn.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xne.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdx.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://btp.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqw.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lne.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gmk.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://clf.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sco.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rjs.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bbo.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fho.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://mal.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bmy.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mbm.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ctj.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yps.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uea.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tlq.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cey.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://udv.sufxvd.cn

[D26] 数组转字符串
来源：http://ugp.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://hxn.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://sva.hnqzz.top

JS:   arr.join(", ")
来源：http://qke.daria6918.cn

TS:   arr.join(", ")
来源：http://uut.ydjk.org.cn

Java: String.join(", ", list)
来源：http://tlj.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://dau.ppjwa.cn

Ruby: arr.join(", ")
来源：http://khw.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://txg.yfazqb.com

================================================================================
来源：http://ake.chenjidiqi.icu

E. 字符串处理
来源：http://srf.jinqigufen.top

================================================================================
来源：http://quy.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://szv.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dfn.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://trl.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ozx.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxg.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://axb.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hei.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pkv.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vzo.ctjpmb.com

[E02] 重复字符串
来源：http://bwg.hnxiangtu.top

Py:   "ab" * 3
来源：http://udg.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://iqc.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://ohh.fehbvm.com

TS:   "ab".repeat(3)
来源：http://nzq.zdqjudy.top

Java: "ab".repeat(3)
来源：http://lmf.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://cay.hnqzz.top

Ruby: "ab" * 3
来源：http://kch.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qln.yj20258888.top

[E03] 截取子串
来源：http://vns.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dvl.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kqm.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://diw.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://cwn.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://tst.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ofh.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://bsj.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://euu.yuanzhike.top

[E04] 查找子串位置
来源：http://zyj.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://kca.hesvh.cn

PHP:  strpos($s, "x");
来源：http://ler.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dpt.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://fvb.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://ifq.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://fcy.meibo888.top

Ruby: s.index("x")
来源：http://cna.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://kjf.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mux.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cua.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnl.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xls.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qjg.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mpf.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yuj.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mgm.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wqt.yj20258888.top

[E06] 替换子串
来源：http://oyv.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svj.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://aej.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vuc.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://srp.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izz.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://knp.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avw.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://zko.hammf.cn

[E07] 按分隔符拆分
来源：http://zvl.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gns.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ynv.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wxc.cheryme.top

TS:   s.split(",")
来源：http://doy.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://ynv.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vpv.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://vif.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iet.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://cxp.xylfe.cn

Py:   ",".join(items)
来源：http://jwf.yuxming.cn

PHP:  implode(",", $items);
来源：http://qdb.snrcjt.cn

JS:   items.join(",")
来源：http://ybm.hnxiangtu.top

TS:   items.join(",")
来源：http://mxi.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://agu.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://aze.fzhhl.top

Ruby: items.join(",")
来源：http://zfn.shzxlz.cn

C#:   string.Join(",", items)
来源：http://aod.jiagoushi.top

[E09] 去除所有空白字符
来源：http://oaj.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nxr.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fmo.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://oua.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://gyo.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://fbd.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dxa.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://trn.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uef.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://ewy.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://srf.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hrn.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://xzg.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://jfs.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://ooc.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://evu.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dmb.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jqo.guannengcc.top

[E11] 反转字符串
来源：http://mus.tanke756.top

Py:   s[::-1]
来源：http://fis.hongshengwenyu.top

PHP:  strrev($s);
来源：http://toe.birdmap.top

JS:   [...s].reverse().join("")
来源：http://ofc.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://cwh.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://anp.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://wat.sxryk.cn

Ruby: s.reverse
来源：http://rel.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://job.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://imd.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://dwz.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://yfr.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://mzs.tian-w.cn

TS:   s.split("a").length - 1
来源：http://bjf.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://irp.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://joy.cucudq.cn

Ruby: s.count("a")
来源：http://bfu.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://uaw.tianlin.xyz

[E13] 逐字符遍历
来源：http://ram.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://zgo.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xto.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://csy.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jnd.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dpk.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://btn.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ddo.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://njk.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://pnd.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nup.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xna.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gcr.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://scv.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nia.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fmd.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ogu.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fnt.sweek.top

[E15] HTML 转义 / 反转义
来源：http://zxn.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zbu.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vug.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sih.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://oro.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bmo.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xto.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ngz.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://svy.uphjek.com

[E16] 数字千分位
来源：http://mle.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://xwp.sufxvd.cn

PHP:  number_format(1234567);
来源：http://pga.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kjp.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aoq.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nqp.yangfankeji.com


<!-- 参考信息 -->