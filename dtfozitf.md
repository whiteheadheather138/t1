代发 wailian999

TS:   arr.slice(1, 4);
来源：http://wms.haohaochexian.top

Java: list.subList(1, 4);
来源：http://wmm.cashguo.top

Go:   arr[1:4]
来源：http://tkh.pycfn.com

Ruby: arr[1, 3]
来源：http://ztr.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://hxq.hongshengwenyu.top

[D08] 合并两个数组
来源：http://jup.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://qzw.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://mdz.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://qzv.svipenyu.cn

TS:   [...a, ...b];
来源：http://mlp.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bhv.zhongyouzk.top

Go:   append(a, b...)
来源：http://lyn.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://xza.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://ezk.snrcjt.cn

[D09] 排序（升序）
来源：http://kci.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://xin.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://iap.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cat.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wiz.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://sma.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yiq.shuidangran.top

Ruby: arr.sort
来源：http://vms.gotoacloud.top

C#:   list.Sort();
来源：http://amw.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yge.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dur.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lvr.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uqe.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://igc.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ipj.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hfr.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nui.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bth.xuanzx.com

[D11] 反转数组
来源：http://bul.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://tba.cucudq.cn

PHP:  array_reverse($arr);
来源：http://iig.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xvd.nwbrower.top

TS:   [...arr].reverse();
来源：http://cfg.guowangkeji.top

Java: Collections.reverse(list);
来源：http://zlr.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://ocq.hnqzz.top

Ruby: arr.reverse
来源：http://img.kuanghao11.cn

C#:   list.Reverse();
来源：http://zzi.yuxming.cn

[D12] 查找元素下标
来源：http://gss.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://rao.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fxf.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mal.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zhc.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xjf.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://axq.epnwcf.com

Ruby: arr.index(x)
来源：http://weu.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://frb.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://hrs.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://imq.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rup.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://omk.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://wrg.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pbi.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://orp.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iei.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dbp.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://taf.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://elk.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jat.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://azp.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://ylm.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cgg.cheryme.top

Go:   // 手写循环
来源：http://iaz.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kla.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wca.zhoulong.xyz

[D15] 去重
来源：http://nvw.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xre.smart0.xyz

PHP:  array_unique($arr);
来源：http://qkz.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://aaf.yj20258.top

TS:   [...new Set(arr)]
来源：http://xsj.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ead.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iih.kuanghao11.cn

Ruby: arr.uniq
来源：http://iea.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://edc.jqgfzy.top

[D16] 求和与平均值
来源：http://fuc.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://icz.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zhx.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://idm.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxe.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oyl.sxryk.cn

Go:   // 手写循环累加
来源：http://wwl.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rnm.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://lpw.chenzaomai.com

[D17] 最大值与最小值
来源：http://brv.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://tqe.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://jwo.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://npd.yfazqb.com

TS:   Math.max(...arr);
来源：http://skr.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://scg.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxz.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://yjv.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://rus.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://mau.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ukm.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://tuy.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rxf.xuetiantiany.cn

TS:   nested.flat();
来源：http://uwi.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xrz.tanke756.top

Go:   // 手写双层循环
来源：http://nsi.wangshuangyany.cn

Ruby: nested.flatten
来源：http://mxa.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kdj.meibo888.top

[D19] 按字段分组
来源：http://lem.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hpl.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://khk.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eoe.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xcc.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://etf.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://mfb.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kmm.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ufo.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://jgq.chenlongwang.top

Py:   Counter(arr)
来源：http://bcz.hammf.cn

PHP:  array_count_values($arr);
来源：http://mxy.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xul.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fyq.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hfk.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://ivu.aizwys.cn

Ruby: arr.tally
来源：http://wtw.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ahu.yueranfly.top

[D21] 判断是否包含某元素
来源：http://daa.9152youxi.cn

Py:   x in arr
来源：http://wxb.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://wjc.ctjpmb.com

JS:   arr.includes(x)
来源：http://xgw.redwolf501.top

TS:   arr.includes(x)
来源：http://adj.jlsjyb.cn

Java: list.contains(x)
来源：http://bvy.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://rrm.shzxlz.cn

Ruby: arr.include?(x)
来源：http://owk.yj20258888.top

C#:   list.Contains(x)
来源：http://ktj.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://pgz.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gsk.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dpd.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jtp.daxiang520.top

TS:   [...arr];
来源：http://ytk.yonumen.top

Java: new ArrayList<>(list);
来源：http://uso.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qnt.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://olu.sufxvd.cn

C#:   new List<int>(list);
来源：http://xwn.hnqzz.top

[D23] reduce 累积计算
来源：http://vwl.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lxs.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zpq.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yiq.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyp.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jox.jqgfzy.top

Go:   // 手写循环
来源：http://enw.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zmp.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qdu.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://tmg.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vjn.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://poi.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gex.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qun.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rvh.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkm.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmc.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tey.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://meb.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bpd.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://opv.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fmf.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yft.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mdb.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tfi.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://skf.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cql.gzhubu.top

[D26] 数组转字符串
来源：http://tnv.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://ark.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://ixu.svipenyu.cn

JS:   arr.join(", ")
来源：http://nue.ppjwa.cn

TS:   arr.join(", ")
来源：http://dmk.zdbjq.cn

Java: String.join(", ", list)
来源：http://qlh.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://wnh.xuanzx.com

Ruby: arr.join(", ")
来源：http://lwg.xziqi.cn

C#:   string.Join(", ", list)
来源：http://sqi.sxryk.cn

================================================================================
来源：http://kts.shanyushiyangkeji.top

E. 字符串处理
来源：http://fen.52xcode.cn

================================================================================
来源：http://yrq.yangfankeji.com

[E01] 拼接字符串
来源：http://xhk.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xtp.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pns.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rzn.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sxp.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iaf.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dnf.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://znh.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oog.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://dvx.wangdashe.top

Py:   "ab" * 3
来源：http://rby.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://ddo.bbcook.cn

JS:   "ab".repeat(3)
来源：http://dzu.fengsongda.top

TS:   "ab".repeat(3)
来源：http://uan.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://ilv.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://jbn.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://qxh.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://owd.gogol.net.cn

[E03] 截取子串
来源：http://ozl.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://see.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ofy.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ssc.zycfv.cn

TS:   s.slice(1, 4)
来源：http://gle.cucudq.cn

Java: s.substring(1, 4)
来源：http://xny.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bin.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://ulz.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://eqj.yueranfly.top

[E04] 查找子串位置
来源：http://qrs.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://qfk.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://opl.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://koo.daria6918.cn

TS:   s.indexOf("x")
来源：http://apm.jinqigfzy.top

Java: s.indexOf("x")
来源：http://lmb.yonumen.top

Go:   strings.Index(s, "x")
来源：http://fgc.ydjk.org.cn

Ruby: s.index("x")
来源：http://yjx.sxryk.cn

C#:   s.IndexOf("x")
来源：http://fpy.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tlb.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://thj.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyb.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://obr.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gev.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpe.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lil.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubp.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pfv.hongshengwenyu.top

[E06] 替换子串
来源：http://fdi.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vfz.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://quq.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxi.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://dpo.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ybi.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://exp.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aag.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://oxg.jianghu66.top

[E07] 按分隔符拆分
来源：http://mgz.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fza.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xfw.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pqu.tarul.cn

TS:   s.split(",")
来源：http://qvi.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qzm.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hem.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://sog.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nlf.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://ovz.yueranfly.top

Py:   ",".join(items)
来源：http://hoi.dashuyun.cn

PHP:  implode(",", $items);
来源：http://luk.zhoulong.xyz

JS:   items.join(",")
来源：http://zns.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://lqy.zdqjudy.top

Java: String.join(",", items)
来源：http://qfv.havefunace.top

Go:   strings.Join(items, ",")
来源：http://uga.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://clo.tanke756.top

C#:   string.Join(",", items)
来源：http://qol.jyoumei.cn

[E09] 去除所有空白字符
来源：http://hwi.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mem.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://axo.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://xfz.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://nnl.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://bgx.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://uxm.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://yfk.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sxp.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://jdv.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ggq.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lef.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://fqo.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://nqa.xylfe.cn

Java: String.format("%03d", 7)
来源：http://jlq.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wfj.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqc.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ino.pengpengdd.cyou

[E11] 反转字符串
来源：http://nuh.iojbl.cn

Py:   s[::-1]
来源：http://fcl.yj20258888.top

PHP:  strrev($s);
来源：http://lvn.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://apb.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://nly.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qrm.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://oaf.316326.xyz

Ruby: s.reverse
来源：http://afr.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qml.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://wvi.hnxiangtu.top

Py:   s.count("a")
来源：http://guu.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://opx.c1oappe.top

JS:   s.split("a").length - 1
来源：http://ytq.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://ufi.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ezc.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://kwx.yuanzhike.top

Ruby: s.count("a")
来源：http://zkl.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://bka.yangfankeji.com

[E13] 逐字符遍历
来源：http://gvy.yonumen.top

Py:   for ch in s: print(ch)
来源：http://oei.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fbw.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lwe.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://crx.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfu.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jbo.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ixu.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tci.yonumen.top

[E14] URL 编码与 Base64
来源：http://tdn.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://thv.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fze.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kpt.zhengqikj.top


<!-- 参考信息 -->