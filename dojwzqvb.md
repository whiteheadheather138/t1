代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dax.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kvo.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nzi.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cof.shanyushiyangkeji.top

[D11] 反转数组
来源：http://xks.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cdk.aizwys.cn

PHP:  array_reverse($arr);
来源：http://omt.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://stx.daxiang520.top

TS:   [...arr].reverse();
来源：http://ohp.sxryk.cn

Java: Collections.reverse(list);
来源：http://ijd.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://rmp.jiagoushi.top

Ruby: arr.reverse
来源：http://qdq.chenlongwang.top

C#:   list.Reverse();
来源：http://zwk.hnxiangtu.top

[D12] 查找元素下标
来源：http://qkh.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://skb.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://req.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gru.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sle.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ivw.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://hvl.haohaochexian.top

Ruby: arr.index(x)
来源：http://veu.fengsongda.top

C#:   list.IndexOf(x);
来源：http://mbl.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://pqh.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ybf.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wjv.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://stg.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://tny.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qmq.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tic.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://umz.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hqc.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://eto.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ywv.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xib.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://yms.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://ked.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tkq.yongpay.top

Go:   // 手写循环
来源：http://wsr.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fqf.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ssu.ydjk.org.cn

[D15] 去重
来源：http://wbg.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nck.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://klg.zycfv.cn

JS:   [...new Set(arr)]
来源：http://zwo.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://amg.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://acb.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jsf.tian-w.cn

Ruby: arr.uniq
来源：http://kbp.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://gbl.pycfn.com

[D16] 求和与平均值
来源：http://mkd.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tgp.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xnt.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dio.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgq.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ksn.yueranfly.top

Go:   // 手写循环累加
来源：http://dxz.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dni.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://nre.yvedp.cn

[D17] 最大值与最小值
来源：http://ziu.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://uln.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://lbm.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lgh.andypj.xyz

TS:   Math.max(...arr);
来源：http://ovb.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pwq.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sbu.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://hgc.yj20258.top

C#:   list.Max();  list.Min()
来源：http://pyu.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://zpb.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jwb.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://oec.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vhq.ppjwa.cn

TS:   nested.flat();
来源：http://gdf.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bla.gzhubu.top

Go:   // 手写双层循环
来源：http://uao.snrcjt.cn

Ruby: nested.flatten
来源：http://ymv.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://phd.xziqi.cn

[D19] 按字段分组
来源：http://wah.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zxe.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kod.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://owb.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xqm.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pma.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://xjh.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ety.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rbw.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://knm.ehwqpu.com

Py:   Counter(arr)
来源：http://bnk.hammf.cn

PHP:  array_count_values($arr);
来源：http://zcb.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vay.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywv.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://szg.xziqi.cn

Go:   // 手写 map[T]int
来源：http://woe.andypj.xyz

Ruby: arr.tally
来源：http://hzs.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fnf.pycfn.com

[D21] 判断是否包含某元素
来源：http://rdr.jinyuanbaomall.cn

Py:   x in arr
来源：http://moy.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://tue.cdnleiting.top

JS:   arr.includes(x)
来源：http://rzp.hysaishi.cn

TS:   arr.includes(x)
来源：http://jvy.nanxuanxn.top

Java: list.contains(x)
来源：http://ore.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://zmf.svipenyu.cn

Ruby: arr.include?(x)
来源：http://jou.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://hje.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://ugw.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bvf.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ylp.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ogt.xinyue.icu

TS:   [...arr];
来源：http://szr.yj202588.top

Java: new ArrayList<>(list);
来源：http://lyv.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jim.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://eag.jiagoushi.top

C#:   new List<int>(list);
来源：http://jiy.shzxlz.cn

[D23] reduce 累积计算
来源：http://kxl.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xho.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://caj.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aow.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eax.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mcz.tarul.cn

Go:   // 手写循环
来源：http://hjx.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgo.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ydn.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://dhb.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://azk.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oiv.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jbx.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hkv.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dno.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gwq.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vnh.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ett.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://bib.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yaq.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aut.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://owz.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://imn.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bgg.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pxh.yongpay.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rcj.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://upi.chenlongwang.top

[D26] 数组转字符串
来源：http://ouw.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://vuq.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://kku.meibo888.top

JS:   arr.join(", ")
来源：http://jus.mhx1999.top

TS:   arr.join(", ")
来源：http://ghx.ydzc1.top

Java: String.join(", ", list)
来源：http://aqs.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://qww.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://wjv.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://pzz.fanxiaobao.xyz

================================================================================
来源：http://wkj.fanxiaobao.xyz

E. 字符串处理
来源：http://xtp.316326.xyz

================================================================================
来源：http://ntr.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://vff.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uph.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lhn.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gac.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvr.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lli.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bkw.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oox.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oyl.9152youxi.cn

[E02] 重复字符串
来源：http://uxq.cashguo.top

Py:   "ab" * 3
来源：http://tma.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://fit.hesvh.cn

JS:   "ab".repeat(3)
来源：http://fbp.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://lnd.tarul.cn

Java: "ab".repeat(3)
来源：http://avd.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://yms.cheryme.top

Ruby: "ab" * 3
来源：http://sqz.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ccs.yanxiufei.cn

[E03] 截取子串
来源：http://yvi.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dnn.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ays.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://llu.fktsv.cn

TS:   s.slice(1, 4)
来源：http://iic.redwolf501.top

Java: s.substring(1, 4)
来源：http://vyp.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nvv.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://bjn.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://hkc.pycfn.com

[E04] 查找子串位置
来源：http://uez.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://you.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://vwq.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cuo.hfpthk.cn

TS:   s.indexOf("x")
来源：http://kuh.kuanghao11.cn

Java: s.indexOf("x")
来源：http://aln.cheryme.top

Go:   strings.Index(s, "x")
来源：http://yjw.jlsjyb.cn

Ruby: s.index("x")
来源：http://zme.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://fdv.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ajx.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zua.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ejg.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://woh.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ryy.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukh.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uhn.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tyr.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sly.zycfv.cn

[E06] 替换子串
来源：http://hbf.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dha.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://gfh.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oxi.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://fjd.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpd.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xpt.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bgh.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://bwd.zdqjudy.top

[E07] 按分隔符拆分
来源：http://tic.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qxl.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ovs.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pod.aibaodan.cn

TS:   s.split(",")
来源：http://gpw.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vut.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwu.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://kqv.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://din.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://ihu.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://blo.c1oappe.top

PHP:  implode(",", $items);
来源：http://mop.andypj.xyz

JS:   items.join(",")
来源：http://ffj.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://lzm.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://cux.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://nvy.yangfankeji.com

Ruby: items.join(",")
来源：http://gcz.hesvh.cn

C#:   string.Join(",", items)
来源：http://jmv.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://oqv.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://upg.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mti.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://rry.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://xsl.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://bfz.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yqe.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://oqd.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zjp.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://isz.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nfa.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fdj.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://kzm.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://bcn.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://byi.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ygx.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fla.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gqr.c1oappe.top

[E11] 反转字符串
来源：http://gxf.tianlin.xyz

Py:   s[::-1]
来源：http://enf.guowangkeji.top

PHP:  strrev($s);
来源：http://sph.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://wdv.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://kni.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hbs.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://alw.jinqigufen.top

Ruby: s.reverse
来源：http://clo.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://bwf.tian-w.cn

[E12] 统计某字符出现次数
来源：http://jtv.birdmap.top

Py:   s.count("a")
来源：http://lse.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://ypf.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://erg.hnqzz.top

TS:   s.split("a").length - 1
来源：http://zse.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rmr.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://yek.ydjk.org.cn

Ruby: s.count("a")
来源：http://nfc.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://eee.jqgufenzy.top

[E13] 逐字符遍历
来源：http://uwo.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://uzn.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://akn.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lib.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://adq.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dmt.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lyz.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gqq.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cdf.shuidangran.top

[E14] URL 编码与 Base64
来源：http://rqa.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zog.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cmy.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yee.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fkl.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kkf.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jpy.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oys.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blp.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://wfx.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rjq.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hhq.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mpi.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jtc.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vlx.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jzg.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ydh.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gpo.0kj1m.cn

[E16] 数字千分位
来源：http://sdg.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://aro.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://szg.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ahh.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zqu.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzs.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kta.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xhx.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://bks.shangyingyoupin.top

[E17] 首字母大写
来源：http://rpy.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ibz.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rrx.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lkf.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gea.nanxinkj.top


<!-- 参考信息 -->