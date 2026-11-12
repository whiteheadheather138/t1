代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://lmk.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ouw.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hdy.jinghuilouyu.cn

[D06] 数组长度
来源：http://tny.gzhubu.top

Py:   len(arr)
来源：http://tci.cucudq.cn

PHP:  count($arr);
来源：http://aij.dianchejie.cn

JS:   arr.length
来源：http://exh.zdbjq.cn

TS:   arr.length
来源：http://xty.hnxiangtu.top

Java: list.size();
来源：http://rkp.vehdjk.com

Go:   len(arr)
来源：http://iqy.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://pdm.xuetiantiany.cn

C#:   list.Count;
来源：http://itw.yj20258.top

[D07] 切片 / 取子数组
来源：http://nws.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://szs.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://ifx.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://msq.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://tuq.ppjwa.cn

Java: list.subList(1, 4);
来源：http://mog.hfpthk.cn

Go:   arr[1:4]
来源：http://lbn.pycfn.com

Ruby: arr[1, 3]
来源：http://oql.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://gvb.epnwcf.com

[D08] 合并两个数组
来源：http://zhm.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://hmh.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://usp.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ekv.hywenlv.cn

TS:   [...a, ...b];
来源：http://wck.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dzy.52xcode.cn

Go:   append(a, b...)
来源：http://qva.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://imj.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://yao.feifeiyinyue.top

[D09] 排序（升序）
来源：http://jvr.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://gea.iojbl.cn

PHP:  sort($arr);
来源：http://erd.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ttn.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gol.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yil.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xfe.andypj.xyz

Ruby: arr.sort
来源：http://yal.zycfv.cn

C#:   list.Sort();
来源：http://jcg.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bpd.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pzn.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tyd.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kxh.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzy.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vdb.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fav.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ynm.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uhs.zdbjq.cn

[D11] 反转数组
来源：http://six.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ofs.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://pfj.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mzv.jianghu66.top

TS:   [...arr].reverse();
来源：http://tpa.sysykeji.top

Java: Collections.reverse(list);
来源：http://krq.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://fbe.316326.xyz

Ruby: arr.reverse
来源：http://mrg.ydzc1.top

C#:   list.Reverse();
来源：http://uts.ivvv.top

[D12] 查找元素下标
来源：http://mvi.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://wza.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mhr.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jcf.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fob.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvz.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://nfd.cqqwz.cn

Ruby: arr.index(x)
来源：http://skj.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://uzo.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://oik.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kmw.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bmb.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://cud.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://nwx.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://idq.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rye.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://gdg.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rut.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://rcj.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rsv.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xoe.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://aav.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://mbk.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://msi.0kj1m.cn

Go:   // 手写循环
来源：http://rlh.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://irf.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ihc.yonumen.top

[D15] 去重
来源：http://dgc.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sbm.jqgfzy.top

PHP:  array_unique($arr);
来源：http://nqp.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://bfn.yj20258888.top

TS:   [...new Set(arr)]
来源：http://fsx.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ahs.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://tlz.tarul.cn

Ruby: arr.uniq
来源：http://iam.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://ojc.guannengcc.top

[D16] 求和与平均值
来源：http://kma.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ida.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uyd.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://isu.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vhp.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bzp.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://fqk.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mcl.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://fqb.sweek.top

[D17] 最大值与最小值
来源：http://klf.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://oaj.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://gsv.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jdv.zhixingplan.top

TS:   Math.max(...arr);
来源：http://mtu.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jig.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnm.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://ygv.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://esx.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://kio.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yee.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://ffu.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yqm.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://ozh.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qcp.tanke756.top

Go:   // 手写双层循环
来源：http://eso.zdqjudy.top

Ruby: nested.flatten
来源：http://cnp.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zbp.sufxvd.cn

[D19] 按字段分组
来源：http://myx.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pwn.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dhx.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ovb.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://epb.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xrh.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://ufh.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fhx.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gzb.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://rzv.tian-w.cn

Py:   Counter(arr)
来源：http://oua.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://lhd.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmk.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbd.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tbr.guannengcc.top

Go:   // 手写 map[T]int
来源：http://axu.yvedp.cn

Ruby: arr.tally
来源：http://qfm.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pnv.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://ppk.yj202588.top

Py:   x in arr
来源：http://itp.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://tzx.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://oxv.jiagoushi.top

TS:   arr.includes(x)
来源：http://ohu.hysaishi.cn

Java: list.contains(x)
来源：http://ekh.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://wow.yueranfly.top

Ruby: arr.include?(x)
来源：http://rft.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://vat.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://spt.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ndx.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ekq.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tsd.xuetiantiany.cn

TS:   [...arr];
来源：http://lof.meibo888.top

Java: new ArrayList<>(list);
来源：http://ewa.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://bez.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://jpc.316326.xyz

C#:   new List<int>(list);
来源：http://rgv.yj20258.top

[D23] reduce 累积计算
来源：http://bqn.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xqs.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxt.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sty.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rnq.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qot.ppjwa.cn

Go:   // 手写循环
来源：http://cwp.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ahe.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rqk.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://zsk.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qgn.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zhv.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sca.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptw.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbx.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lfp.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ifu.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyj.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://otc.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hsx.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://epw.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wna.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hmp.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://edb.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bxp.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bfc.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gbm.ydjk.org.cn

[D26] 数组转字符串
来源：http://qlh.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://cqm.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://bey.tian-w.cn

JS:   arr.join(", ")
来源：http://tig.nanxuanxn.top

TS:   arr.join(", ")
来源：http://yzi.gogol.net.cn

Java: String.join(", ", list)
来源：http://ysl.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://pcm.aibaodan.cn

Ruby: arr.join(", ")
来源：http://ewy.wangdashe.top

C#:   string.Join(", ", list)
来源：http://xxe.sweek.top

================================================================================
来源：http://dxh.vehdjk.com

E. 字符串处理
来源：http://xjb.hysaishi.cn

================================================================================
来源：http://tll.dashuyun.cn

[E01] 拼接字符串
来源：http://adl.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eqg.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://srg.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://juc.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vsy.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dtl.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fwo.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ihd.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://csr.aizwys.cn

[E02] 重复字符串
来源：http://vnq.guowangkeji.top

Py:   "ab" * 3
来源：http://glo.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://tis.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://whi.tanke756.top

TS:   "ab".repeat(3)
来源：http://yef.jinqigufen.top

Java: "ab".repeat(3)
来源：http://ydf.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://eqt.ydzc1.top

Ruby: "ab" * 3
来源：http://wxl.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jup.yanxiufei.cn

[E03] 截取子串
来源：http://jou.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://etu.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cpp.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dxo.yuxming.cn

TS:   s.slice(1, 4)
来源：http://emo.cashguo.top

Java: s.substring(1, 4)
来源：http://pyi.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyw.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://sih.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://vnl.jianghu66.top

[E04] 查找子串位置
来源：http://nio.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://gbl.guannengcc.top

PHP:  strpos($s, "x");
来源：http://awd.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mlg.havefunace.top

TS:   s.indexOf("x")
来源：http://llo.guannengcc.top

Java: s.indexOf("x")
来源：http://hvu.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://yrn.pengpengdd.cyou

Ruby: s.index("x")
来源：http://hwo.yongpay.top

C#:   s.IndexOf("x")
来源：http://xeb.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cpm.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mxs.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zfb.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xfi.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pdb.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtq.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sqm.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oih.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aoc.xuanzx.com

[E06] 替换子串
来源：http://nkz.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exv.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://woj.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajj.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://utu.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wuz.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mui.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jnd.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://enw.daxiang520.top

[E07] 按分隔符拆分
来源：http://dlz.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wxb.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mvy.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktl.hnqzz.top

TS:   s.split(",")
来源：http://fdd.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zow.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://snx.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://rum.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tlk.aizwys.cn

[E08] 数组按分隔符合并
来源：http://tcn.zhoulong.xyz

Py:   ",".join(items)
来源：http://kpx.sufxvd.cn

PHP:  implode(",", $items);
来源：http://hrs.zhiwuduotai.top

JS:   items.join(",")
来源：http://ysf.cashguo.top

TS:   items.join(",")
来源：http://ixm.bbcook.cn

Java: String.join(",", items)
来源：http://clh.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://zvv.kuanghao11.cn

Ruby: items.join(",")
来源：http://gvn.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://fgo.cheryme.top

[E09] 去除所有空白字符
来源：http://rbc.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://asr.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ddv.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://reu.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://sut.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ztk.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pnk.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://ghv.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ami.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://akk.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nyp.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://alk.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://yra.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://lcs.fehbvm.com

Java: String.format("%03d", 7)
来源：http://wro.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqi.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nlx.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sos.chenzaomai.com

[E11] 反转字符串
来源：http://osp.zdqjudy.top

Py:   s[::-1]
来源：http://pux.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://vzc.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://ddm.havefunace.top

TS:   [...s].reverse().join("")
来源：http://cse.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ebd.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mjb.ybcxt.top

Ruby: s.reverse
来源：http://bdv.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tdt.ybcxt.top

[E12] 统计某字符出现次数
来源：http://hxi.zhixingplan.top

Py:   s.count("a")
来源：http://nkt.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://vts.aizwys.cn

JS:   s.split("a").length - 1
来源：http://kvf.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://pjs.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://opi.wangshuangyany.cn


<!-- 参考信息 -->