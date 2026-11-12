代发 wailian999

PHP:  sort($arr);
来源：http://yyj.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jej.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://mzj.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rwz.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bkv.kuanghao11.cn

Ruby: arr.sort
来源：http://hql.guowangkeji.top

C#:   list.Sort();
来源：http://lgr.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xpf.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cnd.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybc.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gpr.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhb.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dgr.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yft.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnp.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jfu.yfazqb.com

[D11] 反转数组
来源：http://awn.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://tyu.ybcxt.top

PHP:  array_reverse($arr);
来源：http://skv.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkj.hcnkem.com

TS:   [...arr].reverse();
来源：http://htv.hammf.cn

Java: Collections.reverse(list);
来源：http://kof.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://ltv.zhongyouzk.top

Ruby: arr.reverse
来源：http://vyj.ivvv.top

C#:   list.Reverse();
来源：http://rco.wangshuangyany.cn

[D12] 查找元素下标
来源：http://nrw.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://svz.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xyr.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tcs.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://btn.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bst.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://vrs.hfpthk.cn

Ruby: arr.index(x)
来源：http://oqf.hcnkem.com

C#:   list.IndexOf(x);
来源：http://auo.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://mrq.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rkb.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zse.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://dgd.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://mfu.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://seo.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kjx.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://dih.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qcs.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://czc.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qky.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vuz.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://lem.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://cfd.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fmr.tarul.cn

Go:   // 手写循环
来源：http://xcr.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://vcs.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://goo.hcnkem.com

[D15] 去重
来源：http://wpr.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rqf.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://tyh.yj20258888.top

JS:   [...new Set(arr)]
来源：http://yaw.fzhhl.top

TS:   [...new Set(arr)]
来源：http://llp.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jrw.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://asj.jyoumei.cn

Ruby: arr.uniq
来源：http://cmb.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://cnl.shuidangran.top

[D16] 求和与平均值
来源：http://nyj.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hun.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://krd.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://snj.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkp.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ppw.dianchejie.cn

Go:   // 手写循环累加
来源：http://xef.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emt.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://jnx.xylfe.cn

[D17] 最大值与最小值
来源：http://tsn.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://cem.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://mhz.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kdd.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://uwj.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zud.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nbc.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://vxe.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://jme.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://zfd.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tlq.yj202588.top

PHP:  array_merge(...$nested);
来源：http://hwe.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uwz.feifeiyinyue.top

TS:   nested.flat();
来源：http://kdi.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rxn.yj202588.top

Go:   // 手写双层循环
来源：http://gjw.hongshengwenyu.top

Ruby: nested.flatten
来源：http://lvb.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gop.dianchejie.cn

[D19] 按字段分组
来源：http://nuw.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zqx.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dtz.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nci.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dsa.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://knu.yj202588.top

Go:   // 手写 map[string][]T
来源：http://zlx.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gfj.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xsu.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://yja.snrcjt.cn

Py:   Counter(arr)
来源：http://xkf.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://isc.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prf.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oto.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gln.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://rrr.9152youxi.cn

Ruby: arr.tally
来源：http://vaq.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://usl.havefunace.top

[D21] 判断是否包含某元素
来源：http://xku.aibaodan.cn

Py:   x in arr
来源：http://tqq.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://gnl.vqdsnc.cn

JS:   arr.includes(x)
来源：http://gci.quarkkingdee.top

TS:   arr.includes(x)
来源：http://qyw.sysykeji.top

Java: list.contains(x)
来源：http://ejd.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://zah.cqqwz.cn

Ruby: arr.include?(x)
来源：http://vel.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://vzn.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://msk.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ugj.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uig.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wqa.jqgfzy.top

TS:   [...arr];
来源：http://auk.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://tfi.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wgj.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://atv.shzxlz.cn

C#:   new List<int>(list);
来源：http://sys.jiagoushi.top

[D23] reduce 累积计算
来源：http://frd.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iqy.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aqr.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://odg.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipl.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://tpt.cucudq.cn

Go:   // 手写循环
来源：http://kdn.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xqc.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xsd.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://dsk.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gmc.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yru.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yge.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://frq.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wod.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://big.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qkv.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qqj.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://dzu.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tyq.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdy.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kod.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nej.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ret.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://his.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rnz.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bdx.zhijiandao.cn

[D26] 数组转字符串
来源：http://uwe.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://hyq.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://ndx.shuidangran.top

JS:   arr.join(", ")
来源：http://qny.hnqzz.top

TS:   arr.join(", ")
来源：http://kka.yuanzhike.top

Java: String.join(", ", list)
来源：http://qig.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://rjf.316326.xyz

Ruby: arr.join(", ")
来源：http://iwv.hcnkem.com

C#:   string.Join(", ", list)
来源：http://rdk.yj202588.top

================================================================================
来源：http://bgs.cqqwz.cn

E. 字符串处理
来源：http://vrd.shanyushiyangkeji.top

================================================================================
来源：http://wck.0kj1m.cn

[E01] 拼接字符串
来源：http://tnk.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qou.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://abl.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ykm.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vju.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gde.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://btx.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cyh.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mwr.shuidangran.top

[E02] 重复字符串
来源：http://qtw.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://vji.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://htn.hcnkem.com

JS:   "ab".repeat(3)
来源：http://pad.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://pyh.yangfankeji.com

Java: "ab".repeat(3)
来源：http://rwr.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://pcj.pycfn.com

Ruby: "ab" * 3
来源：http://ymi.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ouw.quarkkingdee.top

[E03] 截取子串
来源：http://dsw.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ums.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://crl.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rnr.mhx1999.top

TS:   s.slice(1, 4)
来源：http://qrn.cdnleiting.top

Java: s.substring(1, 4)
来源：http://fur.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kzk.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hfc.havefunace.top

C#:   s.Substring(1, 3)
来源：http://lcz.mhx1999.top

[E04] 查找子串位置
来源：http://pxd.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://xrb.vehdjk.com

PHP:  strpos($s, "x");
来源：http://rog.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wte.daxiang520.top

TS:   s.indexOf("x")
来源：http://qjl.yangfankeji.com

Java: s.indexOf("x")
来源：http://sfi.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://evu.chenjidiqi.icu

Ruby: s.index("x")
来源：http://qpw.redwolf501.top

C#:   s.IndexOf("x")
来源：http://uxy.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kue.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rqk.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fvp.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbu.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jwo.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygr.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://urz.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ihq.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://obs.andypj.xyz

[E06] 替换子串
来源：http://mwb.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ibd.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://szk.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ili.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://tnu.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bvi.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jyw.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ktd.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://xxi.meibo888.top

[E07] 按分隔符拆分
来源：http://srm.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vhu.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wyf.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bit.sysykeji.top

TS:   s.split(",")
来源：http://ixn.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zbf.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cso.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://ucp.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uty.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://rnv.birdmap.top

Py:   ",".join(items)
来源：http://nkk.shuidangran.top

PHP:  implode(",", $items);
来源：http://vpj.kuanghao11.cn

JS:   items.join(",")
来源：http://caa.quarkkingdee.top

TS:   items.join(",")
来源：http://zfp.dianchejie.cn

Java: String.join(",", items)
来源：http://fxd.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://eje.cqqwz.cn

Ruby: items.join(",")
来源：http://tjp.dashuyun.cn

C#:   string.Join(",", items)
来源：http://ksk.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://pyj.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kvz.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qak.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://jou.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://dfa.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://gvb.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bzd.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://jzq.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qxo.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://lrc.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pdz.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qeu.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://nta.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://zrr.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://bbj.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dak.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lcz.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zvt.quarkkingdee.top

[E11] 反转字符串
来源：http://joo.cashguo.top

Py:   s[::-1]
来源：http://ffb.yfazqb.com

PHP:  strrev($s);
来源：http://tem.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://uqm.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://lxr.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lqj.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dmg.zhiwuduotai.top

Ruby: s.reverse
来源：http://kqw.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://ipk.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://htt.jinghuilouyu.cn

Py:   s.count("a")
来源：http://fza.tarul.cn

PHP:  substr_count($s, "a");
来源：http://yox.vehdjk.com

JS:   s.split("a").length - 1
来源：http://cga.havefunace.top

TS:   s.split("a").length - 1
来源：http://sln.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hrv.gogol.net.cn

Go:   strings.Count(s, "a")
来源：http://ois.yueranfly.top

Ruby: s.count("a")
来源：http://pwy.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://iut.haohaochexian.top

[E13] 逐字符遍历
来源：http://nhh.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://ryq.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://krk.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mer.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://fla.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wqm.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sti.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://xep.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nzt.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://hee.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sgk.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ndo.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yac.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mqj.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vgs.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bms.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvf.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rwx.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://mnj.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://emr.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fag.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jtd.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tae.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mfh.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qgz.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://het.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oap.gzhubu.top

[E16] 数字千分位
来源：http://evh.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://jcn.hysaishi.cn


<!-- 参考信息 -->