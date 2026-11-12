代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://qcp.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kqx.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sre.ywan-chungtsiang.top

[D06] 数组长度
来源：http://rkn.yonumen.top

Py:   len(arr)
来源：http://rlm.hongshengwenyu.top

PHP:  count($arr);
来源：http://udi.fengsongda.top

JS:   arr.length
来源：http://zbq.ehwqpu.com

TS:   arr.length
来源：http://enk.jiagoushi.top

Java: list.size();
来源：http://tda.xuanzx.com

Go:   len(arr)
来源：http://ref.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://nfw.kuanghao11.cn

C#:   list.Count;
来源：http://voj.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://mpp.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qrt.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://qok.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://krp.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://nwg.nwbrower.top

Java: list.subList(1, 4);
来源：http://vck.yonumen.top

Go:   arr[1:4]
来源：http://wpg.pycfn.com

Ruby: arr[1, 3]
来源：http://coz.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://agy.hcnkem.com

[D08] 合并两个数组
来源：http://fti.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://zaf.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://arq.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gne.yongpay.top

TS:   [...a, ...b];
来源：http://hxx.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yyn.zdbjq.cn

Go:   append(a, b...)
来源：http://brj.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://ozc.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://rat.pengpengdd.cyou

[D09] 排序（升序）
来源：http://dsg.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://hde.yuanzhike.top

PHP:  sort($arr);
来源：http://ihn.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cnv.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bxn.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ref.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qll.yuxming.cn

Ruby: arr.sort
来源：http://kpp.havefunace.top

C#:   list.Sort();
来源：http://hie.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yht.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zyc.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xcr.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dtm.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bdt.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wsp.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nma.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zbz.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wgh.bbcook.cn

[D11] 反转数组
来源：http://heo.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://lqf.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://cyb.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pzh.yj202588.top

TS:   [...arr].reverse();
来源：http://nkq.jinqigufen.top

Java: Collections.reverse(list);
来源：http://hmf.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://ubw.yj202588.top

Ruby: arr.reverse
来源：http://pgi.daxiang520.top

C#:   list.Reverse();
来源：http://iiz.yuanzhike.top

[D12] 查找元素下标
来源：http://syw.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://dbm.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dgs.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qlt.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://awv.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vuu.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://rhw.aizwys.cn

Ruby: arr.index(x)
来源：http://jlt.vehdjk.com

C#:   list.IndexOf(x);
来源：http://cey.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://tjg.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ebn.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ara.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://ivd.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://qim.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cgv.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://akr.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://iod.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://afw.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://nst.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uak.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://itj.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://jsq.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://fxu.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://qie.daria6918.cn

Go:   // 手写循环
来源：http://muk.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://kmb.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iuf.guowangkeji.top

[D15] 去重
来源：http://why.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hkz.nwbrower.top

PHP:  array_unique($arr);
来源：http://ttr.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://jng.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://xik.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://znq.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wjh.fzhhl.top

Ruby: arr.uniq
来源：http://yfm.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://lhe.pengpengdd.cyou

[D16] 求和与平均值
来源：http://eza.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lfk.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hcj.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tqt.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fub.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zir.c1oappe.top

Go:   // 手写循环累加
来源：http://kil.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dza.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://xlz.guowangkeji.top

[D17] 最大值与最小值
来源：http://vfr.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://gqi.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://cwr.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mrq.xziqi.cn

TS:   Math.max(...arr);
来源：http://aui.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://but.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ohm.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://yic.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://wvd.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://fss.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mjg.birdmap.top

PHP:  array_merge(...$nested);
来源：http://jhc.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bad.snrcjt.cn

TS:   nested.flat();
来源：http://vid.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jdn.aibaodan.cn

Go:   // 手写双层循环
来源：http://pfs.jqgfzy.top

Ruby: nested.flatten
来源：http://dfg.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xya.vqdsnc.cn

[D19] 按字段分组
来源：http://exf.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vvc.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bss.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://poo.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://psh.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kvf.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://ysz.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnb.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unk.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://ery.ivvv.top

Py:   Counter(arr)
来源：http://vkt.316326.xyz

PHP:  array_count_values($arr);
来源：http://mzh.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nok.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mub.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wuo.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://szs.epnwcf.com

Ruby: arr.tally
来源：http://yih.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsh.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://dob.yangfankeji.com

Py:   x in arr
来源：http://mqj.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://ttr.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://bet.svipenyu.cn

TS:   arr.includes(x)
来源：http://kws.cheryme.top

Java: list.contains(x)
来源：http://zxa.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://hnt.sweek.top

Ruby: arr.include?(x)
来源：http://iny.sjlbkw.cn

C#:   list.Contains(x)
来源：http://uwc.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://rsd.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hiy.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ivj.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fbt.zdbjq.cn

TS:   [...arr];
来源：http://igx.jianghu66.top

Java: new ArrayList<>(list);
来源：http://bxl.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://sdg.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://agu.jinqigufen.top

C#:   new List<int>(list);
来源：http://zuq.smart0.xyz

[D23] reduce 累积计算
来源：http://yyi.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sda.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zqu.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://avx.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvo.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yrp.hysaishi.cn

Go:   // 手写循环
来源：http://wke.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://log.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rsc.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://fto.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ugv.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mip.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hgd.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gac.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://row.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://urf.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://daf.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aoz.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://upl.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mau.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://las.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aub.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://agr.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ten.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://azb.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mor.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ccs.guannengcc.top

[D26] 数组转字符串
来源：http://bhn.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://vrv.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://uly.xuanzx.com

JS:   arr.join(", ")
来源：http://eyg.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://crs.zhijiandao.cn

Java: String.join(", ", list)
来源：http://yvt.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://ymt.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://gll.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://okj.zhaomingkeji.xyz

================================================================================
来源：http://dwa.cheryme.top

E. 字符串处理
来源：http://hfd.0kj1m.cn

================================================================================
来源：http://joo.chenlongwang.top

[E01] 拼接字符串
来源：http://csy.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pvu.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://akk.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfa.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzl.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fgy.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://riv.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tcw.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sbq.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://xnl.jinqigfzy.top

Py:   "ab" * 3
来源：http://mwo.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://arb.aizwys.cn

JS:   "ab".repeat(3)
来源：http://huo.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://mbe.yj202588.top

Java: "ab".repeat(3)
来源：http://jps.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://hcq.svipenyu.cn

Ruby: "ab" * 3
来源：http://dkc.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddi.yangfankeji.com

[E03] 截取子串
来源：http://ycr.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jwv.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nol.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvc.sysykeji.top

TS:   s.slice(1, 4)
来源：http://drw.yj202588.top

Java: s.substring(1, 4)
来源：http://mei.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://atu.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://xww.yj202588.top

C#:   s.Substring(1, 3)
来源：http://kxm.birdmap.top

[E04] 查找子串位置
来源：http://jpw.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://skn.bbcook.cn

PHP:  strpos($s, "x");
来源：http://xjr.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kqm.daxiang520.top

TS:   s.indexOf("x")
来源：http://itn.jqgfzy.top

Java: s.indexOf("x")
来源：http://lgg.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://upl.fktsv.cn

Ruby: s.index("x")
来源：http://xfl.yonumen.top

C#:   s.IndexOf("x")
来源：http://xku.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ibw.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://phg.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owu.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqb.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dmw.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgx.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ihx.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mwm.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hcr.zhaomingkeji.xyz

[E06] 替换子串
来源：http://jyo.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pry.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://ppc.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pab.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://bph.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lay.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wqx.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gck.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://xbw.9152youxi.cn

[E07] 按分隔符拆分
来源：http://hld.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kds.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kvj.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://agb.nwbrower.top

TS:   s.split(",")
来源：http://rgb.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://mjs.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zvf.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://pxr.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmw.xinyue.icu

[E08] 数组按分隔符合并
来源：http://qzq.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://lje.daria6918.cn

PHP:  implode(",", $items);
来源：http://imk.xylfe.cn

JS:   items.join(",")
来源：http://bwi.xuetiantiany.cn

TS:   items.join(",")
来源：http://nax.fengsongda.top

Java: String.join(",", items)
来源：http://wmg.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://odl.zhiwuduotai.top

Ruby: items.join(",")
来源：http://jyg.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://win.cqqwz.cn

[E09] 去除所有空白字符
来源：http://xnf.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oqz.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yqp.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://uco.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ico.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://req.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ljl.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bwj.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqu.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://bsa.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://slk.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsc.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://zhf.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://mlk.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://ksj.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://rew.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://igl.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://enn.xuanzx.com

[E11] 反转字符串
来源：http://adl.hesvh.cn

Py:   s[::-1]
来源：http://fqe.vehdjk.com

PHP:  strrev($s);
来源：http://plv.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://uqv.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://qdx.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tyw.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://emo.sxryk.cn

Ruby: s.reverse
来源：http://dgl.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hci.daria6918.cn

[E12] 统计某字符出现次数
来源：http://wxp.daria6918.cn

Py:   s.count("a")
来源：http://mhj.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://fgl.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://jzz.fzhhl.top

TS:   s.split("a").length - 1
来源：http://uqq.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ent.hesvh.cn


<!-- 参考信息 -->