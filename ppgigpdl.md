代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://adq.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://ohf.hammf.cn

[D09] 排序（升序）
来源：http://yvi.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://xzq.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://upb.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://piq.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gje.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eaw.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qzj.0kj1m.cn

Ruby: arr.sort
来源：http://zfl.hfpthk.cn

C#:   list.Sort();
来源：http://eur.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bbd.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wbt.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zpa.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mba.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mzm.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjb.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbv.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://olr.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eyf.yanxiufei.cn

[D11] 反转数组
来源：http://qhc.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://hai.xuanzx.com

PHP:  array_reverse($arr);
来源：http://wkl.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://exw.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://ejx.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://dwt.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://tqm.smart0.xyz

Ruby: arr.reverse
来源：http://nbt.yongpay.top

C#:   list.Reverse();
来源：http://buw.vqdsnc.cn

[D12] 查找元素下标
来源：http://iiq.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://vjz.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrf.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bzj.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://seg.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uxj.meibo888.top

Go:   slices.Index(arr, x)
来源：http://euu.dianchejie.cn

Ruby: arr.index(x)
来源：http://qav.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://kwe.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://wwx.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://psf.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wfa.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://rib.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://wde.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uko.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wbg.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://czf.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://apr.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://hug.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hnj.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pkg.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://kfa.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://zln.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hom.yanxiufei.cn

Go:   // 手写循环
来源：http://ccg.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://gxx.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qbj.smart0.xyz

[D15] 去重
来源：http://hol.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kgn.xziqi.cn

PHP:  array_unique($arr);
来源：http://azp.hammf.cn

JS:   [...new Set(arr)]
来源：http://gto.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://wob.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pdd.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cte.316326.xyz

Ruby: arr.uniq
来源：http://myh.havefunace.top

C#:   list.Distinct().ToList()
来源：http://ill.hammf.cn

[D16] 求和与平均值
来源：http://yci.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ljq.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qyx.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mxw.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xmg.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://via.gotoacloud.top

Go:   // 手写循环累加
来源：http://ago.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvr.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://jrs.fzhhl.top

[D17] 最大值与最小值
来源：http://eyj.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://evo.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://xqx.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xee.shzxlz.cn

TS:   Math.max(...arr);
来源：http://yqb.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cwv.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uua.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://yis.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://cah.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://vcc.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rlp.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://tqr.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yhj.havefunace.top

TS:   nested.flat();
来源：http://yqq.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bvh.hcnkem.com

Go:   // 手写双层循环
来源：http://lii.ybcxt.top

Ruby: nested.flatten
来源：http://ldd.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tgv.jqgfzy.top

[D19] 按字段分组
来源：http://uun.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jrz.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://les.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cga.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://age.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zuv.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://orn.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://zdz.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://khv.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://ejg.zhijiandao.cn

Py:   Counter(arr)
来源：http://ucz.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://rzv.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvb.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cli.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uwx.fehbvm.com

Go:   // 手写 map[T]int
来源：http://xuz.yfazqb.com

Ruby: arr.tally
来源：http://ffd.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://she.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://tww.haohaochexian.top

Py:   x in arr
来源：http://kph.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://wnz.cucudq.cn

JS:   arr.includes(x)
来源：http://wjd.shzxlz.cn

TS:   arr.includes(x)
来源：http://ime.gaohongyu789.top

Java: list.contains(x)
来源：http://aoa.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://yke.ydzc1.top

Ruby: arr.include?(x)
来源：http://jik.hywenlv.cn

C#:   list.Contains(x)
来源：http://pco.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://jsj.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://stu.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qex.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fuh.cashguo.top

TS:   [...arr];
来源：http://ruw.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://chz.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sdi.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://lcf.ppjwa.cn

C#:   new List<int>(list);
来源：http://mco.vehdjk.com

[D23] reduce 累积计算
来源：http://zqc.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lwg.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gpr.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fht.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glr.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ixu.guowangkeji.top

Go:   // 手写循环
来源：http://lwu.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jup.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ivv.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://vzy.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dxs.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sqw.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tyj.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nqq.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cte.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hyt.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qhi.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tjo.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://bdj.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yue.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dya.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://prj.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zxr.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jxo.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gkg.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://htc.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cct.cashguo.top

[D26] 数组转字符串
来源：http://cff.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://prl.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://igk.yanxiufei.cn

JS:   arr.join(", ")
来源：http://rnq.xylfe.cn

TS:   arr.join(", ")
来源：http://czm.cdnleiting.top

Java: String.join(", ", list)
来源：http://cux.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://jcy.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://mhe.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://rav.fktsv.cn

================================================================================
来源：http://dbf.zhijiandao.cn

E. 字符串处理
来源：http://uze.zhengqikj.top

================================================================================
来源：http://ham.tarul.cn

[E01] 拼接字符串
来源：http://ngk.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dfd.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdb.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujn.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yhx.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eka.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://psu.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axa.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nmk.yanxiufei.cn

[E02] 重复字符串
来源：http://mqh.havefunace.top

Py:   "ab" * 3
来源：http://kpo.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://tyv.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://loj.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://knk.fzhhl.top

Java: "ab".repeat(3)
来源：http://pov.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://lxt.cdnleiting.top

Ruby: "ab" * 3
来源：http://swo.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jtt.jiagoushi.top

[E03] 截取子串
来源：http://rra.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://njt.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://izr.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://whn.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://lol.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://nja.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://umw.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wnx.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://yzz.hammf.cn

[E04] 查找子串位置
来源：http://bfu.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://ppn.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://yzj.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://glf.hysaishi.cn

TS:   s.indexOf("x")
来源：http://uvz.zhoulong.xyz

Java: s.indexOf("x")
来源：http://jia.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://afd.epnwcf.com

Ruby: s.index("x")
来源：http://lvj.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://gda.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hfe.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zmo.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xpz.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rip.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jrf.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfg.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kyc.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://drl.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xdp.jianghu66.top

[E06] 替换子串
来源：http://xje.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vak.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://zql.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ruz.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://qir.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqx.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xwf.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jre.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://siq.zdqjudy.top

[E07] 按分隔符拆分
来源：http://wer.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivi.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dyq.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lvd.shanyushiyangtech.top

TS:   s.split(",")
来源：http://rct.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://dyz.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qhq.havefunace.top

Ruby: s.split(",");  s.split
来源：http://tod.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iui.tian-w.cn

[E08] 数组按分隔符合并
来源：http://xft.yj20258.top

Py:   ",".join(items)
来源：http://von.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://qla.redwolf501.top

JS:   items.join(",")
来源：http://shx.9152youxi.cn

TS:   items.join(",")
来源：http://tmb.52xcode.cn

Java: String.join(",", items)
来源：http://ahg.ivvv.top

Go:   strings.Join(items, ",")
来源：http://pdk.mhx1999.top

Ruby: items.join(",")
来源：http://zxb.jqgfzy.top

C#:   string.Join(",", items)
来源：http://wym.iojbl.cn

[E09] 去除所有空白字符
来源：http://ikd.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zyn.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hqt.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://juf.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://mxy.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://gcu.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dsv.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fqd.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ogr.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://ipr.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fru.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wyo.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://tli.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://jyc.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://xla.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bpp.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lrs.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://max.316326.xyz

[E11] 反转字符串
来源：http://pic.jlsjyb.cn

Py:   s[::-1]
来源：http://bwc.vehdjk.com

PHP:  strrev($s);
来源：http://zue.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://hen.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://pjh.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hde.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gsi.yj20258888.top

Ruby: s.reverse
来源：http://jiv.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://opg.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://weu.jyoumei.cn

Py:   s.count("a")
来源：http://qtf.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://vis.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://wef.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://ncn.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vei.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://sot.havefunace.top

Ruby: s.count("a")
来源：http://htk.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://xga.c1oappe.top

[E13] 逐字符遍历
来源：http://mzf.yj202588.top

Py:   for ch in s: print(ch)
来源：http://scv.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zax.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bem.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvr.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://irk.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bof.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jpz.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xfj.tanke756.top

[E14] URL 编码与 Base64
来源：http://jwr.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://axz.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsy.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ysm.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xfv.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lae.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oim.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jal.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tug.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://kqd.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cnp.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://trx.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kdm.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xcs.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uks.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tzh.tian-w.cn


<!-- 参考信息 -->