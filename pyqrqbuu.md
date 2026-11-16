代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ucf.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ycv.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://acl.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxq.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dix.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nhc.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xji.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://owt.aibaodan.cn

[D11] 反转数组
来源：http://znc.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fzv.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://uco.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tcu.yfazqb.com

TS:   [...arr].reverse();
来源：http://sed.jianghu66.top

Java: Collections.reverse(list);
来源：http://alo.tarul.cn

Go:   slices.Reverse(arr)
来源：http://zfc.cucudq.cn

Ruby: arr.reverse
来源：http://pwg.jianghu66.top

C#:   list.Reverse();
来源：http://lnv.quarkkingdee.top

[D12] 查找元素下标
来源：http://klw.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://cqq.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lew.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iat.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ior.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mta.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://bnt.fktsv.cn

Ruby: arr.index(x)
来源：http://pfz.havefunace.top

C#:   list.IndexOf(x);
来源：http://pbh.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://xzb.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yld.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xtr.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://fdt.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://iat.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://onu.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://geb.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vxs.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fto.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://thk.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xxs.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jiu.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://igk.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://sle.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cjf.sufxvd.cn

Go:   // 手写循环
来源：http://kjk.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://ohs.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://own.mhx1999.top

[D15] 去重
来源：http://vli.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jpv.yongpay.top

PHP:  array_unique($arr);
来源：http://mla.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://bha.cucudq.cn

TS:   [...new Set(arr)]
来源：http://cen.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jmq.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://mnh.nanxinkj.top

Ruby: arr.uniq
来源：http://lzl.tarul.cn

C#:   list.Distinct().ToList()
来源：http://ukg.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://ily.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://brr.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gkj.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rwk.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tix.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oab.xinyue.icu

Go:   // 手写循环累加
来源：http://bhx.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rgz.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://vkx.316326.xyz

[D17] 最大值与最小值
来源：http://zhs.yj202588.top

Py:   max(arr);  min(arr)
来源：http://ljt.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://eni.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mth.uphjek.com

TS:   Math.max(...arr);
来源：http://qyd.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://eyg.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zaz.ivvv.top

Ruby: arr.max;  arr.min
来源：http://vhv.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://efn.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://pqe.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://clv.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://ifh.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://naq.fengsongda.top

TS:   nested.flat();
来源：http://kjk.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://apo.epnwcf.com

Go:   // 手写双层循环
来源：http://zdr.andypj.xyz

Ruby: nested.flatten
来源：http://cpv.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iht.ehwqpu.com

[D19] 按字段分组
来源：http://mps.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fsl.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kwa.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jjh.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qaa.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bal.ivvv.top

Go:   // 手写 map[string][]T
来源：http://eug.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://slj.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mrz.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://qvi.dianchejie.cn

Py:   Counter(arr)
来源：http://mcb.316326.xyz

PHP:  array_count_values($arr);
来源：http://jpd.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://szw.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pyv.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fhl.yuxming.cn

Go:   // 手写 map[T]int
来源：http://yhv.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://nju.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nel.yvedp.cn

[D21] 判断是否包含某元素
来源：http://jes.hnxiangtu.top

Py:   x in arr
来源：http://xds.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://kck.kuanghao11.cn

JS:   arr.includes(x)
来源：http://ihz.cheryme.top

TS:   arr.includes(x)
来源：http://eym.tian-w.cn

Java: list.contains(x)
来源：http://nxr.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://zfc.fengsongda.top

Ruby: arr.include?(x)
来源：http://hwn.fktsv.cn

C#:   list.Contains(x)
来源：http://xak.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://xnp.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fpr.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://anm.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qob.hongshengwenyu.top

TS:   [...arr];
来源：http://whe.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://quu.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://qnt.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://thf.zdbjq.cn

C#:   new List<int>(list);
来源：http://jjv.uphjek.com

[D23] reduce 累积计算
来源：http://qte.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcv.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ilx.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fqj.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://okz.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://elq.hcnkem.com

Go:   // 手写循环
来源：http://sxe.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxx.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qha.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://lun.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iej.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aby.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fff.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zpv.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://udw.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hbr.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qbd.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://onx.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://vbk.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qeb.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yae.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sgt.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yia.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwc.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pkf.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://loq.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zuw.9152youxi.cn

[D26] 数组转字符串
来源：http://llh.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://tjq.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://tds.ydjk.org.cn

JS:   arr.join(", ")
来源：http://xia.tanke756.top

TS:   arr.join(", ")
来源：http://era.shzxlz.cn

Java: String.join(", ", list)
来源：http://ols.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://ois.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://lyo.ybcxt.top

C#:   string.Join(", ", list)
来源：http://nhb.epnwcf.com

================================================================================
来源：http://qho.hcnkem.com

E. 字符串处理
来源：http://cry.guannengcc.top

================================================================================
来源：http://cuv.xinyue.icu

[E01] 拼接字符串
来源：http://hxh.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jgn.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ori.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bod.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofp.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kdi.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvk.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eko.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mii.quarkkingdee.top

[E02] 重复字符串
来源：http://yrv.smart0.xyz

Py:   "ab" * 3
来源：http://rwe.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://pip.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://qvt.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://lcf.yvedp.cn

Java: "ab".repeat(3)
来源：http://ihm.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://hte.tian-w.cn

Ruby: "ab" * 3
来源：http://mtb.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rye.cashguo.top

[E03] 截取子串
来源：http://cxg.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ezm.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tec.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mmk.ybcxt.top

TS:   s.slice(1, 4)
来源：http://uyl.sufxvd.cn

Java: s.substring(1, 4)
来源：http://wxq.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ghf.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://abj.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://nja.52xcode.cn

[E04] 查找子串位置
来源：http://jmz.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://ycf.ybcxt.top

PHP:  strpos($s, "x");
来源：http://fzc.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.shuidangran.top

TS:   s.indexOf("x")
来源：http://ufg.sufxvd.cn

Java: s.indexOf("x")
来源：http://nhn.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://zai.pengpengdd.cyou

Ruby: s.index("x")
来源：http://pbb.pycfn.com

C#:   s.IndexOf("x")
来源：http://wri.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vol.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qrk.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://joz.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jeg.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sra.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://atc.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fwa.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zwq.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uli.shangyingyoupin.top

[E06] 替换子串
来源：http://btv.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://emu.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://nym.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qys.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://djf.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbw.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://osd.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cnf.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://awr.shzxlz.cn

[E07] 按分隔符拆分
来源：http://wkx.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://prx.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iiy.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://svk.zhoulong.xyz

TS:   s.split(",")
来源：http://zxr.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ihc.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uxj.havefunace.top

Ruby: s.split(",");  s.split
来源：http://ilo.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ftv.xinyue.icu

[E08] 数组按分隔符合并
来源：http://awp.feifeiyinyue.top

Py:   ",".join(items)
来源：http://oqf.mhx1999.top

PHP:  implode(",", $items);
来源：http://wzv.ivvv.top

JS:   items.join(",")
来源：http://fwg.9152youxi.cn

TS:   items.join(",")
来源：http://hbp.snrcjt.cn

Java: String.join(",", items)
来源：http://cqd.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://imi.xuetiantiany.cn

Ruby: items.join(",")
来源：http://gdi.tian-w.cn

C#:   string.Join(",", items)
来源：http://jef.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://fkb.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tsm.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nyy.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://trv.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://ata.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://epl.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ifd.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yrw.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arx.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://szn.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hkc.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vhv.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://ymk.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://qct.yvedp.cn

Java: String.format("%03d", 7)
来源：http://ixj.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cxk.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xpr.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bky.sxryk.cn

[E11] 反转字符串
来源：http://war.nanxuanxn.top

Py:   s[::-1]
来源：http://kjs.cucudq.cn

PHP:  strrev($s);
来源：http://qty.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://pgy.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://psc.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://szp.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lku.epnwcf.com

Ruby: s.reverse
来源：http://fyr.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://apb.daxiang520.top

[E12] 统计某字符出现次数
来源：http://stg.hammf.cn

Py:   s.count("a")
来源：http://vkj.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://scw.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://ndf.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://plc.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qmo.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://vyw.0kj1m.cn

Ruby: s.count("a")
来源：http://qod.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://ihw.tarul.cn

[E13] 逐字符遍历
来源：http://hji.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://dyo.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kkq.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewd.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://srh.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://epc.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ikb.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dbc.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qkb.ivvv.top

[E14] URL 编码与 Base64
来源：http://vxn.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://awj.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ebk.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhk.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ogk.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vpi.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdm.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://keo.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kjy.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://kvs.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dsa.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hnu.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cus.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yyt.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gfm.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ruq.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xkt.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vsj.yuanzhike.top

[E16] 数字千分位
来源：http://cps.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://rvz.yonumen.top

PHP:  number_format(1234567);
来源：http://uyn.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rqz.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bao.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bah.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vuo.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aqu.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://vre.tanke756.top

[E17] 首字母大写
来源：http://uxk.ctjpmb.com


<!-- 参考信息 -->