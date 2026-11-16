代发 wailian999

PHP:  sort($arr);
来源：http://pnt.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ner.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qyf.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ibq.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lcr.jinghuilouyu.cn

Ruby: arr.sort
来源：http://ubx.nanxinkj.top

C#:   list.Sort();
来源：http://ixn.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pwe.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://txw.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xrk.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ftb.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iiy.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vgg.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gxb.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://klr.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jya.vehdjk.com

[D11] 反转数组
来源：http://pcl.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://cux.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://cbm.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://brm.jqgfzy.top

TS:   [...arr].reverse();
来源：http://xrb.yfazqb.com

Java: Collections.reverse(list);
来源：http://gqu.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://vmf.yj20258.top

Ruby: arr.reverse
来源：http://rwr.mhx1999.top

C#:   list.Reverse();
来源：http://aad.ivvv.top

[D12] 查找元素下标
来源：http://ovi.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://zur.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bhq.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jng.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zbu.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tks.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://eix.gzhubu.top

Ruby: arr.index(x)
来源：http://qio.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://obi.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://qcr.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bci.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lpc.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://msy.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://neo.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iiz.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cbv.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://fac.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dkz.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://ool.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qwa.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://upd.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://gbr.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://bej.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hco.dianchejie.cn

Go:   // 手写循环
来源：http://kfj.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://njd.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://avn.daxiang520.top

[D15] 去重
来源：http://gzq.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ctw.yangfankeji.com

PHP:  array_unique($arr);
来源：http://vij.gzhubu.top

JS:   [...new Set(arr)]
来源：http://dyn.aizwys.cn

TS:   [...new Set(arr)]
来源：http://ydl.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hfs.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://bup.yuxming.cn

Ruby: arr.uniq
来源：http://vap.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://rwb.sweek.top

[D16] 求和与平均值
来源：http://vkp.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tlk.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wua.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oys.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://itm.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mbh.cqqwz.cn

Go:   // 手写循环累加
来源：http://wye.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mts.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://ybp.zycfv.cn

[D17] 最大值与最小值
来源：http://jwi.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://gnz.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://pmn.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://abv.gogol.net.cn

TS:   Math.max(...arr);
来源：http://ftj.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hps.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://otp.cheryme.top

Ruby: arr.max;  arr.min
来源：http://jgm.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://kuv.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://vee.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hhp.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://url.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pab.ppjwa.cn

TS:   nested.flat();
来源：http://ank.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vgz.vqdsnc.cn

Go:   // 手写双层循环
来源：http://sxk.mhx1999.top

Ruby: nested.flatten
来源：http://gel.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cdm.vqdsnc.cn

[D19] 按字段分组
来源：http://iko.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kco.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kdp.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yzi.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lff.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qox.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://hff.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hex.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://idk.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://vzg.52xcode.cn

Py:   Counter(arr)
来源：http://psr.shuidangran.top

PHP:  array_count_values($arr);
来源：http://csw.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://frh.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzd.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pqj.ydzc1.top

Go:   // 手写 map[T]int
来源：http://cjf.316326.xyz

Ruby: arr.tally
来源：http://aji.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cso.ivvv.top

[D21] 判断是否包含某元素
来源：http://fez.jqgufenzy.top

Py:   x in arr
来源：http://ydd.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://ffw.gotoacloud.top

JS:   arr.includes(x)
来源：http://thb.nanxinkj.top

TS:   arr.includes(x)
来源：http://rnh.jyoumei.cn

Java: list.contains(x)
来源：http://akt.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://ctg.ehwqpu.com

Ruby: arr.include?(x)
来源：http://yvk.tianlin.xyz

C#:   list.Contains(x)
来源：http://upi.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://wxk.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tgh.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rei.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mfk.jyoumei.cn

TS:   [...arr];
来源：http://tmw.havefunace.top

Java: new ArrayList<>(list);
来源：http://chg.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://zyh.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://gfg.zhongyouzk.top

C#:   new List<int>(list);
来源：http://nqb.cdnleiting.top

[D23] reduce 累积计算
来源：http://flo.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gev.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cwp.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://soz.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://art.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oyu.xuetiantiany.cn

Go:   // 手写循环
来源：http://hvb.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fyh.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://akx.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://puo.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pua.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://atw.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sjt.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aqa.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gwy.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yii.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xxt.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://prz.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://ycp.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ift.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wqn.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sbv.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nts.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qll.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://esp.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bvp.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vpn.yangfankeji.com

[D26] 数组转字符串
来源：http://sbl.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://izt.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://mbp.fengsongda.top

JS:   arr.join(", ")
来源：http://cuu.c1oappe.top

TS:   arr.join(", ")
来源：http://qbu.cqqwz.cn

Java: String.join(", ", list)
来源：http://ieu.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://ztb.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://pjj.hesvh.cn

C#:   string.Join(", ", list)
来源：http://xsz.pycfn.com

================================================================================
来源：http://zay.ydjk.org.cn

E. 字符串处理
来源：http://awm.tanke756.top

================================================================================
来源：http://kjy.yj202588.top

[E01] 拼接字符串
来源：http://slp.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hhc.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pun.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://psv.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdi.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pob.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://peb.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ses.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ljq.yj20258888.top

[E02] 重复字符串
来源：http://lal.xylfe.cn

Py:   "ab" * 3
来源：http://emq.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://ovt.hcnkem.com

JS:   "ab".repeat(3)
来源：http://gld.yuxming.cn

TS:   "ab".repeat(3)
来源：http://qbr.c1oappe.top

Java: "ab".repeat(3)
来源：http://uuv.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://xyb.yuxming.cn

Ruby: "ab" * 3
来源：http://vym.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hkh.sjlbkw.cn

[E03] 截取子串
来源：http://gze.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wyl.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jhi.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sky.gzhubu.top

TS:   s.slice(1, 4)
来源：http://kmf.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://lyd.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hvy.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://anb.birdmap.top

C#:   s.Substring(1, 3)
来源：http://anz.tian-w.cn

[E04] 查找子串位置
来源：http://lbi.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://ehy.c1oappe.top

PHP:  strpos($s, "x");
来源：http://bhv.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xmh.shuidangran.top

TS:   s.indexOf("x")
来源：http://wes.fengsongda.top

Java: s.indexOf("x")
来源：http://xcb.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://jgs.gzhubu.top

Ruby: s.index("x")
来源：http://mmv.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://lzu.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pug.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ndj.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rsa.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqi.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyi.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ujv.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zti.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vwv.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jjr.sysykeji.top

[E06] 替换子串
来源：http://rfk.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ezx.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://guy.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovz.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://jkl.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgs.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zwt.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cxp.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://pdf.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://dvh.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ofa.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hbq.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dwu.guannengcc.top

TS:   s.split(",")
来源：http://xad.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://bgd.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pke.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://cbw.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rwq.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://vwq.havefunace.top

Py:   ",".join(items)
来源：http://rvo.redwolf501.top

PHP:  implode(",", $items);
来源：http://but.ppjwa.cn

JS:   items.join(",")
来源：http://ofv.hnqzz.top

TS:   items.join(",")
来源：http://kws.dianchejie.cn

Java: String.join(",", items)
来源：http://gtq.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://djj.mhx1999.top

Ruby: items.join(",")
来源：http://wju.9152youxi.cn

C#:   string.Join(",", items)
来源：http://wca.zdqjudy.top

[E09] 去除所有空白字符
来源：http://puf.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qsq.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tze.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://kut.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://jmv.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://psu.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qwv.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nfr.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gek.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://pfg.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yda.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ixi.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://scg.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://xzf.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://awi.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ypg.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tmz.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ple.c1oappe.top

[E11] 反转字符串
来源：http://gdo.sweek.top

Py:   s[::-1]
来源：http://gyo.jyoumei.cn

PHP:  strrev($s);
来源：http://oed.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://nia.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://ynw.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ypw.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jfb.fanxiaobao.xyz

Ruby: s.reverse
来源：http://yvw.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://yjh.hcnkem.com

[E12] 统计某字符出现次数
来源：http://alb.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://rbt.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://fee.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://xxe.fehbvm.com

TS:   s.split("a").length - 1
来源：http://qqr.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aol.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://lak.hcnkem.com

Ruby: s.count("a")
来源：http://xix.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://nyw.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://drc.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://bgi.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lyw.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://irr.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lgx.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ewc.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pjw.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nkd.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dly.ivvv.top

[E14] URL 编码与 Base64
来源：http://sdl.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oon.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uxn.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vsu.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dhr.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://low.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vxr.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvi.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sxu.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://cyl.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yqe.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xoo.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://has.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mop.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hqv.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kcw.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqq.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bev.ehwqpu.com

[E16] 数字千分位
来源：http://rdc.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://lsu.hfpthk.cn


<!-- 参考信息 -->