代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mdd.bbcook.cn

[D08] 合并两个数组
来源：http://ogq.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://qcm.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://qjp.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wnz.9152youxi.cn

TS:   [...a, ...b];
来源：http://fyq.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zel.gaohongyu789.top

Go:   append(a, b...)
来源：http://xcw.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://sfn.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://vdb.sweek.top

[D09] 排序（升序）
来源：http://zzl.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://xyp.chenzaomai.com

PHP:  sort($arr);
来源：http://dvo.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://usw.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xns.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://unb.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ohj.jyoumei.cn

Ruby: arr.sort
来源：http://qva.gzhubu.top

C#:   list.Sort();
来源：http://njv.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gfe.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yfr.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yju.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qop.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nha.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ecf.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tsd.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfw.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pqg.zhijiandao.cn

[D11] 反转数组
来源：http://gqp.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qbu.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://typ.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fck.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://imh.yangfankeji.com

Java: Collections.reverse(list);
来源：http://zua.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://qyu.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://vpz.yangfankeji.com

C#:   list.Reverse();
来源：http://tyj.sysykeji.top

[D12] 查找元素下标
来源：http://ofc.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://jmk.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gwq.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gkj.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cbq.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hem.tarul.cn

Go:   slices.Index(arr, x)
来源：http://olf.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://vfe.ydzc1.top

C#:   list.IndexOf(x);
来源：http://gqy.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://loa.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bzd.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mjq.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://uww.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://azs.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ina.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vot.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iab.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yyp.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://fkh.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://guy.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wpg.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://kqz.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://kke.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gpj.jqgfzy.top

Go:   // 手写循环
来源：http://jpu.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://quf.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zyn.uphjek.com

[D15] 去重
来源：http://zgs.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uam.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://ioi.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://ujm.ybcxt.top

TS:   [...new Set(arr)]
来源：http://wqe.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://daw.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://obu.uphjek.com

Ruby: arr.uniq
来源：http://xft.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://qnu.shuidangran.top

[D16] 求和与平均值
来源：http://hxz.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://czn.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iat.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpr.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cuq.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pkm.9152youxi.cn

Go:   // 手写循环累加
来源：http://rap.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gqz.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://cvt.nwbrower.top

[D17] 最大值与最小值
来源：http://yzr.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://dtn.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://qvp.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zuv.fzhhl.top

TS:   Math.max(...arr);
来源：http://xkh.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zuo.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wnj.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://sfw.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://qow.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://xea.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rmw.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://qec.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fnh.svipenyu.cn

TS:   nested.flat();
来源：http://tul.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lsr.guowangkeji.top

Go:   // 手写双层循环
来源：http://qcj.316326.xyz

Ruby: nested.flatten
来源：http://ndg.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhy.vehdjk.com

[D19] 按字段分组
来源：http://bqo.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qkl.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hol.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jqu.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hdt.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fjw.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://toc.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oqn.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nvb.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://nxz.zhengqikj.top

Py:   Counter(arr)
来源：http://bck.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://wba.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scd.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvh.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yoh.yj20258888.top

Go:   // 手写 map[T]int
来源：http://jdr.zhijiandao.cn

Ruby: arr.tally
来源：http://cdq.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qzh.andypj.xyz

[D21] 判断是否包含某元素
来源：http://kcm.mhx1999.top

Py:   x in arr
来源：http://gui.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://pmi.dashuyun.cn

JS:   arr.includes(x)
来源：http://bub.ctjpmb.com

TS:   arr.includes(x)
来源：http://kpg.jinqigfzy.top

Java: list.contains(x)
来源：http://alh.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://wxi.havefunace.top

Ruby: arr.include?(x)
来源：http://rlo.redwolf501.top

C#:   list.Contains(x)
来源：http://lww.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://vri.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ayw.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qkd.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bwp.svipenyu.cn

TS:   [...arr];
来源：http://gsg.ybcxt.top

Java: new ArrayList<>(list);
来源：http://tgl.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://qxx.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://tds.jianghu66.top

C#:   new List<int>(list);
来源：http://mzo.nanxuanxn.top

[D23] reduce 累积计算
来源：http://syg.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gna.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qrz.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozc.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oye.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ygf.jinghuilouyu.cn

Go:   // 手写循环
来源：http://blf.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://naf.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ptp.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://udk.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qcz.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yhg.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zac.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xqe.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dbv.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vdq.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://etg.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://idd.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://oky.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jmf.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wxi.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gtm.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ofc.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wcb.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cch.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bmn.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://upf.zhiwuduotai.top

[D26] 数组转字符串
来源：http://rgh.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://rwi.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://iun.birdmap.top

JS:   arr.join(", ")
来源：http://wzu.fktsv.cn

TS:   arr.join(", ")
来源：http://shx.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://dzl.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://ful.nanxinkj.top

Ruby: arr.join(", ")
来源：http://kbr.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://xie.iojbl.cn

================================================================================
来源：http://mqj.zhaomingkeji.xyz

E. 字符串处理
来源：http://xil.feifeiyinyue.top

================================================================================
来源：http://sqs.yj20258.top

[E01] 拼接字符串
来源：http://bbb.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwz.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uyt.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://avg.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://roa.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iiu.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yfp.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gsx.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umw.jinqigufen.top

[E02] 重复字符串
来源：http://een.haohaochexian.top

Py:   "ab" * 3
来源：http://ykq.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://zek.52xcode.cn

JS:   "ab".repeat(3)
来源：http://rgr.52xcode.cn

TS:   "ab".repeat(3)
来源：http://egy.xylfe.cn

Java: "ab".repeat(3)
来源：http://zeq.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://bcd.hnqzz.top

Ruby: "ab" * 3
来源：http://oom.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sta.andypj.xyz

[E03] 截取子串
来源：http://msl.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgl.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rey.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xcb.yj202588.top

TS:   s.slice(1, 4)
来源：http://hwg.52xcode.cn

Java: s.substring(1, 4)
来源：http://qdr.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qvz.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iuq.sweek.top

C#:   s.Substring(1, 3)
来源：http://njn.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://psm.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://epr.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://oyv.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gbq.meibo888.top

TS:   s.indexOf("x")
来源：http://sfk.snrcjt.cn

Java: s.indexOf("x")
来源：http://emv.hammf.cn

Go:   strings.Index(s, "x")
来源：http://vql.vehdjk.com

Ruby: s.index("x")
来源：http://naf.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://aqp.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iag.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fam.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pte.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://afn.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yco.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iwd.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kfs.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rpi.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mio.andypj.xyz

[E06] 替换子串
来源：http://sgb.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mwg.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://iix.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ihh.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://fbs.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ttv.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wwy.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nsn.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://ffj.hesvh.cn

[E07] 按分隔符拆分
来源：http://qej.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://voq.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dvv.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://glr.wangshuangyany.cn

TS:   s.split(",")
来源：http://slj.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://gqj.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bww.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://mkj.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mqp.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://uyh.yongpay.top

Py:   ",".join(items)
来源：http://sky.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://tov.zdqjudy.top

JS:   items.join(",")
来源：http://yoe.pycfn.com

TS:   items.join(",")
来源：http://usv.0kj1m.cn

Java: String.join(",", items)
来源：http://niy.tanke756.top

Go:   strings.Join(items, ",")
来源：http://wqe.ydjk.org.cn

Ruby: items.join(",")
来源：http://scg.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://gth.cucudq.cn

[E09] 去除所有空白字符
来源：http://awf.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dcy.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfd.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://thu.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://gnd.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://cjr.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dah.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://edt.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ptx.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://dvg.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ojx.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fss.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://eii.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://ndq.52xcode.cn

Java: String.format("%03d", 7)
来源：http://oyz.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wdi.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gbe.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jpd.uphjek.com

[E11] 反转字符串
来源：http://eov.fehbvm.com

Py:   s[::-1]
来源：http://jia.wangshuangyany.cn

PHP:  strrev($s);
来源：http://kfq.cheryme.top

JS:   [...s].reverse().join("")
来源：http://fkt.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://tyz.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pci.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uvt.zycfv.cn

Ruby: s.reverse
来源：http://dtm.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://cxf.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://cin.birdmap.top

Py:   s.count("a")
来源：http://jcq.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://qxs.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://hhq.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://mee.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ezm.cashguo.top

Go:   strings.Count(s, "a")
来源：http://tgt.zhengqikj.top

Ruby: s.count("a")
来源：http://svc.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://ulp.jyoumei.cn

[E13] 逐字符遍历
来源：http://vws.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://alr.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qni.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vet.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yto.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://onn.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oug.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qrw.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mjd.hammf.cn

[E14] URL 编码与 Base64
来源：http://kqd.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wuf.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zkw.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mna.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mes.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rob.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vtf.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gpa.xingfuxueyuan.xyz


<!-- 参考信息 -->