代发 wailian999

Py:   len(arr)
来源：http://rpr.jyoumei.cn

PHP:  count($arr);
来源：http://zwd.ppjwa.cn

JS:   arr.length
来源：http://ins.vqdsnc.cn

TS:   arr.length
来源：http://iej.jinghuilouyu.cn

Java: list.size();
来源：http://bjk.feifeiyinyue.top

Go:   len(arr)
来源：http://ofm.hcnkem.com

Ruby: arr.length; arr.size
来源：http://ayk.tianlin.xyz

C#:   list.Count;
来源：http://vtd.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://giy.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wqk.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uvu.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://kdb.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://ktc.aibaodan.cn

Java: list.subList(1, 4);
来源：http://lsg.jiagoushi.top

Go:   arr[1:4]
来源：http://awa.andypj.xyz

Ruby: arr[1, 3]
来源：http://mbr.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://qyn.yanxiufei.cn

[D08] 合并两个数组
来源：http://gya.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://izr.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://bay.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ljy.zhixingplan.top

TS:   [...a, ...b];
来源：http://pjz.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zha.svipenyu.cn

Go:   append(a, b...)
来源：http://hfq.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://ccn.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://mto.ivvv.top

[D09] 排序（升序）
来源：http://lsc.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://afj.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://ehk.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vkd.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rch.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pjj.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gzt.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://egn.chenzaomai.com

C#:   list.Sort();
来源：http://uxm.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qdg.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tne.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnh.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gaw.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://syc.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rlp.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fje.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ekb.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxc.shangyingyoupin.top

[D11] 反转数组
来源：http://ycq.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vqf.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://jyy.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gtv.yj20258.top

TS:   [...arr].reverse();
来源：http://xkf.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://zwl.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://atl.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://kws.hysaishi.cn

C#:   list.Reverse();
来源：http://eao.sysykeji.top

[D12] 查找元素下标
来源：http://ddu.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://cal.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wlu.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvw.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqy.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dxj.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://jis.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://khc.guannengcc.top

C#:   list.IndexOf(x);
来源：http://amk.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://gsm.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wta.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wvi.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://cri.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://usx.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uyk.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://msk.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://jih.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qjy.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://wkc.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://omn.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zrs.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://umv.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://zyp.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wlk.kuanghao11.cn

Go:   // 手写循环
来源：http://zny.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://lli.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ahe.jinqigufen.top

[D15] 去重
来源：http://wca.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vyt.hesvh.cn

PHP:  array_unique($arr);
来源：http://lxh.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://hlz.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://iez.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ceq.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://iit.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://vpm.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://zsz.dianchejie.cn

[D16] 求和与平均值
来源：http://qwp.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyx.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cav.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebo.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://drf.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://okk.jlsjyb.cn

Go:   // 手写循环累加
来源：http://dec.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gcm.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://dbo.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://kge.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://pok.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://rry.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vlk.daxiang520.top

TS:   Math.max(...arr);
来源：http://tys.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bif.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cfa.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://tcx.316326.xyz

C#:   list.Max();  list.Min()
来源：http://sew.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://uyl.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zru.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://fld.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hiv.zhongyouzk.top

TS:   nested.flat();
来源：http://zho.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://myt.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://ood.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://syt.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://eww.andypj.xyz

[D19] 按字段分组
来源：http://vjt.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vdo.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cud.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sbr.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rav.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bks.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://djb.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpp.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zbp.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://glj.wangshuangyany.cn

Py:   Counter(arr)
来源：http://uka.fktsv.cn

PHP:  array_count_values($arr);
来源：http://xhh.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://igd.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooe.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://neh.ydzc1.top

Go:   // 手写 map[T]int
来源：http://hey.uphjek.com

Ruby: arr.tally
来源：http://alj.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pwc.tian-w.cn

[D21] 判断是否包含某元素
来源：http://omf.vqdsnc.cn

Py:   x in arr
来源：http://foo.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://etb.0kj1m.cn

JS:   arr.includes(x)
来源：http://csp.havefunace.top

TS:   arr.includes(x)
来源：http://urp.guowangkeji.top

Java: list.contains(x)
来源：http://wzh.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://cyg.zhixingplan.top

Ruby: arr.include?(x)
来源：http://tnd.yuxming.cn

C#:   list.Contains(x)
来源：http://upa.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://flf.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uoc.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://med.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jqs.zhixingplan.top

TS:   [...arr];
来源：http://oir.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://pub.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wbx.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://cgm.chenlongwang.top

C#:   new List<int>(list);
来源：http://htx.quarkkingdee.top

[D23] reduce 累积计算
来源：http://dgl.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ngc.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kev.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qif.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eip.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mpn.hcnkem.com

Go:   // 手写循环
来源：http://tdy.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://alc.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xmb.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://zwy.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ylf.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vmq.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ufr.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jyn.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsd.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cgf.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://arj.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hrk.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://mac.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pig.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jzc.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://phd.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wgg.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ctp.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://njx.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qzh.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://abb.tarul.cn

[D26] 数组转字符串
来源：http://aet.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://rzw.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://qbr.gogol.net.cn

JS:   arr.join(", ")
来源：http://zse.jianghu66.top

TS:   arr.join(", ")
来源：http://skc.sysykeji.top

Java: String.join(", ", list)
来源：http://wmk.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://mwn.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://yzj.hammf.cn

C#:   string.Join(", ", list)
来源：http://cse.shangyingyoupin.top

================================================================================
来源：http://azj.feifeiyinyue.top

E. 字符串处理
来源：http://tjq.zhongyouzk.top

================================================================================
来源：http://rwo.jianghu66.top

[E01] 拼接字符串
来源：http://oth.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://spb.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eub.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ara.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rhs.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fiw.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iud.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://puv.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kzl.chenzaomai.com

[E02] 重复字符串
来源：http://irv.tianlin.xyz

Py:   "ab" * 3
来源：http://hlh.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://vne.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://lvq.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://fog.jianghu66.top

Java: "ab".repeat(3)
来源：http://udt.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://nhv.yongpay.top

Ruby: "ab" * 3
来源：http://hwk.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cps.andypj.xyz

[E03] 截取子串
来源：http://vbi.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dzy.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://akq.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cos.bbcook.cn

TS:   s.slice(1, 4)
来源：http://etf.yuxming.cn

Java: s.substring(1, 4)
来源：http://sii.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xum.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://leh.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://rkj.cqqwz.cn

[E04] 查找子串位置
来源：http://ece.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://uzi.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://een.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mds.ctjpmb.com

TS:   s.indexOf("x")
来源：http://ido.yfazqb.com

Java: s.indexOf("x")
来源：http://eoz.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://fly.jqgufenzy.top

Ruby: s.index("x")
来源：http://znp.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://dqz.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qcv.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zor.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vmh.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywp.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zwi.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fwh.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zrv.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ift.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rls.jinghuilouyu.cn

[E06] 替换子串
来源：http://hfj.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bxd.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://oee.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qux.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://bwk.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifo.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wqt.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://znc.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://psa.zycfv.cn

[E07] 按分隔符拆分
来源：http://xrc.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bsp.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qkg.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dsm.dashuyun.cn

TS:   s.split(",")
来源：http://kcx.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pbm.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fuo.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://eub.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://swc.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://vdb.redwolf501.top

Py:   ",".join(items)
来源：http://jeb.iojbl.cn

PHP:  implode(",", $items);
来源：http://don.vqdsnc.cn

JS:   items.join(",")
来源：http://tfu.ivvv.top

TS:   items.join(",")
来源：http://zos.hfpthk.cn

Java: String.join(",", items)
来源：http://ddi.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://lty.mhx1999.top

Ruby: items.join(",")
来源：http://duo.yonumen.top

C#:   string.Join(",", items)
来源：http://lqv.zycfv.cn

[E09] 去除所有空白字符
来源：http://hwu.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gfq.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bml.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://eua.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://sqb.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://fhi.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mun.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://fum.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ztm.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://cib.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fts.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vjq.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://zor.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://sfg.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://uoa.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://htt.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wqu.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hax.jinghuilouyu.cn

[E11] 反转字符串
来源：http://ayp.0kj1m.cn

Py:   s[::-1]
来源：http://bgc.tian-w.cn

PHP:  strrev($s);
来源：http://hec.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://fka.yj202588.top

TS:   [...s].reverse().join("")
来源：http://jqr.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kqb.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sgd.zhengqikj.top

Ruby: s.reverse
来源：http://myn.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jbn.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://bat.zdqjudy.top

Py:   s.count("a")
来源：http://jjw.uphjek.com

PHP:  substr_count($s, "a");
来源：http://aje.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://tgx.xuanzx.com

TS:   s.split("a").length - 1
来源：http://ast.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://adz.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://ihi.dianchejie.cn

Ruby: s.count("a")
来源：http://nvg.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://ezm.zhongyouzk.top

[E13] 逐字符遍历
来源：http://ano.tian-w.cn


<!-- 参考信息 -->