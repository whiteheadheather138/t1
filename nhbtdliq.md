代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oab.ivvv.top

Ruby: arr.sort
来源：http://joc.smart0.xyz

C#:   list.Sort();
来源：http://dsl.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fhp.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ltp.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://krh.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sgp.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pak.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jrj.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wkt.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cer.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uws.zhixingplan.top

[D11] 反转数组
来源：http://ysk.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wsr.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://ftz.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://axi.iojbl.cn

TS:   [...arr].reverse();
来源：http://idn.dashuyun.cn

Java: Collections.reverse(list);
来源：http://pcd.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://are.zhongyouzk.top

Ruby: arr.reverse
来源：http://apw.yj20258.top

C#:   list.Reverse();
来源：http://ezy.hnxiangtu.top

[D12] 查找元素下标
来源：http://lyb.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://hle.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uia.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://woi.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swn.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hrn.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://uxw.gzhubu.top

Ruby: arr.index(x)
来源：http://hus.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://jvi.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://jcg.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dsi.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qfd.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://scf.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://izt.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zgd.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fkw.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://rxx.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zmi.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://sur.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wbf.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gaz.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://tjc.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://rsi.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gjf.gogol.net.cn

Go:   // 手写循环
来源：http://gzh.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oqk.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ruh.havefunace.top

[D15] 去重
来源：http://bib.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qyz.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://azp.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://mmm.shuidangran.top

TS:   [...new Set(arr)]
来源：http://qsp.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nny.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ypw.tarul.cn

Ruby: arr.uniq
来源：http://qyu.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://xdw.yfazqb.com

[D16] 求和与平均值
来源：http://gaq.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://akw.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cic.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tvt.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://toq.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rqf.haohaochexian.top

Go:   // 手写循环累加
来源：http://tqe.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zpt.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://cqj.hnqzz.top

[D17] 最大值与最小值
来源：http://dcv.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://yjo.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://djb.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://elp.yongpay.top

TS:   Math.max(...arr);
来源：http://bcp.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ymw.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mvy.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://snq.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://pao.yonumen.top

[D18] 扁平化嵌套数组
来源：http://xdw.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ubh.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://bda.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ihj.aibaodan.cn

TS:   nested.flat();
来源：http://ghr.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qcr.vehdjk.com

Go:   // 手写双层循环
来源：http://ajr.tarul.cn

Ruby: nested.flatten
来源：http://rcy.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zfr.gzhubu.top

[D19] 按字段分组
来源：http://ksf.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oli.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ccy.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bpp.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://khb.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wmf.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://wlw.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfj.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eft.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://rpg.fengsongda.top

Py:   Counter(arr)
来源：http://vvt.sweek.top

PHP:  array_count_values($arr);
来源：http://yvh.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gob.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fwg.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zwd.bjfxy.top

Go:   // 手写 map[T]int
来源：http://grq.zhijiandao.cn

Ruby: arr.tally
来源：http://nii.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nmr.bjfxy.top

[D21] 判断是否包含某元素
来源：http://ljg.dashuyun.cn

Py:   x in arr
来源：http://izm.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://zpc.gaohongyu789.top

JS:   arr.includes(x)
来源：http://ycp.uphjek.com

TS:   arr.includes(x)
来源：http://wtu.gaohongyu789.top

Java: list.contains(x)
来源：http://gek.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://tqd.daxiang520.top

Ruby: arr.include?(x)
来源：http://aqq.xylfe.cn

C#:   list.Contains(x)
来源：http://ahp.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://xgl.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uba.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dth.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xkj.uphjek.com

TS:   [...arr];
来源：http://smf.yongpay.top

Java: new ArrayList<>(list);
来源：http://dya.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://qod.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://rnq.havefunace.top

C#:   new List<int>(list);
来源：http://oee.birdmap.top

[D23] reduce 累积计算
来源：http://zff.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://enb.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wrn.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxz.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wks.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pko.hammf.cn

Go:   // 手写循环
来源：http://ztw.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oeo.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wfe.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://tdd.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kyj.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ple.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vxb.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dre.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ebo.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rgw.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wfr.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://obc.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://gkv.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hpk.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rch.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ptt.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ocs.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iss.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rkf.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fqm.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://coi.guannengcc.top

[D26] 数组转字符串
来源：http://wxn.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://fdd.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://nzo.jyoumei.cn

JS:   arr.join(", ")
来源：http://kfj.guowangkeji.top

TS:   arr.join(", ")
来源：http://ybc.tian-w.cn

Java: String.join(", ", list)
来源：http://sbm.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://cks.cqqwz.cn

Ruby: arr.join(", ")
来源：http://efs.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://tnd.wangshuangyany.cn

================================================================================
来源：http://qlh.chenlongwang.top

E. 字符串处理
来源：http://tcj.hywenlv.cn

================================================================================
来源：http://kcl.ydjk.org.cn

[E01] 拼接字符串
来源：http://sgd.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwe.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qkt.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://byt.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://enn.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfs.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vkp.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kju.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lng.sjlbkw.cn

[E02] 重复字符串
来源：http://ohd.dianchejie.cn

Py:   "ab" * 3
来源：http://cbj.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://qee.tian-w.cn

JS:   "ab".repeat(3)
来源：http://iqk.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://xwh.hysaishi.cn

Java: "ab".repeat(3)
来源：http://aca.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://svq.fzhhl.top

Ruby: "ab" * 3
来源：http://jxj.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aca.pengpengdd.cyou

[E03] 截取子串
来源：http://wdr.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ukp.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pkq.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqt.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://bwp.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://uhq.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://waw.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dll.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://eyi.mhx1999.top

[E04] 查找子串位置
来源：http://adi.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://tpb.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://zys.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wab.yj20258.top

TS:   s.indexOf("x")
来源：http://cdk.bjfxy.top

Java: s.indexOf("x")
来源：http://wiv.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://iol.pengpengdd.cyou

Ruby: s.index("x")
来源：http://ihy.bjfxy.top

C#:   s.IndexOf("x")
来源：http://oyz.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dif.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://brj.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eot.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfr.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bcw.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyt.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bqa.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vpd.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jxb.zhengqikj.top

[E06] 替换子串
来源：http://gqx.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swh.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://efz.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://byh.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://nkz.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lub.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ood.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bhe.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rzv.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://uxh.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gog.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wgw.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bje.hnqzz.top

TS:   s.split(",")
来源：http://ilf.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://whc.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bha.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://uyo.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eqm.birdmap.top

[E08] 数组按分隔符合并
来源：http://ieo.cashguo.top

Py:   ",".join(items)
来源：http://sre.xziqi.cn

PHP:  implode(",", $items);
来源：http://gin.meibo888.top

JS:   items.join(",")
来源：http://enw.jqgfzy.top

TS:   items.join(",")
来源：http://jjc.yangfankeji.com

Java: String.join(",", items)
来源：http://egu.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://cix.xinyue.icu

Ruby: items.join(",")
来源：http://sqb.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://mit.epnwcf.com

[E09] 去除所有空白字符
来源：http://eml.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://djr.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jwp.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://uza.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://tql.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://jix.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nqq.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lni.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nji.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://hdh.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xph.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yyb.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://gxq.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://yjj.yfazqb.com

Java: String.format("%03d", 7)
来源：http://vsw.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ryw.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tcw.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://opf.wangdashe.top

[E11] 反转字符串
来源：http://uez.andypj.xyz

Py:   s[::-1]
来源：http://ypj.tianlin.xyz

PHP:  strrev($s);
来源：http://yer.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://ajz.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://myb.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ibp.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://gar.0kj1m.cn

Ruby: s.reverse
来源：http://zpr.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://qpx.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://pbh.fengsongda.top

Py:   s.count("a")
来源：http://sya.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://yyn.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://euy.shuidangran.top

TS:   s.split("a").length - 1
来源：http://gas.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ryd.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://vzo.ivvv.top

Ruby: s.count("a")
来源：http://awp.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://sog.andypj.xyz

[E13] 逐字符遍历
来源：http://vup.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://fln.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nfb.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bbo.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xez.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hqi.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zci.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rfv.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://emq.hcnkem.com

[E14] URL 编码与 Base64
来源：http://iyk.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gql.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wdn.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fjt.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxn.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gzp.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fgs.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zoc.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vfr.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://evl.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://otq.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://coh.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ibb.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://elc.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tms.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkl.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://edw.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dsx.zhongyouzk.top

[E16] 数字千分位
来源：http://qyd.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://gjo.ehwqpu.com

PHP:  number_format(1234567);
来源：http://rkv.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://bbg.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://toq.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxc.dianchejie.cn


<!-- 参考信息 -->