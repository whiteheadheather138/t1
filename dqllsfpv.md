代发 wailian999

[D07] 切片 / 取子数组
来源：http://ymh.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hym.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ahw.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://knz.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://yma.316326.xyz

Java: list.subList(1, 4);
来源：http://yrj.dashuyun.cn

Go:   arr[1:4]
来源：http://wfw.iojbl.cn

Ruby: arr[1, 3]
来源：http://fhg.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://xnd.9152youxi.cn

[D08] 合并两个数组
来源：http://mjz.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://onu.hammf.cn

PHP:  array_merge($a, $b);
来源：http://ybo.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ayv.gogol.net.cn

TS:   [...a, ...b];
来源：http://pko.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hpr.ppjwa.cn

Go:   append(a, b...)
来源：http://ewc.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://bjn.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://osb.uphjek.com

[D09] 排序（升序）
来源：http://jzw.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://adm.fehbvm.com

PHP:  sort($arr);
来源：http://uaf.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qjq.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nsu.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://spt.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hkh.jianghu66.top

Ruby: arr.sort
来源：http://hmv.c1oappe.top

C#:   list.Sort();
来源：http://dvz.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wfb.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://beg.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqa.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rdl.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ugc.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pwf.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wna.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sbj.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://apc.hammf.cn

[D11] 反转数组
来源：http://hug.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://rpb.yuxming.cn

PHP:  array_reverse($arr);
来源：http://mtg.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://brd.bjfxy.top

TS:   [...arr].reverse();
来源：http://wgd.cheryme.top

Java: Collections.reverse(list);
来源：http://vke.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://ihu.ctjpmb.com

Ruby: arr.reverse
来源：http://ltw.haohaochexian.top

C#:   list.Reverse();
来源：http://ael.quarkkingdee.top

[D12] 查找元素下标
来源：http://nfu.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://yia.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://prl.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nky.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfq.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hhs.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://acu.yuxming.cn

Ruby: arr.index(x)
来源：http://cpq.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://wqf.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://tww.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wjw.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rhg.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://diu.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://adm.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tey.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lxh.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://vcb.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://iux.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://hvd.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fig.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jlq.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://ffp.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://qwk.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wva.tian-w.cn

Go:   // 手写循环
来源：http://myz.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://zbs.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qxr.sweek.top

[D15] 去重
来源：http://hhr.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hhd.zdbjq.cn

PHP:  array_unique($arr);
来源：http://fuj.shuidangran.top

JS:   [...new Set(arr)]
来源：http://bqr.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://qqh.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rlp.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wpd.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://ver.yonumen.top

C#:   list.Distinct().ToList()
来源：http://kiw.shangyingyoupin.top

[D16] 求和与平均值
来源：http://hfd.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdk.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://odq.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rnh.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qty.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urk.hysaishi.cn

Go:   // 手写循环累加
来源：http://nlu.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://glk.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://okn.ybcxt.top

[D17] 最大值与最小值
来源：http://dju.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://owf.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://hhe.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bpl.hysaishi.cn

TS:   Math.max(...arr);
来源：http://gvt.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://omk.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nkg.meibo888.top

Ruby: arr.max;  arr.min
来源：http://iwt.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://rek.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://lhb.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tmv.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://yil.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pnb.tanke756.top

TS:   nested.flat();
来源：http://fkk.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lwm.316326.xyz

Go:   // 手写双层循环
来源：http://qiq.nwbrower.top

Ruby: nested.flatten
来源：http://ads.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://glq.sjlbkw.cn

[D19] 按字段分组
来源：http://ejs.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rrj.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qnp.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lih.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ckw.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggp.ivvv.top

Go:   // 手写 map[string][]T
来源：http://hps.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ngq.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wry.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://pli.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://sbg.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://vxi.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khv.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gef.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ave.xuanzx.com

Go:   // 手写 map[T]int
来源：http://htu.jinqigufen.top

Ruby: arr.tally
来源：http://mee.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lcn.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://kyx.dianchejie.cn

Py:   x in arr
来源：http://hvp.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://kca.316326.xyz

JS:   arr.includes(x)
来源：http://uux.jinqigufen.top

TS:   arr.includes(x)
来源：http://sux.hnqzz.top

Java: list.contains(x)
来源：http://bke.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://csc.nwbrower.top

Ruby: arr.include?(x)
来源：http://fht.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://dlr.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://eds.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rgs.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bfo.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tci.hnxiangtu.top

TS:   [...arr];
来源：http://sat.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://bkn.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://otl.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://kpo.uphjek.com

C#:   new List<int>(list);
来源：http://zkk.gzhubu.top

[D23] reduce 累积计算
来源：http://thv.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wpk.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qnx.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fen.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iep.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fkr.52xcode.cn

Go:   // 手写循环
来源：http://ipc.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kcp.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cip.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://evo.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://smf.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://stl.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skd.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lft.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bcs.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxk.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zsf.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uew.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://rrd.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uoo.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pmg.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qcm.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sle.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://msi.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wqa.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bef.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eia.kuanghao11.cn

[D26] 数组转字符串
来源：http://kkq.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://zbz.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://ysu.sweek.top

JS:   arr.join(", ")
来源：http://wwc.zycfv.cn

TS:   arr.join(", ")
来源：http://hoa.ctjpmb.com

Java: String.join(", ", list)
来源：http://vfq.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://jtc.tianlin.xyz

Ruby: arr.join(", ")
来源：http://vap.shuidangran.top

C#:   string.Join(", ", list)
来源：http://drk.andypj.xyz

================================================================================
来源：http://sos.fzhhl.top

E. 字符串处理
来源：http://vzk.epnwcf.com

================================================================================
来源：http://wdc.iojbl.cn

[E01] 拼接字符串
来源：http://bge.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gti.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nrs.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmq.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzs.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bsc.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://brp.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ldp.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://faa.kuanghao11.cn

[E02] 重复字符串
来源：http://rlw.mhx1999.top

Py:   "ab" * 3
来源：http://zyh.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://bjd.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://llt.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://mnh.ehwqpu.com

Java: "ab".repeat(3)
来源：http://fcr.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://siv.tian-w.cn

Ruby: "ab" * 3
来源：http://cyi.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uuz.fktsv.cn

[E03] 截取子串
来源：http://vgo.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ysq.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iel.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://swk.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://cfe.sufxvd.cn

Java: s.substring(1, 4)
来源：http://rfc.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dow.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://ceu.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://jlj.xylfe.cn

[E04] 查找子串位置
来源：http://ymn.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://poj.ybcxt.top

PHP:  strpos($s, "x");
来源：http://nbg.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sii.ctjpmb.com

TS:   s.indexOf("x")
来源：http://udi.yvedp.cn

Java: s.indexOf("x")
来源：http://ara.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://cxj.yvedp.cn

Ruby: s.index("x")
来源：http://nfb.ydzc1.top

C#:   s.IndexOf("x")
来源：http://eyd.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://abn.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pkf.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mak.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffi.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tkg.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gdg.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aii.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lmu.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kcj.sysykeji.top

[E06] 替换子串
来源：http://omd.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xkp.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://cnq.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uxy.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://vhy.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ife.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://trc.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tih.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://wop.andypj.xyz

[E07] 按分隔符拆分
来源：http://xxh.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jxg.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wtd.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://big.sysykeji.top

TS:   s.split(",")
来源：http://esx.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pav.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dag.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://jin.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ozj.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://cgf.havefunace.top

Py:   ",".join(items)
来源：http://qok.tanke756.top

PHP:  implode(",", $items);
来源：http://dcw.redwolf501.top

JS:   items.join(",")
来源：http://olr.xylfe.cn

TS:   items.join(",")
来源：http://wlm.cdnleiting.top

Java: String.join(",", items)
来源：http://zqn.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://dwu.mhx1999.top

Ruby: items.join(",")
来源：http://zdg.fehbvm.com

C#:   string.Join(",", items)
来源：http://shm.cashguo.top

[E09] 去除所有空白字符
来源：http://etj.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hzo.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbi.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://zqu.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://edn.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://emr.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://atf.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eri.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://los.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://qcm.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zog.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rpa.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://esn.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://djt.gzhubu.top

Java: String.format("%03d", 7)
来源：http://spo.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://kij.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nwa.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://saq.nanxinkj.top

[E11] 反转字符串
来源：http://xug.gotoacloud.top

Py:   s[::-1]
来源：http://tbt.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://mlf.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://nku.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://wue.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cvw.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lmw.sjlbkw.cn

Ruby: s.reverse
来源：http://nox.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://hjf.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://qyv.xuetiantiany.cn

Py:   s.count("a")
来源：http://wyt.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://qui.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://lrx.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://cud.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ytx.316326.xyz

Go:   strings.Count(s, "a")
来源：http://pyo.zhoulong.xyz

Ruby: s.count("a")
来源：http://jpn.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://aqq.jlsjyb.cn

[E13] 逐字符遍历
来源：http://nab.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://bip.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hrt.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jlx.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lkm.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ayr.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mht.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nal.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dgo.zhixingplan.top


<!-- 参考信息 -->