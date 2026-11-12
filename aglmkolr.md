代发 wailian999

[D07] 切片 / 取子数组
来源：http://xos.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ehz.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://bjq.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://cdf.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://syy.yj20258888.top

Java: list.subList(1, 4);
来源：http://wns.smart0.xyz

Go:   arr[1:4]
来源：http://jlq.yuxming.cn

Ruby: arr[1, 3]
来源：http://ydz.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://ggo.aizwys.cn

[D08] 合并两个数组
来源：http://jzc.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://enj.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://xhh.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://eri.cqqwz.cn

TS:   [...a, ...b];
来源：http://wda.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yoz.sufxvd.cn

Go:   append(a, b...)
来源：http://lxt.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://dre.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://pjg.zdbjq.cn

[D09] 排序（升序）
来源：http://pul.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://vai.vqdsnc.cn

PHP:  sort($arr);
来源：http://dxk.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwk.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cue.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jka.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hut.yj202588.top

Ruby: arr.sort
来源：http://tvs.hnqzz.top

C#:   list.Sort();
来源：http://wvq.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cxu.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uey.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcd.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lce.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://alp.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mbm.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yyf.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pho.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tjy.yongpay.top

[D11] 反转数组
来源：http://gfz.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://qfz.fzhhl.top

PHP:  array_reverse($arr);
来源：http://rol.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jss.cashguo.top

TS:   [...arr].reverse();
来源：http://ilz.fengsongda.top

Java: Collections.reverse(list);
来源：http://ovn.ivvv.top

Go:   slices.Reverse(arr)
来源：http://zdl.guowangkeji.top

Ruby: arr.reverse
来源：http://aop.sufxvd.cn

C#:   list.Reverse();
来源：http://etc.hysaishi.cn

[D12] 查找元素下标
来源：http://xbi.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://kww.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vkz.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ylw.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqk.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dpn.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://mdv.xinyue.icu

Ruby: arr.index(x)
来源：http://hlb.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://rwn.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://ohw.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oub.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://puv.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://asq.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://hmr.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ken.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gnp.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lup.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dwg.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://mup.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wxt.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cqy.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://xit.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://yoj.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dux.bbcook.cn

Go:   // 手写循环
来源：http://mzy.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uwy.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bjc.pengpengdd.cyou

[D15] 去重
来源：http://vjc.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mae.chenzaomai.com

PHP:  array_unique($arr);
来源：http://dev.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://eaa.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://msd.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mzt.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://gpi.guowangkeji.top

Ruby: arr.uniq
来源：http://bbm.yj20258.top

C#:   list.Distinct().ToList()
来源：http://iwj.havefunace.top

[D16] 求和与平均值
来源：http://vtt.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lwp.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hrd.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fit.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvp.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wro.havefunace.top

Go:   // 手写循环累加
来源：http://nwh.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://puq.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://sep.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://wwr.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://tsy.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://kky.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sdv.316326.xyz

TS:   Math.max(...arr);
来源：http://jjt.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://isf.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://smt.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://hoy.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://hoc.hammf.cn

[D18] 扁平化嵌套数组
来源：http://yus.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lrv.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://nox.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://afz.fengsongda.top

TS:   nested.flat();
来源：http://hny.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ugr.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://tqf.bbcook.cn

Ruby: nested.flatten
来源：http://rdq.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://evn.wangshuangyany.cn

[D19] 按字段分组
来源：http://jup.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jjj.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kkb.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ezg.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qpx.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mgo.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://huk.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpk.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umz.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://fua.tian-w.cn

Py:   Counter(arr)
来源：http://dit.hammf.cn

PHP:  array_count_values($arr);
来源：http://hbn.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmc.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kxy.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://frr.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://rgc.yfazqb.com

Ruby: arr.tally
来源：http://oug.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eur.cheryme.top

[D21] 判断是否包含某元素
来源：http://uii.sxryk.cn

Py:   x in arr
来源：http://ezo.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://kpb.svipenyu.cn

JS:   arr.includes(x)
来源：http://ndm.guannengcc.top

TS:   arr.includes(x)
来源：http://wna.yj20258888.top

Java: list.contains(x)
来源：http://wtv.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://qve.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://tle.ehwqpu.com

C#:   list.Contains(x)
来源：http://hks.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://jza.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ciq.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wng.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edi.cheryme.top

TS:   [...arr];
来源：http://uzz.birdmap.top

Java: new ArrayList<>(list);
来源：http://lox.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lgv.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://ocr.daxiang520.top

C#:   new List<int>(list);
来源：http://iun.yongpay.top

[D23] reduce 累积计算
来源：http://hxb.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tfw.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://onv.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://din.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xlx.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iin.yj202588.top

Go:   // 手写循环
来源：http://fam.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jml.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yei.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://qlt.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ppj.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wmn.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fbh.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bfs.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hwy.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cfj.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bgv.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://obt.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://qis.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iyy.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vsw.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mmz.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hin.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iyb.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvs.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pgm.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nic.ybcxt.top

[D26] 数组转字符串
来源：http://viy.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://phb.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://hcp.9152youxi.cn

JS:   arr.join(", ")
来源：http://kxs.gogol.net.cn

TS:   arr.join(", ")
来源：http://emr.0kj1m.cn

Java: String.join(", ", list)
来源：http://flv.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://pxg.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://qmx.aizwys.cn

C#:   string.Join(", ", list)
来源：http://hmo.shzxlz.cn

================================================================================
来源：http://lik.daria6918.cn

E. 字符串处理
来源：http://ves.cheryme.top

================================================================================
来源：http://cgz.xuetiantiany.cn

[E01] 拼接字符串
来源：http://mfx.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nlj.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gou.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://udt.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eua.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tmd.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mww.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tnu.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fnc.tanke756.top

[E02] 重复字符串
来源：http://xbn.xylfe.cn

Py:   "ab" * 3
来源：http://zff.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://ice.cheryme.top

JS:   "ab".repeat(3)
来源：http://baj.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://whb.yj20258888.top

Java: "ab".repeat(3)
来源：http://phg.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://kul.bjfxy.top

Ruby: "ab" * 3
来源：http://hzv.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qwa.hesvh.cn

[E03] 截取子串
来源：http://sjj.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gaf.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fii.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wav.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://gqm.jinqigufen.top

Java: s.substring(1, 4)
来源：http://akf.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qso.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://ebv.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://wfm.ydzc1.top

[E04] 查找子串位置
来源：http://udx.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://pmi.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://hnw.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oaj.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://evs.fzhhl.top

Java: s.indexOf("x")
来源：http://nsi.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://gwv.dashuyun.cn

Ruby: s.index("x")
来源：http://ocw.sweek.top

C#:   s.IndexOf("x")
来源：http://xjf.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvy.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqe.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fhb.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bjp.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ham.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pgw.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://skq.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mai.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dck.yfazqb.com

[E06] 替换子串
来源：http://mch.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bxl.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://moa.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idv.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://zqu.mhx1999.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aui.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzo.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pff.tarul.cn

C#:   s.Replace("a", "b")
来源：http://clm.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://tnf.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dgm.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://occ.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://dxg.aizwys.cn

TS:   s.split(",")
来源：http://ueq.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://yzd.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aqb.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://ogu.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pnx.yuxming.cn

[E08] 数组按分隔符合并
来源：http://vfr.yueranfly.top

Py:   ",".join(items)
来源：http://bzp.tarul.cn

PHP:  implode(",", $items);
来源：http://vsg.sysykeji.top

JS:   items.join(",")
来源：http://xaj.svipenyu.cn

TS:   items.join(",")
来源：http://nnp.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://aby.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://juf.svipenyu.cn

Ruby: items.join(",")
来源：http://xsj.hysaishi.cn

C#:   string.Join(",", items)
来源：http://hbo.hysaishi.cn

[E09] 去除所有空白字符
来源：http://fbc.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ini.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nbg.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://tki.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://dwh.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://qaz.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxl.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://vxe.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmg.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://ufq.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nzt.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zvk.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://vlo.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://fql.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://rel.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftc.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esf.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejr.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://ebf.zhixingplan.top

Py:   s[::-1]
来源：http://idl.hammf.cn

PHP:  strrev($s);
来源：http://wfc.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://pmk.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://eyl.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xlh.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zck.xuetiantiany.cn

Ruby: s.reverse
来源：http://muq.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://pgm.yongpay.top

[E12] 统计某字符出现次数
来源：http://ncc.xinyue.icu

Py:   s.count("a")
来源：http://nbk.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://alk.sweek.top

JS:   s.split("a").length - 1
来源：http://ewy.wangdashe.top

TS:   s.split("a").length - 1
来源：http://ftu.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yrd.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://nim.kuanghao11.cn

Ruby: s.count("a")
来源：http://oif.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://rjk.yj20258.top

[E13] 逐字符遍历
来源：http://zkc.havefunace.top

Py:   for ch in s: print(ch)
来源：http://fhb.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hxt.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://scv.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://edr.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://meu.gzhubu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qgd.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://fzs.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gir.birdmap.top


<!-- 参考信息 -->