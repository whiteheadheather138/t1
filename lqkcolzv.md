代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://rco.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wsd.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://szx.fehbvm.com

[D06] 数组长度
来源：http://ujs.shanyushiyangkeji.top

Py:   len(arr)
来源：http://pye.zhixingplan.top

PHP:  count($arr);
来源：http://jdy.fzhhl.top

JS:   arr.length
来源：http://sao.zhoulong.xyz

TS:   arr.length
来源：http://ejp.shanyushiyangtech.top

Java: list.size();
来源：http://qbi.jlsjyb.cn

Go:   len(arr)
来源：http://uro.yuxming.cn

Ruby: arr.length; arr.size
来源：http://bow.vehdjk.com

C#:   list.Count;
来源：http://kyl.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://tkk.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vff.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://lsf.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://ywz.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://txu.jinqigufen.top

Java: list.subList(1, 4);
来源：http://lde.meibo888.top

Go:   arr[1:4]
来源：http://vus.cqqwz.cn

Ruby: arr[1, 3]
来源：http://hwd.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://npi.smart0.xyz

[D08] 合并两个数组
来源：http://ydi.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://huo.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://yag.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://swt.ppjwa.cn

TS:   [...a, ...b];
来源：http://tqu.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mpc.haohaochexian.top

Go:   append(a, b...)
来源：http://mzn.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://ktv.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://lrd.chenjidiqi.icu

[D09] 排序（升序）
来源：http://ssb.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://yvw.jinqigfzy.top

PHP:  sort($arr);
来源：http://qtu.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://akd.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wiv.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qdl.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jym.yj20258888.top

Ruby: arr.sort
来源：http://pbb.yvedp.cn

C#:   list.Sort();
来源：http://cob.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hmk.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://phj.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eoq.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kpp.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vjn.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vek.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ajw.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://trk.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mkr.bjfxy.top

[D11] 反转数组
来源：http://anr.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://nkh.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://ctj.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://scn.ctjpmb.com

TS:   [...arr].reverse();
来源：http://cpr.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://nbd.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://fwp.cheryme.top

Ruby: arr.reverse
来源：http://yco.9152youxi.cn

C#:   list.Reverse();
来源：http://frd.jyoumei.cn

[D12] 查找元素下标
来源：http://fan.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://fhk.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nze.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gsu.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzp.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jfz.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://dli.fzhhl.top

Ruby: arr.index(x)
来源：http://vtb.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://ywx.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://iaj.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://csa.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wbs.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://zuj.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://afa.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://foe.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vjx.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ynf.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://goz.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://odt.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gyh.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fam.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://nle.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://hwt.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rbs.iojbl.cn

Go:   // 手写循环
来源：http://jix.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mzd.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jzj.tianlin.xyz

[D15] 去重
来源：http://nyi.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kfu.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://hce.fktsv.cn

JS:   [...new Set(arr)]
来源：http://bgz.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://uce.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oxn.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://aab.shuidangran.top

Ruby: arr.uniq
来源：http://ihi.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://aih.9152youxi.cn

[D16] 求和与平均值
来源：http://ulm.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ztt.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fcw.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqe.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wxw.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aic.hesvh.cn

Go:   // 手写循环累加
来源：http://twa.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ccj.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://tuq.nwbrower.top

[D17] 最大值与最小值
来源：http://wla.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://vcl.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://hdq.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eej.cheryme.top

TS:   Math.max(...arr);
来源：http://gdi.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://atn.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fzl.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://cbp.316326.xyz

C#:   list.Max();  list.Min()
来源：http://wtx.pycfn.com

[D18] 扁平化嵌套数组
来源：http://hiy.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tej.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://hgy.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kcr.cdnleiting.top

TS:   nested.flat();
来源：http://wuh.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://loj.hesvh.cn

Go:   // 手写双层循环
来源：http://myn.shangyingyoupin.top

Ruby: nested.flatten
来源：http://qwx.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lbb.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://dwc.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sct.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ubc.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jqh.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pxs.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qff.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://bby.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rks.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryn.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://vvx.jiagoushi.top

Py:   Counter(arr)
来源：http://ckr.sxryk.cn

PHP:  array_count_values($arr);
来源：http://rnh.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqt.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjf.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bsd.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://fdo.shuidangran.top

Ruby: arr.tally
来源：http://zao.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bcx.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://lrs.yanxiufei.cn

Py:   x in arr
来源：http://dgg.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://min.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://xmn.xziqi.cn

TS:   arr.includes(x)
来源：http://oln.yangfankeji.com

Java: list.contains(x)
来源：http://knm.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://ifb.nanxinkj.top

Ruby: arr.include?(x)
来源：http://dvp.fktsv.cn

C#:   list.Contains(x)
来源：http://wgw.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://rrc.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rhd.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://psi.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qyt.pycfn.com

TS:   [...arr];
来源：http://ytq.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://soi.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://lxg.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://ywh.jiagoushi.top

C#:   new List<int>(list);
来源：http://bxk.0kj1m.cn

[D23] reduce 累积计算
来源：http://fnx.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cqg.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mfm.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tkb.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://srx.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cjt.xuetiantiany.cn

Go:   // 手写循环
来源：http://vsy.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ezk.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gic.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://jmm.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqe.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oeq.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tom.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ozu.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bla.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://omq.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwn.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xvu.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://ofn.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xxa.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kyg.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mwb.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ide.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fmo.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jwn.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ftq.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://odi.chenjidiqi.icu

[D26] 数组转字符串
来源：http://ujv.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://bzz.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://bha.shzxlz.cn

JS:   arr.join(", ")
来源：http://eou.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://syn.ctjpmb.com

Java: String.join(", ", list)
来源：http://wdd.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://smr.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://hru.cucudq.cn

C#:   string.Join(", ", list)
来源：http://iqf.jqgufenzy.top

================================================================================
来源：http://fhv.jinqigufen.top

E. 字符串处理
来源：http://vtk.yj202588.top

================================================================================
来源：http://jud.tian-w.cn

[E01] 拼接字符串
来源：http://zbj.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kln.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://obf.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzj.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wrf.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tuv.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fiz.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zvo.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bon.hesvh.cn

[E02] 重复字符串
来源：http://ktj.ybcxt.top

Py:   "ab" * 3
来源：http://dzx.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://fer.shuidangran.top

JS:   "ab".repeat(3)
来源：http://pbz.cheryme.top

TS:   "ab".repeat(3)
来源：http://djc.smart0.xyz

Java: "ab".repeat(3)
来源：http://iig.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://tfc.sufxvd.cn

Ruby: "ab" * 3
来源：http://rvm.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gyx.gogol.net.cn

[E03] 截取子串
来源：http://lcn.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vby.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wkz.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qym.guannengcc.top

TS:   s.slice(1, 4)
来源：http://zfa.aizwys.cn

Java: s.substring(1, 4)
来源：http://xqr.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jtk.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://dqs.uphjek.com

C#:   s.Substring(1, 3)
来源：http://vev.c1oappe.top

[E04] 查找子串位置
来源：http://bnn.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://tmb.bjfxy.top

PHP:  strpos($s, "x");
来源：http://dds.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wnx.yvedp.cn

TS:   s.indexOf("x")
来源：http://urt.daxiang520.top

Java: s.indexOf("x")
来源：http://tio.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://var.pengpengdd.cyou

Ruby: s.index("x")
来源：http://fir.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://ell.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ayw.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rci.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fhy.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://boc.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nnx.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hlm.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bvx.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pld.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eve.zhixingplan.top

[E06] 替换子串
来源：http://quf.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pwa.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://qsx.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://prh.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://zre.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://spa.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://out.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fis.nanxuanxn.top

C#:   s.Replace("a", "b")
来源：http://nxh.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://uyr.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://twe.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lzi.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://wnr.yongpay.top

TS:   s.split(",")
来源：http://vds.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://gon.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jio.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://tgl.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fcp.cucudq.cn

[E08] 数组按分隔符合并
来源：http://oma.nanxuanxn.top

Py:   ",".join(items)
来源：http://yab.yj202588.top

PHP:  implode(",", $items);
来源：http://imp.zhixingplan.top

JS:   items.join(",")
来源：http://myu.sjlbkw.cn

TS:   items.join(",")
来源：http://yor.daria6918.cn

Java: String.join(",", items)
来源：http://lyt.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://isi.gotoacloud.top

Ruby: items.join(",")
来源：http://haz.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://pop.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://ppf.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://byf.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dqe.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://ipo.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://inw.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://oqj.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wiw.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eah.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nel.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://lfu.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://taz.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bpo.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://ywv.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://irm.shuidangran.top

Java: String.format("%03d", 7)
来源：http://otx.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahp.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lwd.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kbz.cdnleiting.top

[E11] 反转字符串
来源：http://wak.snrcjt.cn

Py:   s[::-1]
来源：http://nmb.hongshengwenyu.top

PHP:  strrev($s);
来源：http://zmu.ivvv.top

JS:   [...s].reverse().join("")
来源：http://hpx.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://rdz.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fxv.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nzc.cucudq.cn

Ruby: s.reverse
来源：http://ulj.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rhl.cashguo.top

[E12] 统计某字符出现次数
来源：http://xaq.cashguo.top

Py:   s.count("a")
来源：http://ipb.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://hto.mhx1999.top

JS:   s.split("a").length - 1
来源：http://vek.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://ddy.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iey.zdbjq.cn


<!-- 参考信息 -->