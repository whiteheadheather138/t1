代发 wailian999

PHP:  sort($arr);
来源：http://zhf.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tgr.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kaa.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xsk.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ovg.yueranfly.top

Ruby: arr.sort
来源：http://ofz.iojbl.cn

C#:   list.Sort();
来源：http://apa.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cdn.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aoq.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bjz.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwf.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://brb.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eut.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://spg.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ecq.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://szs.zycfv.cn

[D11] 反转数组
来源：http://gmi.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://qig.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://zyi.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qpw.xziqi.cn

TS:   [...arr].reverse();
来源：http://zgd.hywenlv.cn

Java: Collections.reverse(list);
来源：http://ajo.ivvv.top

Go:   slices.Reverse(arr)
来源：http://txi.fktsv.cn

Ruby: arr.reverse
来源：http://ppy.feifeiyinyue.top

C#:   list.Reverse();
来源：http://smo.cashguo.top

[D12] 查找元素下标
来源：http://mix.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://lvo.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mof.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pea.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htz.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gab.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://siv.hesvh.cn

Ruby: arr.index(x)
来源：http://hod.uphjek.com

C#:   list.IndexOf(x);
来源：http://xck.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://hby.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lyy.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vxd.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://ffc.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://pgy.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bjp.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ybo.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://gyu.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dqu.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://btn.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uco.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yhh.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://orb.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://cag.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://dws.yonumen.top

Go:   // 手写循环
来源：http://xls.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://cze.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dmc.yj20258.top

[D15] 去重
来源：http://uae.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://knx.shzxlz.cn

PHP:  array_unique($arr);
来源：http://gfk.yj20258888.top

JS:   [...new Set(arr)]
来源：http://fen.xuanzx.com

TS:   [...new Set(arr)]
来源：http://jtj.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vga.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://jaf.yuxming.cn

Ruby: arr.uniq
来源：http://cqd.cheryme.top

C#:   list.Distinct().ToList()
来源：http://qqn.mhx1999.top

[D16] 求和与平均值
来源：http://slr.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jib.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hlk.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nml.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sox.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lmu.zhongyouzk.top

Go:   // 手写循环累加
来源：http://sfn.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gap.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://pfp.sjlbkw.cn

[D17] 最大值与最小值
来源：http://sff.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://ahe.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://gtw.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zxz.jqgfzy.top

TS:   Math.max(...arr);
来源：http://ioc.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://obc.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pvt.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://dmo.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://wyn.yonumen.top

[D18] 扁平化嵌套数组
来源：http://itc.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://azc.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://twr.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gix.cucudq.cn

TS:   nested.flat();
来源：http://mjg.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wvp.hywenlv.cn

Go:   // 手写双层循环
来源：http://kuv.sweek.top

Ruby: nested.flatten
来源：http://klw.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yol.zhiwuduotai.top

[D19] 按字段分组
来源：http://rzd.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wsp.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://edy.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wdh.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dgz.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qjy.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://uzs.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://cty.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jlz.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://zst.cqqwz.cn

Py:   Counter(arr)
来源：http://tam.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://mzm.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zch.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://haa.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bvv.fzhhl.top

Go:   // 手写 map[T]int
来源：http://cip.shuidangran.top

Ruby: arr.tally
来源：http://spe.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bjq.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://swo.jinghuilouyu.cn

Py:   x in arr
来源：http://zzx.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://hox.yanxiufei.cn

JS:   arr.includes(x)
来源：http://dbh.dianchejie.cn

TS:   arr.includes(x)
来源：http://cny.ybcxt.top

Java: list.contains(x)
来源：http://aao.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://pnv.tianlin.xyz

Ruby: arr.include?(x)
来源：http://wxu.hammf.cn

C#:   list.Contains(x)
来源：http://zzn.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://lxu.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wsd.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xbu.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://upw.zycfv.cn

TS:   [...arr];
来源：http://igq.wangdashe.top

Java: new ArrayList<>(list);
来源：http://gky.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://opk.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://npe.guowangkeji.top

C#:   new List<int>(list);
来源：http://vjw.yuanzhike.top

[D23] reduce 累积计算
来源：http://klv.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://igc.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aac.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://agf.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qsy.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://liu.ivvv.top

Go:   // 手写循环
来源：http://kdw.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://azl.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ilf.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://pmr.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gel.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ewt.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ass.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pry.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uie.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jkh.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ikc.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tzm.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://yoz.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zcn.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pts.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zij.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kqf.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ttq.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bhj.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pdl.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nkn.jqgfzy.top

[D26] 数组转字符串
来源：http://zaj.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://ksn.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://pcd.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://fdl.tian-w.cn

TS:   arr.join(", ")
来源：http://puo.xuanzx.com

Java: String.join(", ", list)
来源：http://hrq.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://wbc.iojbl.cn

Ruby: arr.join(", ")
来源：http://rpj.yfazqb.com

C#:   string.Join(", ", list)
来源：http://wpg.feifeiyinyue.top

================================================================================
来源：http://wgo.nanxuanxn.top

E. 字符串处理
来源：http://zfm.jianghu66.top

================================================================================
来源：http://jdl.ybcxt.top

[E01] 拼接字符串
来源：http://kep.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nkl.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eux.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xei.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlo.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yjn.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://omz.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mzk.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://udy.52xcode.cn

[E02] 重复字符串
来源：http://fzu.daxiang520.top

Py:   "ab" * 3
来源：http://pqi.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://odk.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://ykl.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://nnv.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://rjh.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ezr.shzxlz.cn

Ruby: "ab" * 3
来源：http://nyc.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cqs.yuanzhike.top

[E03] 截取子串
来源：http://piy.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://osu.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lou.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ssd.shuidangran.top

TS:   s.slice(1, 4)
来源：http://aul.hywenlv.cn

Java: s.substring(1, 4)
来源：http://wdd.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nai.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cnt.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://afh.shzxlz.cn

[E04] 查找子串位置
来源：http://kgt.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://tyc.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://nan.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qjs.wangdashe.top

TS:   s.indexOf("x")
来源：http://zhd.yvedp.cn

Java: s.indexOf("x")
来源：http://ekc.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://dtw.dianchejie.cn

Ruby: s.index("x")
来源：http://yzo.wangdashe.top

C#:   s.IndexOf("x")
来源：http://fhh.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gpy.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nda.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fue.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqf.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lnl.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jlf.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zyi.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uug.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aek.birdmap.top

[E06] 替换子串
来源：http://sim.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ypu.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://rhb.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgh.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://ugl.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bpy.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yig.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hiq.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://cql.chenlongwang.top

[E07] 按分隔符拆分
来源：http://hrn.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gfq.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://own.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://onv.yfazqb.com

TS:   s.split(",")
来源：http://tfg.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://cyo.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://edd.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://yvv.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jze.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://myt.xziqi.cn

Py:   ",".join(items)
来源：http://adq.pycfn.com

PHP:  implode(",", $items);
来源：http://yzv.c1oappe.top

JS:   items.join(",")
来源：http://ufp.zhongyouzk.top

TS:   items.join(",")
来源：http://ctc.andypj.xyz

Java: String.join(",", items)
来源：http://xwv.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://vrj.yanxiufei.cn

Ruby: items.join(",")
来源：http://ufu.jqgfzy.top

C#:   string.Join(",", items)
来源：http://oqw.ybcxt.top

[E09] 去除所有空白字符
来源：http://ytj.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lwa.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ext.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://svw.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://mql.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://gvh.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ovt.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://rze.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cbd.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://kvb.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ckx.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yvi.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://tlt.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://wrq.hcnkem.com

Java: String.format("%03d", 7)
来源：http://yao.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qch.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ndd.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ilj.gzhubu.top

[E11] 反转字符串
来源：http://ofk.jinqigufen.top

Py:   s[::-1]
来源：http://mpj.ivvv.top

PHP:  strrev($s);
来源：http://dnw.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://fpc.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://xnc.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cvs.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lcu.hywenlv.cn

Ruby: s.reverse
来源：http://rcu.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://kcd.uphjek.com

[E12] 统计某字符出现次数
来源：http://hvv.fanxiaobao.xyz

Py:   s.count("a")
来源：http://fkl.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://var.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://brk.52xcode.cn

TS:   s.split("a").length - 1
来源：http://dlq.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gwp.cheryme.top

Go:   strings.Count(s, "a")
来源：http://slw.xinyue.icu

Ruby: s.count("a")
来源：http://fdp.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://wqh.dianchejie.cn

[E13] 逐字符遍历
来源：http://zpw.yj202588.top

Py:   for ch in s: print(ch)
来源：http://vom.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://khu.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://gnb.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://zag.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://keg.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://naw.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nrj.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evi.xuanzx.com

[E14] URL 编码与 Base64
来源：http://qvv.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cbq.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gia.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://myc.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swd.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttd.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://knc.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xvs.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rzm.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://nax.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bhv.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iba.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sgw.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pwk.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vph.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hpx.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wzo.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kcn.redwolf501.top

[E16] 数字千分位
来源：http://gpa.yvedp.cn

Py:   f"{1234567:,}"
来源：http://vzr.vehdjk.com


<!-- 参考信息 -->