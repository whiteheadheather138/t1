代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://auw.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ghg.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lzb.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fqm.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kup.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://laz.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pjm.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nxr.pengpengdd.cyou

[D11] 反转数组
来源：http://yvq.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://oev.c1oappe.top

PHP:  array_reverse($arr);
来源：http://rsk.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cau.cqqwz.cn

TS:   [...arr].reverse();
来源：http://bih.chenzaomai.com

Java: Collections.reverse(list);
来源：http://xup.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://okr.andypj.xyz

Ruby: arr.reverse
来源：http://iuw.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://gjm.ehwqpu.com

[D12] 查找元素下标
来源：http://sxt.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://igo.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oyw.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://opi.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eny.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ept.tanke756.top

Go:   slices.Index(arr, x)
来源：http://cqp.tanke756.top

Ruby: arr.index(x)
来源：http://qfk.vehdjk.com

C#:   list.IndexOf(x);
来源：http://myu.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://dhe.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://plq.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cwj.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://wtr.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://xep.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jze.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oix.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bpo.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://syn.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://jcv.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgv.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zdw.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://lab.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://wxy.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://avn.hysaishi.cn

Go:   // 手写循环
来源：http://lbn.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wlc.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hes.kuanghao11.cn

[D15] 去重
来源：http://txr.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yom.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://fuu.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://bdr.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://nho.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pyw.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://smd.hnqzz.top

Ruby: arr.uniq
来源：http://xpu.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://jpw.chenjidiqi.icu

[D16] 求和与平均值
来源：http://jmi.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pkz.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dmc.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ayu.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zhd.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dzk.hnqzz.top

Go:   // 手写循环累加
来源：http://sxa.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qbr.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://dlo.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://kre.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://dby.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://xds.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ihi.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://ahh.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://grv.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ktb.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://qqb.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://ynq.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://wux.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tlr.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://org.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jck.zhiwuduotai.top

TS:   nested.flat();
来源：http://dth.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gis.hywenlv.cn

Go:   // 手写双层循环
来源：http://gml.ctjpmb.com

Ruby: nested.flatten
来源：http://xtm.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kyu.hnxiangtu.top

[D19] 按字段分组
来源：http://jga.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vhi.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqb.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://isv.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rnj.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rhc.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://wji.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rci.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rdx.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://qhx.xuanzx.com

Py:   Counter(arr)
来源：http://ibq.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://ary.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uje.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nrj.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zco.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://hcn.0kj1m.cn

Ruby: arr.tally
来源：http://qia.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cej.hcnkem.com

[D21] 判断是否包含某元素
来源：http://osv.wangshuangyany.cn

Py:   x in arr
来源：http://fke.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://ggm.cdnleiting.top

JS:   arr.includes(x)
来源：http://yiw.guowangkeji.top

TS:   arr.includes(x)
来源：http://ftd.jqgfzy.top

Java: list.contains(x)
来源：http://uyp.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://hbt.jinqigufen.top

Ruby: arr.include?(x)
来源：http://iel.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://hoj.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://ffn.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ujy.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tsj.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pfz.yj202588.top

TS:   [...arr];
来源：http://cqe.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://fbc.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://faf.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://sei.c1oappe.top

C#:   new List<int>(list);
来源：http://idn.aizwys.cn

[D23] reduce 累积计算
来源：http://loj.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://snp.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://frn.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://okq.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hmo.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ogg.yangfankeji.com

Go:   // 手写循环
来源：http://ggr.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ile.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://arp.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://ujs.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ane.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fvd.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qsg.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zik.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wtr.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgs.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rky.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hxp.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://rny.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bqr.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qru.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dao.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tjh.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ejt.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nnb.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyg.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jha.feifeiyinyue.top

[D26] 数组转字符串
来源：http://qei.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://jow.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://yyc.snrcjt.cn

JS:   arr.join(", ")
来源：http://rrq.uphjek.com

TS:   arr.join(", ")
来源：http://kez.jinqigfzy.top

Java: String.join(", ", list)
来源：http://chz.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://eyd.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://soi.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://tsv.jinghuilouyu.cn

================================================================================
来源：http://dss.mhx1999.top

E. 字符串处理
来源：http://ixz.ydzc1.top

================================================================================
来源：http://rpr.fktsv.cn

[E01] 拼接字符串
来源：http://ncg.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hdf.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aqn.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mjh.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jwn.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ofz.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://abf.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bzw.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://slw.yj202588.top

[E02] 重复字符串
来源：http://zpg.epnwcf.com

Py:   "ab" * 3
来源：http://ixy.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://mdi.wangdashe.top

JS:   "ab".repeat(3)
来源：http://adw.sweek.top

TS:   "ab".repeat(3)
来源：http://djq.xziqi.cn

Java: "ab".repeat(3)
来源：http://tar.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://yve.zycfv.cn

Ruby: "ab" * 3
来源：http://wox.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://daz.hnqzz.top

[E03] 截取子串
来源：http://tbw.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yve.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jjz.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gqu.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://dkd.cqqwz.cn

Java: s.substring(1, 4)
来源：http://exq.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vqw.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://zhs.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://wtv.xuetiantiany.cn

[E04] 查找子串位置
来源：http://xfj.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://dil.yj20258.top

PHP:  strpos($s, "x");
来源：http://brl.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vss.pycfn.com

TS:   s.indexOf("x")
来源：http://pnn.52xcode.cn

Java: s.indexOf("x")
来源：http://nib.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://apf.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://fwa.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://pof.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ttj.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jfr.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rgz.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmo.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ptg.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxw.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dyt.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pvg.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dxf.vqdsnc.cn

[E06] 替换子串
来源：http://ucw.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ixy.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://nge.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nup.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://oba.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggp.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gjq.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://auy.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://vti.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://ggr.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jfn.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qbw.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://nfr.hywenlv.cn

TS:   s.split(",")
来源：http://out.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://ebw.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://llq.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://epg.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qeu.jianghu66.top

[E08] 数组按分隔符合并
来源：http://ptl.tianlin.xyz

Py:   ",".join(items)
来源：http://uav.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://udu.gotoacloud.top

JS:   items.join(",")
来源：http://wok.yueranfly.top

TS:   items.join(",")
来源：http://bjm.zhengqikj.top

Java: String.join(",", items)
来源：http://mcs.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://iqa.feifeiyinyue.top

Ruby: items.join(",")
来源：http://jwc.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://abe.havefunace.top

[E09] 去除所有空白字符
来源：http://aqq.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wik.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wbz.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://hlm.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://hlz.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://xhg.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://wda.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dsb.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bfh.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://dfj.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lan.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lxn.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://vpc.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://bci.yfazqb.com

Java: String.format("%03d", 7)
来源：http://qeq.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kmy.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fjf.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zaq.dianchejie.cn

[E11] 反转字符串
来源：http://akf.hcnkem.com

Py:   s[::-1]
来源：http://fja.vehdjk.com

PHP:  strrev($s);
来源：http://iuo.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://orh.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://zfm.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ciu.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://hir.cdnleiting.top

Ruby: s.reverse
来源：http://tbb.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://oax.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://oyr.zhoulong.xyz

Py:   s.count("a")
来源：http://liv.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://ubm.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://fnx.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://slr.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kxz.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://iul.daxiang520.top

Ruby: s.count("a")
来源：http://jbj.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://ace.shuidangran.top

[E13] 逐字符遍历
来源：http://rxe.tanke756.top

Py:   for ch in s: print(ch)
来源：http://ait.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eai.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://vcy.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uyc.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://crz.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ddu.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nsh.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fpu.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://vyt.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tbv.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tip.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zlg.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://owl.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xll.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ahz.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xrn.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yma.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://kxs.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yzc.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bzl.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uwx.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xxw.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zfj.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://anl.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bff.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ybj.zdbjq.cn

[E16] 数字千分位
来源：http://ayv.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://zwo.sweek.top

PHP:  number_format(1234567);
来源：http://aue.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://dkr.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eem.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qfu.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://add.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gzl.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://ydx.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://nnw.fzhhl.top


<!-- 参考信息 -->