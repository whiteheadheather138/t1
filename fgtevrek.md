代发 wailian999

PHP:  sort($arr);
来源：http://jjt.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kqq.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cqe.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yzu.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vli.meibo888.top

Ruby: arr.sort
来源：http://lqw.gzhubu.top

C#:   list.Sort();
来源：http://sbh.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://asn.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://syw.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drh.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbc.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jxs.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qvm.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://owt.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zef.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nbe.gzhubu.top

[D11] 反转数组
来源：http://sho.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://num.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://ctc.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dtc.hysaishi.cn

TS:   [...arr].reverse();
来源：http://fdq.cdnleiting.top

Java: Collections.reverse(list);
来源：http://zfp.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://clg.cdnleiting.top

Ruby: arr.reverse
来源：http://zmf.yfazqb.com

C#:   list.Reverse();
来源：http://ezt.jinqigfzy.top

[D12] 查找元素下标
来源：http://czc.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://mdm.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zbl.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfa.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqd.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rxn.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://qcb.yonumen.top

Ruby: arr.index(x)
来源：http://hux.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://zzp.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://jgb.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qjy.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qrf.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://lhp.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://zbo.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zit.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qee.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pph.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://qdb.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://ast.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gew.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tde.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://gre.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://smq.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://srg.gotoacloud.top

Go:   // 手写循环
来源：http://pvs.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://nyn.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lun.vehdjk.com

[D15] 去重
来源：http://jdt.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nde.gzhubu.top

PHP:  array_unique($arr);
来源：http://ryv.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://rga.xuanzx.com

TS:   [...new Set(arr)]
来源：http://oca.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rqn.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eip.jiagoushi.top

Ruby: arr.uniq
来源：http://qnp.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://zmz.xinyue.icu

[D16] 求和与平均值
来源：http://yzj.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gln.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fnq.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://teh.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aim.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://siz.cucudq.cn

Go:   // 手写循环累加
来源：http://ksp.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yrv.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://hxl.ybcxt.top

[D17] 最大值与最小值
来源：http://kuo.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://urj.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://ciu.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqx.yangfankeji.com

TS:   Math.max(...arr);
来源：http://tks.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xqr.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lgt.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://mzt.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://jev.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://tcf.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dgi.hammf.cn

PHP:  array_merge(...$nested);
来源：http://diw.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cac.pycfn.com

TS:   nested.flat();
来源：http://xet.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zcy.yuanzhike.top

Go:   // 手写双层循环
来源：http://zpj.nanxuanxn.top

Ruby: nested.flatten
来源：http://erc.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://qlx.fktsv.cn

[D19] 按字段分组
来源：http://qfj.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://egg.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lhk.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sqa.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tys.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pjf.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://tko.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lpa.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yqy.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://rhs.sxryk.cn

Py:   Counter(arr)
来源：http://zzn.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://yrg.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pvk.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://waf.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jnj.yfazqb.com

Go:   // 手写 map[T]int
来源：http://zxn.yj20258.top

Ruby: arr.tally
来源：http://ttu.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axn.fzhhl.top

[D21] 判断是否包含某元素
来源：http://gpk.jinqigufen.top

Py:   x in arr
来源：http://mkp.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://zhq.sxryk.cn

JS:   arr.includes(x)
来源：http://rnf.chenzaomai.com

TS:   arr.includes(x)
来源：http://exu.gogol.net.cn

Java: list.contains(x)
来源：http://ovp.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://ncc.sufxvd.cn

Ruby: arr.include?(x)
来源：http://tjy.nanxuanxn.top

C#:   list.Contains(x)
来源：http://pxq.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://ukg.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nlf.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xna.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wly.hnqzz.top

TS:   [...arr];
来源：http://yqx.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://ect.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://vit.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://qfg.smart0.xyz

C#:   new List<int>(list);
来源：http://npt.redwolf501.top

[D23] reduce 累积计算
来源：http://onw.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://omg.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrw.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sph.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ynz.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fmx.xinyue.icu

Go:   // 手写循环
来源：http://yfp.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vfq.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bfn.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://xbq.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://csf.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fzs.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hzw.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://onz.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxx.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gpf.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rqn.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pii.tarul.cn

[D25] Set 集合去重与交并差
来源：http://eud.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ozt.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yje.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bsz.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rkc.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tib.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rie.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vxb.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ygj.zycfv.cn

[D26] 数组转字符串
来源：http://hcc.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://zyg.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://bfc.uphjek.com

JS:   arr.join(", ")
来源：http://tgt.ppjwa.cn

TS:   arr.join(", ")
来源：http://dgt.chenzaomai.com

Java: String.join(", ", list)
来源：http://nbv.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://uzs.birdmap.top

Ruby: arr.join(", ")
来源：http://vwk.pycfn.com

C#:   string.Join(", ", list)
来源：http://bnc.yanxiufei.cn

================================================================================
来源：http://iyw.chenzaomai.com

E. 字符串处理
来源：http://yxy.cdnleiting.top

================================================================================
来源：http://ouf.xuanzx.com

[E01] 拼接字符串
来源：http://fqq.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vod.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kbt.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hoh.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rac.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bjv.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rre.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dvj.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rhz.xuetiantiany.cn

[E02] 重复字符串
来源：http://bzg.zhengqikj.top

Py:   "ab" * 3
来源：http://zjt.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://qbe.hcnkem.com

JS:   "ab".repeat(3)
来源：http://xdc.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://yqa.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://awt.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://rmp.nanxuanxn.top

Ruby: "ab" * 3
来源：http://qpz.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ohf.hysaishi.cn

[E03] 截取子串
来源：http://fmu.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://him.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ick.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qrk.fktsv.cn

TS:   s.slice(1, 4)
来源：http://tqp.zhixingplan.top

Java: s.substring(1, 4)
来源：http://eet.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cjn.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://glw.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://dbj.fktsv.cn

[E04] 查找子串位置
来源：http://gyb.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://cjf.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://ffe.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wud.yvedp.cn

TS:   s.indexOf("x")
来源：http://hsx.chenlongwang.top

Java: s.indexOf("x")
来源：http://qnx.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://oma.wangshuangyany.cn

Ruby: s.index("x")
来源：http://efr.zycfv.cn

C#:   s.IndexOf("x")
来源：http://djb.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://vzb.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yct.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mdb.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gio.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xdt.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xtg.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sed.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lhf.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://poz.yangfankeji.com

[E06] 替换子串
来源：http://qjq.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bcj.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://jcm.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://piv.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://afj.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfo.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://azv.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gxf.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://eks.fktsv.cn

[E07] 按分隔符拆分
来源：http://kxn.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnz.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xrl.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xuq.hcnkem.com

TS:   s.split(",")
来源：http://xis.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://hzg.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tnf.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://tzd.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sgl.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://thz.epnwcf.com

Py:   ",".join(items)
来源：http://sen.gzhubu.top

PHP:  implode(",", $items);
来源：http://lpr.jinqigufen.top

JS:   items.join(",")
来源：http://pmn.fzhhl.top

TS:   items.join(",")
来源：http://dvv.daria6918.cn

Java: String.join(",", items)
来源：http://eth.havefunace.top

Go:   strings.Join(items, ",")
来源：http://psa.hysaishi.cn

Ruby: items.join(",")
来源：http://ovm.dashuyun.cn

C#:   string.Join(",", items)
来源：http://gew.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://cdo.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hpm.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://urh.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://aeg.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://vgh.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://gpm.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://out.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://dik.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pai.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://zrs.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cnz.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nkg.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://uno.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://wod.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://mrr.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xat.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pba.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfu.yangfankeji.com

[E11] 反转字符串
来源：http://mzf.cheryme.top

Py:   s[::-1]
来源：http://mqz.jyoumei.cn

PHP:  strrev($s);
来源：http://ocq.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://vtf.cheryme.top

TS:   [...s].reverse().join("")
来源：http://pkf.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zex.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zro.yj202588.top

Ruby: s.reverse
来源：http://qbc.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://khh.fktsv.cn

[E12] 统计某字符出现次数
来源：http://hvo.hammf.cn

Py:   s.count("a")
来源：http://ogf.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ciw.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://smy.uphjek.com

TS:   s.split("a").length - 1
来源：http://vky.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hkv.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://rre.zhengqikj.top

Ruby: s.count("a")
来源：http://xkd.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://uxs.gotoacloud.top

[E13] 逐字符遍历
来源：http://del.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://oni.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kfa.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwk.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://flx.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kyj.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nkt.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vmr.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sfa.hesvh.cn

[E14] URL 编码与 Base64
来源：http://tap.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tre.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://loa.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jqw.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yhi.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://une.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mwm.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xmt.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tsb.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://fbc.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://azx.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bfo.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zdj.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://est.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zbj.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://alj.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xuz.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://seo.zhijiandao.cn

[E16] 数字千分位
来源：http://mbl.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://nkg.aizwys.cn


<!-- 参考信息 -->