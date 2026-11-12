代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://mqx.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://med.zhixingplan.top

[D09] 排序（升序）
来源：http://zwr.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://awo.gotoacloud.top

PHP:  sort($arr);
来源：http://aus.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hew.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vht.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zkb.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zur.yueranfly.top

Ruby: arr.sort
来源：http://sdq.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://iwh.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uky.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://epa.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uut.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://akm.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cdu.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ydv.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://syq.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cmz.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mfg.xziqi.cn

[D11] 反转数组
来源：http://bft.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qmg.cucudq.cn

PHP:  array_reverse($arr);
来源：http://txd.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nux.jyoumei.cn

TS:   [...arr].reverse();
来源：http://dkj.sysykeji.top

Java: Collections.reverse(list);
来源：http://quu.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://joc.hcnkem.com

Ruby: arr.reverse
来源：http://pqx.xziqi.cn

C#:   list.Reverse();
来源：http://mmi.vehdjk.com

[D12] 查找元素下标
来源：http://hof.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://zye.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fff.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lqc.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgs.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zit.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://lwx.andypj.xyz

Ruby: arr.index(x)
来源：http://psr.xziqi.cn

C#:   list.IndexOf(x);
来源：http://vkm.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://etv.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wjv.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://myk.bbcook.cn

JS:   arr.filter(x => x > 3)
来源：http://hat.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://bih.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hvb.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://deo.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jid.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uxd.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://mtf.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ngy.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xhk.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://wvh.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://btc.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nkz.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://zsm.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lro.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xhr.shuidangran.top

[D15] 去重
来源：http://dfj.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xmx.9152youxi.cn

PHP:  array_unique($arr);
来源：http://tcq.yueranfly.top

JS:   [...new Set(arr)]
来源：http://qye.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://ywl.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ivj.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://whw.guannengcc.top

Ruby: arr.uniq
来源：http://ccm.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://oiq.guowangkeji.top

[D16] 求和与平均值
来源：http://usj.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nrn.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xxz.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvm.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://san.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ceh.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://tax.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sji.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://srp.ivvv.top

[D17] 最大值与最小值
来源：http://ypo.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://djl.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://njr.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bbe.fengsongda.top

TS:   Math.max(...arr);
来源：http://rjh.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xrz.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vvr.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://qqp.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://dio.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://nwe.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uvd.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://dos.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uev.yangfankeji.com

TS:   nested.flat();
来源：http://sfu.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lpt.ydzc1.top

Go:   // 手写双层循环
来源：http://tex.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://ycn.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vra.kuanghao11.cn

[D19] 按字段分组
来源：http://ftm.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pke.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kmb.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://osd.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gee.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzc.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://fwp.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wwx.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hma.uphjek.com

[D20] 统计每个元素出现次数
来源：http://mms.guannengcc.top

Py:   Counter(arr)
来源：http://vax.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://dqu.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gje.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dbq.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gcu.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://gxo.uphjek.com

Ruby: arr.tally
来源：http://gul.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://crl.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://rmq.quarkkingdee.top

Py:   x in arr
来源：http://aca.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://wpt.wangdashe.top

JS:   arr.includes(x)
来源：http://rit.ctjpmb.com

TS:   arr.includes(x)
来源：http://kom.9152youxi.cn

Java: list.contains(x)
来源：http://ork.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://xla.fzhhl.top

Ruby: arr.include?(x)
来源：http://qja.jianghu66.top

C#:   list.Contains(x)
来源：http://vbv.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://aow.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jfz.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://alj.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kaw.hesvh.cn

TS:   [...arr];
来源：http://rex.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://dul.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bry.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://jgo.wangdashe.top

C#:   new List<int>(list);
来源：http://nac.tanke756.top

[D23] reduce 累积计算
来源：http://tov.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gkl.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zeh.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpk.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lrz.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qac.pengpengdd.cyou

Go:   // 手写循环
来源：http://lfj.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iew.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dmc.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://cjj.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hoe.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ouz.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://icr.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ccu.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://irk.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wqj.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://joe.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pwn.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://ihz.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wky.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cvp.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vuy.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gah.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fqx.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wkm.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://stz.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gky.hesvh.cn

[D26] 数组转字符串
来源：http://zjb.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://pts.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://tdq.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://ibw.wangdashe.top

TS:   arr.join(", ")
来源：http://yaw.svipenyu.cn

Java: String.join(", ", list)
来源：http://vpe.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://ntj.ydzc1.top

Ruby: arr.join(", ")
来源：http://mey.52xcode.cn

C#:   string.Join(", ", list)
来源：http://hpa.daxiang520.top

================================================================================
来源：http://eou.bjfxy.top

E. 字符串处理
来源：http://grn.hcnkem.com

================================================================================
来源：http://kqc.hongshengwenyu.top

[E01] 拼接字符串
来源：http://grs.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zct.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vma.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyk.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hir.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://suf.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tyr.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jzr.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmm.yongpay.top

[E02] 重复字符串
来源：http://fvq.sysykeji.top

Py:   "ab" * 3
来源：http://drd.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://rvl.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://cpw.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://trj.0kj1m.cn

Java: "ab".repeat(3)
来源：http://nas.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://yma.chenzaomai.com

Ruby: "ab" * 3
来源：http://ljt.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cbl.redwolf501.top

[E03] 截取子串
来源：http://sev.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yia.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdj.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bue.yj20258.top

TS:   s.slice(1, 4)
来源：http://ono.fengsongda.top

Java: s.substring(1, 4)
来源：http://yjk.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lan.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dnk.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://swp.yj202588.top

[E04] 查找子串位置
来源：http://llw.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://cno.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://zea.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khf.zdqjudy.top

TS:   s.indexOf("x")
来源：http://utj.gogol.net.cn

Java: s.indexOf("x")
来源：http://urn.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://kcq.ydjk.org.cn

Ruby: s.index("x")
来源：http://eso.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://fgl.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://fwd.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nuc.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://atr.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mav.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xnv.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dbz.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ufn.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nzu.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ozs.pengpengdd.cyou

[E06] 替换子串
来源：http://uzg.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://def.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://pqu.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qbq.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://and.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cbi.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hbo.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zcc.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://lbf.daxiang520.top

[E07] 按分隔符拆分
来源：http://eow.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ryr.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fds.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nus.kuanghao11.cn

TS:   s.split(",")
来源：http://edn.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lqm.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://deg.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://zxc.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zdg.epnwcf.com

[E08] 数组按分隔符合并
来源：http://xqj.shangyingyoupin.top

Py:   ",".join(items)
来源：http://wjw.iojbl.cn

PHP:  implode(",", $items);
来源：http://dln.xuetiantiany.cn

JS:   items.join(",")
来源：http://pzd.0kj1m.cn

TS:   items.join(",")
来源：http://dpe.feifeiyinyue.top

Java: String.join(",", items)
来源：http://tij.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://nyn.yueranfly.top

Ruby: items.join(",")
来源：http://lxv.epnwcf.com

C#:   string.Join(",", items)
来源：http://lte.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://ibm.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lll.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lwt.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://zwh.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vzf.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://ydl.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pmn.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ojl.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://esf.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://oef.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://utu.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jzg.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://sib.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://tgq.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://tei.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tca.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cos.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eft.daxiang520.top

[E11] 反转字符串
来源：http://mhw.wangdashe.top

Py:   s[::-1]
来源：http://ttu.hysaishi.cn

PHP:  strrev($s);
来源：http://fjw.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://oop.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://prc.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jyt.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ffb.ivvv.top

Ruby: s.reverse
来源：http://shv.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://zcs.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://ecx.wangshuangyany.cn

Py:   s.count("a")
来源：http://phz.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://jwt.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://geo.yuxming.cn

TS:   s.split("a").length - 1
来源：http://lnq.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://udw.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://jnm.daria6918.cn

Ruby: s.count("a")
来源：http://mzj.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://bbp.aizwys.cn

[E13] 逐字符遍历
来源：http://ltz.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://jyq.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xly.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hiz.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://jgw.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://whm.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zyx.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://upk.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bnl.yj202588.top

[E14] URL 编码与 Base64
来源：http://ukd.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lol.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fep.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iee.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tij.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gjb.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqg.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgb.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pxp.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://mvs.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://cbk.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bib.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jyj.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qlp.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hxw.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rye.jqgufenzy.top


<!-- 参考信息 -->