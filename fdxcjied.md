代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ycg.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fza.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnt.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://job.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wow.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vfz.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbz.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hva.jlsjyb.cn

[D11] 反转数组
来源：http://txp.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://tdk.316326.xyz

PHP:  array_reverse($arr);
来源：http://sbe.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dig.ivvv.top

TS:   [...arr].reverse();
来源：http://dkj.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://jvf.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://dat.hfpthk.cn

Ruby: arr.reverse
来源：http://pgl.9152youxi.cn

C#:   list.Reverse();
来源：http://nub.hnqzz.top

[D12] 查找元素下标
来源：http://izh.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://ixn.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pef.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hfr.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wns.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mwe.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://vgf.hnxiangtu.top

Ruby: arr.index(x)
来源：http://jsj.gzhubu.top

C#:   list.IndexOf(x);
来源：http://jai.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://imm.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xrr.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gwb.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://czk.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://xdi.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vuk.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://thn.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://ikv.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://jtq.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://xnd.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dmo.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hgm.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://hjl.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://nvr.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fcy.aizwys.cn

Go:   // 手写循环
来源：http://frn.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://nip.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://upe.jinqigufen.top

[D15] 去重
来源：http://mbt.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pvt.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://cux.yuxming.cn

JS:   [...new Set(arr)]
来源：http://myo.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://evz.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fso.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://twz.kuanghao11.cn

Ruby: arr.uniq
来源：http://thz.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://oru.zhongyouzk.top

[D16] 求和与平均值
来源：http://dvj.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jwo.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ntz.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fte.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mkh.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sns.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://ned.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mlc.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://xxf.yj20258.top

[D17] 最大值与最小值
来源：http://mtw.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://uiv.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://kig.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://brs.xylfe.cn

TS:   Math.max(...arr);
来源：http://zac.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ktm.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uat.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://fcn.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://hom.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://tch.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lzv.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://qtl.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dqh.yuxming.cn

TS:   nested.flat();
来源：http://omg.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tgd.bjfxy.top

Go:   // 手写双层循环
来源：http://ufu.ivvv.top

Ruby: nested.flatten
来源：http://zrk.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tlq.hesvh.cn

[D19] 按字段分组
来源：http://vcf.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://whj.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rpa.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rin.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lwh.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sel.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://ohc.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tne.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zdl.hammf.cn

[D20] 统计每个元素出现次数
来源：http://per.hfpthk.cn

Py:   Counter(arr)
来源：http://olx.wangdashe.top

PHP:  array_count_values($arr);
来源：http://xdn.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cjv.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qdu.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bzy.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://job.yvedp.cn

Ruby: arr.tally
来源：http://pif.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wvt.ybcxt.top

[D21] 判断是否包含某元素
来源：http://ahp.jqgfzy.top

Py:   x in arr
来源：http://jwr.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://bbp.dianchejie.cn

JS:   arr.includes(x)
来源：http://rzc.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://ill.shanyushiyangtech.top

Java: list.contains(x)
来源：http://qpv.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://gsw.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://zfr.zhoulong.xyz

C#:   list.Contains(x)
来源：http://xpr.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://lay.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ear.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xfk.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fis.yuxming.cn

TS:   [...arr];
来源：http://qxx.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://jtz.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://hqj.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://fra.nanxuanxn.top

C#:   new List<int>(list);
来源：http://pmg.fktsv.cn

[D23] reduce 累积计算
来源：http://ski.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tjm.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ifr.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbi.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzs.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ztk.aibaodan.cn

Go:   // 手写循环
来源：http://fav.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ysk.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tie.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://tfs.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tnt.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pec.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jaa.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptd.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jvo.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pfs.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://loy.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ugb.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://opp.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ped.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://buc.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yqg.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://osu.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bfw.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xng.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mvg.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qhg.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://cex.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://drf.birdmap.top

PHP:  implode(", ", $arr);
来源：http://rgg.xuanzx.com

JS:   arr.join(", ")
来源：http://udp.quarkkingdee.top

TS:   arr.join(", ")
来源：http://dkf.fzhhl.top

Java: String.join(", ", list)
来源：http://pba.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://xzo.c1oappe.top

Ruby: arr.join(", ")
来源：http://btb.uphjek.com

C#:   string.Join(", ", list)
来源：http://wdb.fzhhl.top

================================================================================
来源：http://php.cqqwz.cn

E. 字符串处理
来源：http://qxw.nwbrower.top

================================================================================
来源：http://cup.fktsv.cn

[E01] 拼接字符串
来源：http://lsv.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uru.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpf.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uju.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rwp.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://emc.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xbq.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cjf.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oqz.xuanzx.com

[E02] 重复字符串
来源：http://icy.yj202588.top

Py:   "ab" * 3
来源：http://hxa.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://rgt.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://yuz.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://jue.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://gnu.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ykz.ctjpmb.com

Ruby: "ab" * 3
来源：http://mpl.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://exo.ydjk.org.cn

[E03] 截取子串
来源：http://lyp.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sbe.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hhf.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ogs.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://qmi.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://hzf.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://byh.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://wrs.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://vjr.mhx1999.top

[E04] 查找子串位置
来源：http://poh.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://fdh.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://vxz.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yei.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://dxl.sweek.top

Java: s.indexOf("x")
来源：http://dzk.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://nsn.tarul.cn

Ruby: s.index("x")
来源：http://wzj.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://syc.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zzn.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zro.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zmz.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hbq.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekn.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvk.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pgz.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xej.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qsn.nanxuanxn.top

[E06] 替换子串
来源：http://nwm.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vxz.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://vmz.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hjp.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://czg.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lmt.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kbx.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lkz.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://rqb.tarul.cn

[E07] 按分隔符拆分
来源：http://qmx.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bss.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ovp.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://okk.vehdjk.com

TS:   s.split(",")
来源：http://une.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://jen.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kny.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://ykw.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mts.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://dpi.guowangkeji.top

Py:   ",".join(items)
来源：http://xol.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://wic.sysykeji.top

JS:   items.join(",")
来源：http://zbd.tianlin.xyz

TS:   items.join(",")
来源：http://zvc.dashuyun.cn

Java: String.join(",", items)
来源：http://rpd.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://lax.c1oappe.top

Ruby: items.join(",")
来源：http://zqt.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://kei.sufxvd.cn

[E09] 去除所有空白字符
来源：http://qcv.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxf.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wnk.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://ltj.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://kbl.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://weq.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ybp.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rhz.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gbe.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://yks.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rxz.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://woc.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://eoo.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://opm.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://yny.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://htu.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zsd.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hdx.jyoumei.cn

[E11] 反转字符串
来源：http://obr.iojbl.cn

Py:   s[::-1]
来源：http://ndt.cucudq.cn

PHP:  strrev($s);
来源：http://tup.hammf.cn

JS:   [...s].reverse().join("")
来源：http://vfn.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://mlt.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://phe.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xwj.mhx1999.top

Ruby: s.reverse
来源：http://ooc.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pge.wangdashe.top

[E12] 统计某字符出现次数
来源：http://mcv.zycfv.cn

Py:   s.count("a")
来源：http://rez.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://afo.tarul.cn

JS:   s.split("a").length - 1
来源：http://qqm.xinyue.icu

TS:   s.split("a").length - 1
来源：http://wmg.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kfz.cashguo.top

Go:   strings.Count(s, "a")
来源：http://pfk.jqgfzy.top

Ruby: s.count("a")
来源：http://nni.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://out.shuidangran.top

[E13] 逐字符遍历
来源：http://zij.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://und.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jrs.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bnm.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vsk.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aco.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://upe.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cre.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kzo.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://fdu.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xwm.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uyr.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ant.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rau.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zej.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uqu.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bpw.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://efn.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://xdp.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://skw.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lxm.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zbz.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qel.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uig.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://usk.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://paf.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://llq.ppjwa.cn

[E16] 数字千分位
来源：http://oph.fzhhl.top

Py:   f"{1234567:,}"
来源：http://ivh.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://okm.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mni.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tug.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jpj.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cbx.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ban.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://acj.xziqi.cn

[E17] 首字母大写
来源：http://pvs.cheryme.top


<!-- 参考信息 -->