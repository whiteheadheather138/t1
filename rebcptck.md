代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hcg.feifeiyinyue.top

[D08] 合并两个数组
来源：http://fgk.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://vbd.cheryme.top

PHP:  array_merge($a, $b);
来源：http://zgb.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://rxl.iojbl.cn

TS:   [...a, ...b];
来源：http://rvi.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://toj.xuanzx.com

Go:   append(a, b...)
来源：http://nau.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://zxs.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://nrh.gotoacloud.top

[D09] 排序（升序）
来源：http://etl.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xvz.fktsv.cn

PHP:  sort($arr);
来源：http://pvg.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ocn.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://quq.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aaa.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://inb.ppjwa.cn

Ruby: arr.sort
来源：http://vzy.ehwqpu.com

C#:   list.Sort();
来源：http://qsk.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lns.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://znp.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iti.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yyi.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://now.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ddd.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oaz.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dui.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hsw.xziqi.cn

[D11] 反转数组
来源：http://fxt.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://ojv.yfazqb.com

PHP:  array_reverse($arr);
来源：http://gme.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zra.zdbjq.cn

TS:   [...arr].reverse();
来源：http://xio.aibaodan.cn

Java: Collections.reverse(list);
来源：http://eih.meibo888.top

Go:   slices.Reverse(arr)
来源：http://vdp.gotoacloud.top

Ruby: arr.reverse
来源：http://trn.hongshengwenyu.top

C#:   list.Reverse();
来源：http://dqk.aizwys.cn

[D12] 查找元素下标
来源：http://ygd.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://zvx.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rts.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fim.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tbx.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://erg.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://lmt.ydzc1.top

Ruby: arr.index(x)
来源：http://ifg.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://eqr.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://qkf.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ujz.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzl.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://vfd.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://zsb.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wpb.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ycp.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://dmb.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ljp.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://lnf.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pow.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cba.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://ljo.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://uxk.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://znw.zhijiandao.cn

Go:   // 手写循环
来源：http://xye.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://fzu.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://alf.xingfuxueyuan.xyz

[D15] 去重
来源：http://gpp.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kam.uphjek.com

PHP:  array_unique($arr);
来源：http://ljd.tanke756.top

JS:   [...new Set(arr)]
来源：http://thr.hcnkem.com

TS:   [...new Set(arr)]
来源：http://soi.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jwf.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://xxt.cdnleiting.top

Ruby: arr.uniq
来源：http://qjh.sweek.top

C#:   list.Distinct().ToList()
来源：http://hcl.jqgufenzy.top

[D16] 求和与平均值
来源：http://qzf.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ece.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nrh.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rrf.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvh.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ira.yuanzhike.top

Go:   // 手写循环累加
来源：http://icj.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ykz.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://jzi.fehbvm.com

[D17] 最大值与最小值
来源：http://yez.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://jqp.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://noa.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gzi.sufxvd.cn

TS:   Math.max(...arr);
来源：http://dll.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pgw.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dua.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://url.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://icu.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://xye.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://obk.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://lte.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hcc.aibaodan.cn

TS:   nested.flat();
来源：http://dkr.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vjp.jlsjyb.cn

Go:   // 手写双层循环
来源：http://spn.daria6918.cn

Ruby: nested.flatten
来源：http://xcg.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wpj.ydzc1.top

[D19] 按字段分组
来源：http://jeb.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://loy.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kaq.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vei.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lzk.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ltq.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://ntc.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyt.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npl.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://rru.jinqigufen.top

Py:   Counter(arr)
来源：http://gpl.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://gjh.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qlp.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhv.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://htd.smart0.xyz

Go:   // 手写 map[T]int
来源：http://fmg.fktsv.cn

Ruby: arr.tally
来源：http://ott.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qjg.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://dgf.wangdashe.top

Py:   x in arr
来源：http://vzo.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://fzj.daxiang520.top

JS:   arr.includes(x)
来源：http://jrd.yfazqb.com

TS:   arr.includes(x)
来源：http://zzv.9152youxi.cn

Java: list.contains(x)
来源：http://ruh.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://wki.epnwcf.com

Ruby: arr.include?(x)
来源：http://cuf.sufxvd.cn

C#:   list.Contains(x)
来源：http://ysx.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://ssf.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fwb.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xbc.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dzg.fengsongda.top

TS:   [...arr];
来源：http://dvk.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://jkm.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://pod.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://bxp.uphjek.com

C#:   new List<int>(list);
来源：http://hmj.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://pgh.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://idx.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lji.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrv.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lza.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyi.cheryme.top

Go:   // 手写循环
来源：http://yuc.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xvp.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hnr.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://kvv.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wux.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://knl.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jxp.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hnc.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zwe.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rec.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ioz.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yhq.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://xbh.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rmk.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tdk.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dex.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijk.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebe.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://maf.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yhr.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tsd.svipenyu.cn

[D26] 数组转字符串
来源：http://ewq.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://edr.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://qsy.hcnkem.com

JS:   arr.join(", ")
来源：http://xsh.svipenyu.cn

TS:   arr.join(", ")
来源：http://rcq.quarkkingdee.top

Java: String.join(", ", list)
来源：http://nhh.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://ygy.ydzc1.top

Ruby: arr.join(", ")
来源：http://pkb.iojbl.cn

C#:   string.Join(", ", list)
来源：http://reb.yj20258.top

================================================================================
来源：http://gwq.hongshengwenyu.top

E. 字符串处理
来源：http://fnf.hysaishi.cn

================================================================================
来源：http://knj.gogol.net.cn

[E01] 拼接字符串
来源：http://zve.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://txy.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fuo.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://koh.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixb.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cns.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pvl.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wkz.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mkb.jyoumei.cn

[E02] 重复字符串
来源：http://thl.ctjpmb.com

Py:   "ab" * 3
来源：http://ahl.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://vrr.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://qjv.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://cpy.yvedp.cn

Java: "ab".repeat(3)
来源：http://hgx.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://vla.chenlongwang.top

Ruby: "ab" * 3
来源：http://ccg.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dir.hammf.cn

[E03] 截取子串
来源：http://ypv.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://otb.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://czg.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kgi.yonumen.top

TS:   s.slice(1, 4)
来源：http://qsf.yangfankeji.com

Java: s.substring(1, 4)
来源：http://deh.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://msy.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tym.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://zje.tanke756.top

[E04] 查找子串位置
来源：http://ncd.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://thm.fengsongda.top

PHP:  strpos($s, "x");
来源：http://snw.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nat.fehbvm.com

TS:   s.indexOf("x")
来源：http://gyl.dashuyun.cn

Java: s.indexOf("x")
来源：http://mns.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://kba.yj20258888.top

Ruby: s.index("x")
来源：http://tip.hammf.cn

C#:   s.IndexOf("x")
来源：http://wfl.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://szb.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hfr.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://alx.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nlh.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpy.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lrd.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qip.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jqd.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ejb.52xcode.cn

[E06] 替换子串
来源：http://tlq.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nxa.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://nox.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://opo.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://vib.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bgb.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oks.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmq.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://fzm.redwolf501.top

[E07] 按分隔符拆分
来源：http://vmv.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ooy.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://srw.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lkp.pengpengdd.cyou

TS:   s.split(",")
来源：http://epk.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hbo.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qyw.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://tmc.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lfc.yonumen.top

[E08] 数组按分隔符合并
来源：http://xwa.yuanzhike.top

Py:   ",".join(items)
来源：http://aus.zdbjq.cn

PHP:  implode(",", $items);
来源：http://pmp.hesvh.cn

JS:   items.join(",")
来源：http://jlh.c1oappe.top

TS:   items.join(",")
来源：http://xmm.c1oappe.top

Java: String.join(",", items)
来源：http://cjr.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://ype.wangshuangyany.cn

Ruby: items.join(",")
来源：http://zqc.yj20258.top

C#:   string.Join(",", items)
来源：http://vjp.316326.xyz

[E09] 去除所有空白字符
来源：http://sab.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fch.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qsr.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://xuk.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://hpl.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://ksm.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ajc.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kzb.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://itd.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://zoh.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kmm.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://peh.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://bie.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://jyw.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://cmn.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fxc.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cyl.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://myg.nanxinkj.top

[E11] 反转字符串
来源：http://unf.jqgufenzy.top

Py:   s[::-1]
来源：http://dpn.xylfe.cn

PHP:  strrev($s);
来源：http://spq.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://iiz.cashguo.top

TS:   [...s].reverse().join("")
来源：http://raz.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dll.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rmx.zhiwuduotai.top

Ruby: s.reverse
来源：http://soh.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://xga.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://azk.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://dyf.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://dcz.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://cep.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://cqy.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://efq.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://igz.gzhubu.top

Ruby: s.count("a")
来源：http://nsm.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://cww.yfazqb.com

[E13] 逐字符遍历
来源：http://kmh.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://pmb.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmx.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cog.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xmd.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bpu.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hex.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xos.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wxr.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://cvn.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sxl.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xri.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://miu.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qqk.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hia.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://abi.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mtf.yuxming.cn


<!-- 参考信息 -->