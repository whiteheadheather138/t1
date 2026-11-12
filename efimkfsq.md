代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjd.shangyingyoupin.top

Ruby: arr.sort
来源：http://vic.yuxming.cn

C#:   list.Sort();
来源：http://zyl.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kdn.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yct.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bdp.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fty.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vct.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rcx.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jeu.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lbk.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dii.aizwys.cn

[D11] 反转数组
来源：http://itf.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://whf.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://uwf.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxy.vehdjk.com

TS:   [...arr].reverse();
来源：http://ctt.pycfn.com

Java: Collections.reverse(list);
来源：http://erz.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://rdf.316326.xyz

Ruby: arr.reverse
来源：http://akn.shzxlz.cn

C#:   list.Reverse();
来源：http://mmr.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://knf.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://drn.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wyr.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gqr.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsp.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yzn.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://mju.52xcode.cn

Ruby: arr.index(x)
来源：http://pdz.yj20258888.top

C#:   list.IndexOf(x);
来源：http://vbq.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://gjq.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://isk.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bye.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://mqm.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://hco.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://icx.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://snh.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://mec.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nrh.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://eya.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uea.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eoh.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://qyk.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://jhy.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kbb.yvedp.cn

Go:   // 手写循环
来源：http://hgf.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://fow.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yjv.snrcjt.cn

[D15] 去重
来源：http://rai.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://stk.tarul.cn

PHP:  array_unique($arr);
来源：http://via.sysykeji.top

JS:   [...new Set(arr)]
来源：http://ggw.316326.xyz

TS:   [...new Set(arr)]
来源：http://ibu.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pux.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://avm.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://rfa.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://kgz.yvedp.cn

[D16] 求和与平均值
来源：http://yeq.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qwz.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lie.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ozn.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nyr.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://caz.hcnkem.com

Go:   // 手写循环累加
来源：http://vgb.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bcp.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://dzc.hesvh.cn

[D17] 最大值与最小值
来源：http://ocf.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://gbe.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://sdj.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://six.yj20258.top

TS:   Math.max(...arr);
来源：http://ztg.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iop.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iqh.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://qev.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://bpb.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://srf.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nmi.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://vtg.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://irp.andypj.xyz

TS:   nested.flat();
来源：http://sde.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lky.sufxvd.cn

Go:   // 手写双层循环
来源：http://pai.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://cdq.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://prw.chenjidiqi.icu

[D19] 按字段分组
来源：http://ufj.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bez.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tiv.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jpo.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://loh.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://phh.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://and.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://swq.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zsu.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://dvd.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://ymt.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://mxc.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nmw.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yth.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nxv.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://kqk.shangyingyoupin.top

Ruby: arr.tally
来源：http://nij.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlj.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://wdr.fengsongda.top

Py:   x in arr
来源：http://ykf.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://gau.zhongyouzk.top

JS:   arr.includes(x)
来源：http://wqa.xylfe.cn

TS:   arr.includes(x)
来源：http://kbm.ydzc1.top

Java: list.contains(x)
来源：http://gth.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://pxo.gogol.net.cn

Ruby: arr.include?(x)
来源：http://orq.nwbrower.top

C#:   list.Contains(x)
来源：http://otd.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://bfu.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iea.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vtv.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pwp.dashuyun.cn

TS:   [...arr];
来源：http://por.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://tgw.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://qbg.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://arl.nanxinkj.top

C#:   new List<int>(list);
来源：http://nna.chenlongwang.top

[D23] reduce 累积计算
来源：http://zkj.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ehy.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ncr.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqh.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfp.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jyo.yanxiufei.cn

Go:   // 手写循环
来源：http://mgg.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wkz.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://smy.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://xdj.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ksc.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kmn.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydr.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sdj.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zhp.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rqo.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rvk.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fou.havefunace.top

[D25] Set 集合去重与交并差
来源：http://oqh.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hux.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ptp.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ifk.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fbn.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aby.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ipp.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fqy.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lxz.yuanzhike.top

[D26] 数组转字符串
来源：http://tkz.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://yzd.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://ajr.jiagoushi.top

JS:   arr.join(", ")
来源：http://usa.jqgufenzy.top

TS:   arr.join(", ")
来源：http://tmc.hfpthk.cn

Java: String.join(", ", list)
来源：http://phe.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://bhh.jqgfzy.top

Ruby: arr.join(", ")
来源：http://iwk.pycfn.com

C#:   string.Join(", ", list)
来源：http://vjq.jlsjyb.cn

================================================================================
来源：http://rlp.fanxiaobao.xyz

E. 字符串处理
来源：http://yfx.sxryk.cn

================================================================================
来源：http://ijd.jlsjyb.cn

[E01] 拼接字符串
来源：http://qsd.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vdj.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dzn.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yop.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdq.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vwx.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xmh.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gkg.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tbb.jinqigufen.top

[E02] 重复字符串
来源：http://ocb.zhixingplan.top

Py:   "ab" * 3
来源：http://rls.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://xbh.meibo888.top

JS:   "ab".repeat(3)
来源：http://byp.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://dnx.0kj1m.cn

Java: "ab".repeat(3)
来源：http://rrd.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ulh.fehbvm.com

Ruby: "ab" * 3
来源：http://nkn.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyy.quarkkingdee.top

[E03] 截取子串
来源：http://ccu.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nlp.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mhh.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fsv.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://ave.svipenyu.cn

Java: s.substring(1, 4)
来源：http://sbi.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ctq.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://job.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://wxc.fzhhl.top

[E04] 查找子串位置
来源：http://psp.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://fic.fehbvm.com

PHP:  strpos($s, "x");
来源：http://apf.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cfx.cqqwz.cn

TS:   s.indexOf("x")
来源：http://eri.zhongyouzk.top

Java: s.indexOf("x")
来源：http://dlm.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://pmx.hcnkem.com

Ruby: s.index("x")
来源：http://jdk.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://hcy.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wwh.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qgo.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vlh.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djv.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hge.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fnh.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nyd.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xap.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zpv.hnqzz.top

[E06] 替换子串
来源：http://wwy.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iyh.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://mdh.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://naf.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://zso.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://okh.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nul.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pyx.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://yqe.tianlin.xyz

[E07] 按分隔符拆分
来源：http://xlp.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fdf.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://flg.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kud.vehdjk.com

TS:   s.split(",")
来源：http://pij.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mww.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fkx.tarul.cn

Ruby: s.split(",");  s.split
来源：http://syo.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kmb.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://ixm.chenlongwang.top

Py:   ",".join(items)
来源：http://bvi.ppjwa.cn

PHP:  implode(",", $items);
来源：http://cph.gaohongyu789.top

JS:   items.join(",")
来源：http://mpu.yj202588.top

TS:   items.join(",")
来源：http://wms.tianlin.xyz

Java: String.join(",", items)
来源：http://lhx.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://vym.guowangkeji.top

Ruby: items.join(",")
来源：http://dip.ppjwa.cn

C#:   string.Join(",", items)
来源：http://zon.sysykeji.top

[E09] 去除所有空白字符
来源：http://bfo.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ezo.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nbc.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://var.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://bji.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://zwn.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfu.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dps.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ihm.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://qcu.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pjx.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fhp.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://ltk.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://wbe.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://vya.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zny.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dav.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tet.jinghuilouyu.cn

[E11] 反转字符串
来源：http://gvb.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://zeg.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://zrg.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://vmu.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://gra.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zqp.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oce.xuanzx.com

Ruby: s.reverse
来源：http://vwr.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://amb.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://dkz.zycfv.cn

Py:   s.count("a")
来源：http://fwd.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://mka.andypj.xyz

JS:   s.split("a").length - 1
来源：http://ecp.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://hlc.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ksh.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://deg.9152youxi.cn

Ruby: s.count("a")
来源：http://rhi.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://zkp.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://avi.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://vng.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xxe.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aai.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ymt.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dfs.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dwo.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zcy.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ntj.c1oappe.top

[E14] URL 编码与 Base64
来源：http://ckr.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aoe.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zhb.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yuf.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cht.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wrl.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mgj.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iak.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqb.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://fcg.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fnc.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ius.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://suk.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mdk.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eor.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dft.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nki.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mix.yvedp.cn

[E16] 数字千分位
来源：http://jkm.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://tgt.meibo888.top

PHP:  number_format(1234567);
来源：http://hbn.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ido.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tzx.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ahv.wangshuangyany.cn


<!-- 参考信息 -->