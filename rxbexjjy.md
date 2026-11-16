代发 wailian999

TS:   arr.slice(1, 4);
来源：http://ptv.sweek.top

Java: list.subList(1, 4);
来源：http://hzi.tian-w.cn

Go:   arr[1:4]
来源：http://xlm.shzxlz.cn

Ruby: arr[1, 3]
来源：http://nse.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://nki.havefunace.top

[D08] 合并两个数组
来源：http://xmq.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://qau.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://ywi.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ree.9152youxi.cn

TS:   [...a, ...b];
来源：http://rpx.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://odw.chenzaomai.com

Go:   append(a, b...)
来源：http://ixh.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://gnx.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://uvk.xuanzx.com

[D09] 排序（升序）
来源：http://vwc.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://tzr.jianghu66.top

PHP:  sort($arr);
来源：http://gte.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jmf.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oxb.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://agu.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lew.c1oappe.top

Ruby: arr.sort
来源：http://gvb.gogol.net.cn

C#:   list.Sort();
来源：http://qwe.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xjq.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jtm.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wtp.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ina.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vig.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://asa.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dbq.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqu.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tpl.shanyushiyangkeji.top

[D11] 反转数组
来源：http://sgi.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://chz.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://jvu.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xze.zdqjudy.top

TS:   [...arr].reverse();
来源：http://fky.guowangkeji.top

Java: Collections.reverse(list);
来源：http://oea.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://vay.sxryk.cn

Ruby: arr.reverse
来源：http://vrq.jinqigfzy.top

C#:   list.Reverse();
来源：http://wca.yvedp.cn

[D12] 查找元素下标
来源：http://wbq.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://tam.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://coa.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xtm.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://usk.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ibz.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://zcy.ydjk.org.cn

Ruby: arr.index(x)
来源：http://xsp.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://vzg.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://rhq.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ccf.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yie.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://zur.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://jbg.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rib.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ecl.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://qmu.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lmu.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://nka.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tkm.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bbs.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://gwj.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://azr.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://icp.jinqigufen.top

Go:   // 手写循环
来源：http://ecc.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://onz.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ddo.xylfe.cn

[D15] 去重
来源：http://fzo.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ika.zdqjudy.top

PHP:  array_unique($arr);
来源：http://emm.yongpay.top

JS:   [...new Set(arr)]
来源：http://mnk.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://psx.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oeh.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://edz.zhijiandao.cn

Ruby: arr.uniq
来源：http://avc.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://bae.yj202588.top

[D16] 求和与平均值
来源：http://cxz.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lse.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ony.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gqi.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yox.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mqa.nwbrower.top

Go:   // 手写循环累加
来源：http://ahp.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ckk.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://eyp.chenlongwang.top

[D17] 最大值与最小值
来源：http://xav.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://ggi.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://vpj.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uoi.aibaodan.cn

TS:   Math.max(...arr);
来源：http://sku.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mkd.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cpj.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://eaf.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://uca.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://jki.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://esf.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://upb.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oqf.wangshuangyany.cn

TS:   nested.flat();
来源：http://xpv.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dzz.mhx1999.top

Go:   // 手写双层循环
来源：http://zbi.feifeiyinyue.top

Ruby: nested.flatten
来源：http://uee.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bzf.hammf.cn

[D19] 按字段分组
来源：http://xcb.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uum.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hyt.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sos.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lwe.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://leb.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://qwh.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://sii.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://awa.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://ahh.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://eeo.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://sup.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aaq.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqe.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ddk.vehdjk.com

Go:   // 手写 map[T]int
来源：http://hhr.yj20258888.top

Ruby: arr.tally
来源：http://nyi.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xil.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://emm.jinqigfzy.top

Py:   x in arr
来源：http://ydw.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://nrq.meibo888.top

JS:   arr.includes(x)
来源：http://pnu.ivvv.top

TS:   arr.includes(x)
来源：http://pos.ehwqpu.com

Java: list.contains(x)
来源：http://goi.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://efw.gogol.net.cn

Ruby: arr.include?(x)
来源：http://fph.jiagoushi.top

C#:   list.Contains(x)
来源：http://jqm.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://skh.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blm.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yiu.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvb.bbcook.cn

TS:   [...arr];
来源：http://gvb.xylfe.cn

Java: new ArrayList<>(list);
来源：http://qvs.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://mzj.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://zwg.nanxuanxn.top

C#:   new List<int>(list);
来源：http://zap.cashguo.top

[D23] reduce 累积计算
来源：http://dyh.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iua.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dwn.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfm.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rdx.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kla.ivvv.top

Go:   // 手写循环
来源：http://srr.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nct.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ppw.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://jrn.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tgk.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://arz.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vcz.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qvn.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ugr.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rjg.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qjb.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ipf.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://tsy.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://shy.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ola.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nli.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gbs.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pfj.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tng.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kps.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://msn.redwolf501.top

[D26] 数组转字符串
来源：http://jas.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://vlm.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://baz.ehwqpu.com

JS:   arr.join(", ")
来源：http://bcp.jiagoushi.top

TS:   arr.join(", ")
来源：http://ujg.dashuyun.cn

Java: String.join(", ", list)
来源：http://opk.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://ofv.guannengcc.top

Ruby: arr.join(", ")
来源：http://wkr.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://ext.gaohongyu789.top

================================================================================
来源：http://ngn.cqqwz.cn

E. 字符串处理
来源：http://llv.guowangkeji.top

================================================================================
来源：http://iey.xylfe.cn

[E01] 拼接字符串
来源：http://toz.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lsc.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vac.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyo.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uef.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://idb.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pqx.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wcv.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://smv.chenjidiqi.icu

[E02] 重复字符串
来源：http://miv.ybcxt.top

Py:   "ab" * 3
来源：http://pwu.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://dtq.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://zxw.yj202588.top

TS:   "ab".repeat(3)
来源：http://fue.daxiang520.top

Java: "ab".repeat(3)
来源：http://dpj.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://ykt.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://hdz.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvd.tian-w.cn

[E03] 截取子串
来源：http://fiy.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uos.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vfv.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mpm.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://tbb.sweek.top

Java: s.substring(1, 4)
来源：http://hwc.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lzk.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wlm.hammf.cn

C#:   s.Substring(1, 3)
来源：http://yfm.birdmap.top

[E04] 查找子串位置
来源：http://lns.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://skx.52xcode.cn

PHP:  strpos($s, "x");
来源：http://vxv.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wqe.smart0.xyz

TS:   s.indexOf("x")
来源：http://poy.aibaodan.cn

Java: s.indexOf("x")
来源：http://jxu.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://yko.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://dkj.sysykeji.top

C#:   s.IndexOf("x")
来源：http://rnu.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qah.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pds.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://btx.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnw.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://hqw.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whg.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tzg.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ayp.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wta.havefunace.top

[E06] 替换子串
来源：http://sok.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jng.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://efy.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfr.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://lqa.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xqv.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cez.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dig.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://kpt.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://beb.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ous.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ukz.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fiy.jqgufenzy.top

TS:   s.split(",")
来源：http://ctb.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://drq.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://udd.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://obl.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hlp.yueranfly.top

[E08] 数组按分隔符合并
来源：http://buq.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://aod.tarul.cn

PHP:  implode(",", $items);
来源：http://hag.daxiang520.top

JS:   items.join(",")
来源：http://ioq.cucudq.cn

TS:   items.join(",")
来源：http://ual.shzxlz.cn

Java: String.join(",", items)
来源：http://gfg.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://aof.ctjpmb.com

Ruby: items.join(",")
来源：http://tbj.c1oappe.top

C#:   string.Join(",", items)
来源：http://inm.yonumen.top

[E09] 去除所有空白字符
来源：http://rwp.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xmq.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bgf.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://gax.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://vlr.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://zwg.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wfp.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://qmc.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://obh.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://eup.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ymw.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yup.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://jwf.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://jkk.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://tkj.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://dfo.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udx.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vdj.zhoulong.xyz

[E11] 反转字符串
来源：http://wms.haohaochexian.top

Py:   s[::-1]
来源：http://hhz.aizwys.cn

PHP:  strrev($s);
来源：http://dcj.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://hld.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://ipu.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dct.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fqm.yj202588.top

Ruby: s.reverse
来源：http://hmn.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://drq.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://fgg.jinqigfzy.top

Py:   s.count("a")
来源：http://vsk.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://kzd.ydzc1.top

JS:   s.split("a").length - 1
来源：http://kxe.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://fgo.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azk.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://ekr.feifeiyinyue.top

Ruby: s.count("a")
来源：http://jaz.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://zag.pycfn.com

[E13] 逐字符遍历
来源：http://zhr.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://oyt.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pnw.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vff.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cdr.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ywg.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cci.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vqb.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evc.fktsv.cn

[E14] URL 编码与 Base64
来源：http://lag.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zba.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rna.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qgq.52xcode.cn


<!-- 参考信息 -->