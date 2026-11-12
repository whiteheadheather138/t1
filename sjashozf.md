代发 wailian999

TS:   arr.slice(1, 4);
来源：http://qnp.fehbvm.com

Java: list.subList(1, 4);
来源：http://vvi.xinyue.icu

Go:   arr[1:4]
来源：http://bne.nwbrower.top

Ruby: arr[1, 3]
来源：http://jnd.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://btw.cheryme.top

[D08] 合并两个数组
来源：http://pgo.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://qco.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://lff.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dln.cqqwz.cn

TS:   [...a, ...b];
来源：http://stp.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pvq.jqgfzy.top

Go:   append(a, b...)
来源：http://ynu.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://spv.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://tqy.zdbjq.cn

[D09] 排序（升序）
来源：http://aqk.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://tly.cdnleiting.top

PHP:  sort($arr);
来源：http://jtj.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kdk.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gku.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mkh.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bie.sjlbkw.cn

Ruby: arr.sort
来源：http://dit.tian-w.cn

C#:   list.Sort();
来源：http://qku.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hae.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cgg.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qbu.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggb.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rfk.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://phw.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mac.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pmf.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yhp.tian-w.cn

[D11] 反转数组
来源：http://xko.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://dil.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://pby.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cvu.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://txl.daria6918.cn

Java: Collections.reverse(list);
来源：http://ibe.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://pui.pengpengdd.cyou

Ruby: arr.reverse
来源：http://urm.yj202588.top

C#:   list.Reverse();
来源：http://auk.jqgufenzy.top

[D12] 查找元素下标
来源：http://loc.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://ihi.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yri.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyq.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://haq.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lot.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://nhz.sxryk.cn

Ruby: arr.index(x)
来源：http://kkj.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://hbz.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://sdg.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://drb.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wca.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://ley.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://uch.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lfi.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfv.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://wor.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dks.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://yaw.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wfd.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ija.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://ynu.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://syz.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nmh.tarul.cn

Go:   // 手写循环
来源：http://bpq.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://xfi.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nxt.nanxuanxn.top

[D15] 去重
来源：http://aiy.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tll.birdmap.top

PHP:  array_unique($arr);
来源：http://hxs.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://efd.yongpay.top

TS:   [...new Set(arr)]
来源：http://yyc.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqk.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://wik.jyoumei.cn

Ruby: arr.uniq
来源：http://xmi.tanke756.top

C#:   list.Distinct().ToList()
来源：http://ihj.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://bhe.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zgk.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qoa.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://amk.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xfg.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgj.bjfxy.top

Go:   // 手写循环累加
来源：http://wpy.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qiu.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://epb.chenzaomai.com

[D17] 最大值与最小值
来源：http://wcr.yj20258.top

Py:   max(arr);  min(arr)
来源：http://zul.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://zjq.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://smy.iojbl.cn

TS:   Math.max(...arr);
来源：http://efi.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fxf.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tpq.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://gky.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://dha.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://rxx.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lbe.uphjek.com

PHP:  array_merge(...$nested);
来源：http://xkg.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://att.zhengqikj.top

TS:   nested.flat();
来源：http://ltz.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zfq.hesvh.cn

Go:   // 手写双层循环
来源：http://jpm.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://rwf.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wck.bbcook.cn

[D19] 按字段分组
来源：http://mxg.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://juk.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vaz.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubb.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://unr.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qwy.birdmap.top

Go:   // 手写 map[string][]T
来源：http://jhy.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gsb.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://foy.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://fkc.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://tqs.vehdjk.com

PHP:  array_count_values($arr);
来源：http://cxo.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://igr.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzk.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rwo.hcnkem.com

Go:   // 手写 map[T]int
来源：http://yya.hysaishi.cn

Ruby: arr.tally
来源：http://imk.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://job.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://lvi.nanxinkj.top

Py:   x in arr
来源：http://gzu.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://bve.iojbl.cn

JS:   arr.includes(x)
来源：http://kyf.yuxming.cn

TS:   arr.includes(x)
来源：http://scc.yuxming.cn

Java: list.contains(x)
来源：http://zhq.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://bns.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://ptw.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://qqg.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://pxs.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://crb.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xgg.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://syh.fengsongda.top

TS:   [...arr];
来源：http://azd.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://nzv.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wfj.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://uku.yonumen.top

C#:   new List<int>(list);
来源：http://pfj.sxryk.cn

[D23] reduce 累积计算
来源：http://cpl.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://orl.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ohh.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://spn.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fcv.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jaz.ybcxt.top

Go:   // 手写循环
来源：http://iwy.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cgo.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fui.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://zza.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hgy.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ozw.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lxh.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kmp.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrb.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tqf.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jef.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzh.birdmap.top

[D25] Set 集合去重与交并差
来源：http://vkm.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fee.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://opv.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ruj.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zyw.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gdt.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wvp.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvz.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qmg.yangfankeji.com

[D26] 数组转字符串
来源：http://nbf.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://nyv.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://dun.hysaishi.cn

JS:   arr.join(", ")
来源：http://euz.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://nww.daxiang520.top

Java: String.join(", ", list)
来源：http://xcd.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://vuw.ctjpmb.com

Ruby: arr.join(", ")
来源：http://nzn.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://tpc.xingfuxueyuan.xyz

================================================================================
来源：http://drz.daxiang520.top

E. 字符串处理
来源：http://orh.vqdsnc.cn

================================================================================
来源：http://wws.hnxiangtu.top

[E01] 拼接字符串
来源：http://oib.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wgd.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gmt.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjk.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dhz.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nke.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lry.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ino.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lfz.tianlin.xyz

[E02] 重复字符串
来源：http://xnm.c1oappe.top

Py:   "ab" * 3
来源：http://ddc.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://mwn.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://oou.yfazqb.com

TS:   "ab".repeat(3)
来源：http://aff.yongpay.top

Java: "ab".repeat(3)
来源：http://ayg.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://oaq.snrcjt.cn

Ruby: "ab" * 3
来源：http://eia.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yly.xylfe.cn

[E03] 截取子串
来源：http://gkv.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxk.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bzb.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csx.yonumen.top

TS:   s.slice(1, 4)
来源：http://nso.cucudq.cn

Java: s.substring(1, 4)
来源：http://vak.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yuj.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vzg.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://hhc.cqqwz.cn

[E04] 查找子串位置
来源：http://zqk.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://xxo.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://tkc.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tov.hfpthk.cn

TS:   s.indexOf("x")
来源：http://hfj.zhixingplan.top

Java: s.indexOf("x")
来源：http://tbj.pycfn.com

Go:   strings.Index(s, "x")
来源：http://tlf.birdmap.top

Ruby: s.index("x")
来源：http://chg.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://knn.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pyp.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xuh.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eny.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fmk.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lnd.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zlm.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tqf.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ceb.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wzk.chenlongwang.top

[E06] 替换子串
来源：http://kwh.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ukg.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://qxf.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tux.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://bkb.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://koq.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dmk.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vly.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://pwf.xylfe.cn

[E07] 按分隔符拆分
来源：http://zuo.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://osm.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://spt.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wla.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://lrx.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://hoc.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gto.tarul.cn

Ruby: s.split(",");  s.split
来源：http://osc.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://shk.wangdashe.top

[E08] 数组按分隔符合并
来源：http://hao.yongpay.top

Py:   ",".join(items)
来源：http://tkj.yongpay.top

PHP:  implode(",", $items);
来源：http://wbu.andypj.xyz

JS:   items.join(",")
来源：http://unp.hnqzz.top

TS:   items.join(",")
来源：http://sfx.kuanghao11.cn

Java: String.join(",", items)
来源：http://atp.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://kkw.jyoumei.cn

Ruby: items.join(",")
来源：http://twi.xinyue.icu

C#:   string.Join(",", items)
来源：http://kvp.cheryme.top

[E09] 去除所有空白字符
来源：http://mwc.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ros.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nim.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://ekl.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://vny.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://yna.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cwl.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rpv.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vwm.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://qpq.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mom.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mbg.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://itn.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://rno.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://zwc.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aee.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://awr.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bff.zycfv.cn

[E11] 反转字符串
来源：http://zob.guannengcc.top

Py:   s[::-1]
来源：http://ejx.zhiwuduotai.top

PHP:  strrev($s);
来源：http://wbe.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://iar.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://leq.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zds.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ibl.yuxming.cn

Ruby: s.reverse
来源：http://stj.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://edi.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://elo.shangyingyoupin.top

Py:   s.count("a")
来源：http://ywn.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://vaj.hammf.cn

JS:   s.split("a").length - 1
来源：http://jbe.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://aly.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aaa.meibo888.top

Go:   strings.Count(s, "a")
来源：http://vet.epnwcf.com

Ruby: s.count("a")
来源：http://csu.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://swb.zhixingplan.top

[E13] 逐字符遍历
来源：http://vnn.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://ogy.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://imi.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wcu.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xjo.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jsb.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gql.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://agn.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nwn.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://tjs.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tbi.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nbi.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://icw.yuanzhike.top


<!-- 参考信息 -->