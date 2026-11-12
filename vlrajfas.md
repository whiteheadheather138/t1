代发 wailian999

PHP:  sort($arr);
来源：http://tfd.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qro.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mdj.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmb.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pij.shzxlz.cn

Ruby: arr.sort
来源：http://ydb.wangdashe.top

C#:   list.Sort();
来源：http://qwm.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://twy.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://axg.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dln.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yuu.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tvh.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yev.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fui.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bey.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vtu.fehbvm.com

[D11] 反转数组
来源：http://gvs.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://obd.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://olb.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wgs.gotoacloud.top

TS:   [...arr].reverse();
来源：http://lcf.jianghu66.top

Java: Collections.reverse(list);
来源：http://ssd.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://vem.xylfe.cn

Ruby: arr.reverse
来源：http://rno.cheryme.top

C#:   list.Reverse();
来源：http://mgd.gaohongyu789.top

[D12] 查找元素下标
来源：http://xwq.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://jwt.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fbk.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pnw.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sjh.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qkw.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://lwf.sweek.top

Ruby: arr.index(x)
来源：http://ang.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://iar.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://fsu.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fde.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zdd.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://hst.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://mip.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nvb.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://soj.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://app.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xvf.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://egx.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xce.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://huj.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://pvv.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://ets.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://pdb.zycfv.cn

Go:   // 手写循环
来源：http://zey.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://emj.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qrg.yuxming.cn

[D15] 去重
来源：http://cst.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lbh.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://uat.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://knt.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://ioi.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yeu.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vhy.jiagoushi.top

Ruby: arr.uniq
来源：http://uyx.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://cpc.uphjek.com

[D16] 求和与平均值
来源：http://nmn.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://chc.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ivs.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwz.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eer.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gbf.cheryme.top

Go:   // 手写循环累加
来源：http://mow.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cgq.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://bsk.sweek.top

[D17] 最大值与最小值
来源：http://pvk.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://ffr.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://uek.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vai.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://lhe.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xjf.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qda.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://dua.birdmap.top

C#:   list.Max();  list.Min()
来源：http://nap.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://xfo.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cpx.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://eqe.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zfm.wangshuangyany.cn

TS:   nested.flat();
来源：http://fct.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ssl.zhixingplan.top

Go:   // 手写双层循环
来源：http://beh.xinyue.icu

Ruby: nested.flatten
来源：http://xld.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dcm.fehbvm.com

[D19] 按字段分组
来源：http://vtj.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmt.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mup.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kam.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ggj.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://twf.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://nxs.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://igv.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://thg.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://odo.jqgfzy.top

Py:   Counter(arr)
来源：http://dpt.mhx1999.top

PHP:  array_count_values($arr);
来源：http://bid.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pza.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lql.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gcn.tian-w.cn

Go:   // 手写 map[T]int
来源：http://gjn.cucudq.cn

Ruby: arr.tally
来源：http://tgu.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hba.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://vjc.daxiang520.top

Py:   x in arr
来源：http://juk.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://sqo.redwolf501.top

JS:   arr.includes(x)
来源：http://vry.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://vjy.xziqi.cn

Java: list.contains(x)
来源：http://nqc.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://bnp.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://jau.tianlin.xyz

C#:   list.Contains(x)
来源：http://ofv.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://yyu.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oyp.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://idb.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mol.xuanzx.com

TS:   [...arr];
来源：http://abw.gzhubu.top

Java: new ArrayList<>(list);
来源：http://tht.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sgl.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://yrh.tian-w.cn

C#:   new List<int>(list);
来源：http://pkr.cdnleiting.top

[D23] reduce 累积计算
来源：http://bgz.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zbv.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wzv.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pak.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nqx.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxa.kuanghao11.cn

Go:   // 手写循环
来源：http://arr.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gfl.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://itg.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://tuv.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyz.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kqf.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pac.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lhr.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://epf.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ibk.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://str.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ahk.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://zzq.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gcm.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wyx.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://law.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggf.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fwh.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tqe.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wuo.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqc.sweek.top

[D26] 数组转字符串
来源：http://dxe.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://rmq.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://usn.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://xvh.mhx1999.top

TS:   arr.join(", ")
来源：http://zci.shzxlz.cn

Java: String.join(", ", list)
来源：http://gjm.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://boc.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://ahh.yueranfly.top

C#:   string.Join(", ", list)
来源：http://ilm.0kj1m.cn

================================================================================
来源：http://clw.birdmap.top

E. 字符串处理
来源：http://ovj.hcnkem.com

================================================================================
来源：http://cel.havefunace.top

[E01] 拼接字符串
来源：http://fuy.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://men.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iyo.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kte.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nci.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gam.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ieu.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://phb.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aui.tanke756.top

[E02] 重复字符串
来源：http://rhv.ydzc1.top

Py:   "ab" * 3
来源：http://abd.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://pjz.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://cup.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://ywy.redwolf501.top

Java: "ab".repeat(3)
来源：http://kxn.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://euo.ehwqpu.com

Ruby: "ab" * 3
来源：http://kno.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nrp.havefunace.top

[E03] 截取子串
来源：http://une.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgg.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://orr.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bmu.tarul.cn

TS:   s.slice(1, 4)
来源：http://mfu.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://vgv.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gah.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lnz.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://uww.kuanghao11.cn

[E04] 查找子串位置
来源：http://ssg.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://jdr.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://mwy.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://faa.fzhhl.top

TS:   s.indexOf("x")
来源：http://sxw.fzhhl.top

Java: s.indexOf("x")
来源：http://rbm.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://qsw.yongpay.top

Ruby: s.index("x")
来源：http://pes.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://hdo.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opd.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://abv.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vse.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yce.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uhf.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ahf.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://het.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hes.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ukg.redwolf501.top

[E06] 替换子串
来源：http://vmw.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xxk.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://cjs.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fed.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://dgo.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zog.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yvs.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vvb.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://nml.xinyue.icu

[E07] 按分隔符拆分
来源：http://cod.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://efg.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bnm.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xoe.yj20258888.top

TS:   s.split(",")
来源：http://sil.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://nvo.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwo.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://xki.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qqv.havefunace.top

[E08] 数组按分隔符合并
来源：http://nav.cdnleiting.top

Py:   ",".join(items)
来源：http://lnk.gotoacloud.top

PHP:  implode(",", $items);
来源：http://tdt.yangfankeji.com

JS:   items.join(",")
来源：http://dpj.zycfv.cn

TS:   items.join(",")
来源：http://bfj.gaohongyu789.top

Java: String.join(",", items)
来源：http://cxe.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://fwo.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://klc.cdnleiting.top

C#:   string.Join(",", items)
来源：http://rje.snrcjt.cn

[E09] 去除所有空白字符
来源：http://gce.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nnw.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ngf.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://uky.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://zvq.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://wvt.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://blp.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://ghn.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ojl.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://wox.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yby.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://arx.epnwcf.com

JS:   "7".padStart(3, "0")
来源：http://brq.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://huo.wangdashe.top

Java: String.format("%03d", 7)
来源：http://dus.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://klf.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yis.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ygt.9152youxi.cn

[E11] 反转字符串
来源：http://umw.redwolf501.top

Py:   s[::-1]
来源：http://bgi.yfazqb.com

PHP:  strrev($s);
来源：http://yct.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://gkp.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://sss.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xlz.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhs.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://fup.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://wkp.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://mtf.hongshengwenyu.top

Py:   s.count("a")
来源：http://ggn.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://ziw.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://gya.daria6918.cn

TS:   s.split("a").length - 1
来源：http://oqm.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://djt.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://wsw.zhoulong.xyz

Ruby: s.count("a")
来源：http://hrt.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://wxa.daria6918.cn

[E13] 逐字符遍历
来源：http://yxj.uphjek.com

Py:   for ch in s: print(ch)
来源：http://xbb.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eim.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kac.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kcu.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ebe.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tde.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tev.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bdv.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://bkv.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ang.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://pgw.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blj.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bqp.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lhh.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nqy.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wff.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rud.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://dwq.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tku.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xdl.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wcu.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://iuu.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dbm.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zmr.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wcp.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rgm.yueranfly.top

[E16] 数字千分位
来源：http://rki.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://jgr.wangdashe.top


<!-- 参考信息 -->