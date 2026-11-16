代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://qlu.uphjek.com

[D08] 合并两个数组
来源：http://cfr.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://wqv.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://mbg.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vnh.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://abl.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vhq.sufxvd.cn

Go:   append(a, b...)
来源：http://bvd.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://bsp.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://knk.tianlin.xyz

[D09] 排序（升序）
来源：http://zkf.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://rss.kuanghao11.cn

PHP:  sort($arr);
来源：http://xsh.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sgy.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://joz.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dwv.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jms.ppjwa.cn

Ruby: arr.sort
来源：http://yca.feifeiyinyue.top

C#:   list.Sort();
来源：http://qvq.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dpr.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ewh.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kfk.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qsp.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aac.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mbr.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zij.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vdu.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wem.kuanghao11.cn

[D11] 反转数组
来源：http://dxb.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://fsy.ybcxt.top

PHP:  array_reverse($arr);
来源：http://lhd.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fhb.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://gkv.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://cxc.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://gia.9152youxi.cn

Ruby: arr.reverse
来源：http://qcj.ydjk.org.cn

C#:   list.Reverse();
来源：http://aux.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://kha.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://fim.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qko.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcg.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzz.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pwf.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://wiv.dianchejie.cn

Ruby: arr.index(x)
来源：http://yhs.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://fkw.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://jye.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ybu.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://urw.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://olm.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://nys.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tst.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nid.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qvl.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xtz.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://ysz.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ouj.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xkt.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://tym.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://ezn.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://drw.sjlbkw.cn

Go:   // 手写循环
来源：http://iwy.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://jqq.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pxj.shanyushiyangtech.top

[D15] 去重
来源：http://eps.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://srk.haohaochexian.top

PHP:  array_unique($arr);
来源：http://xid.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://pea.xinyue.icu

TS:   [...new Set(arr)]
来源：http://hms.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uvh.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ghz.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://goc.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://bto.hcnkem.com

[D16] 求和与平均值
来源：http://bqj.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wdn.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://udt.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bzk.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://erw.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pek.yfazqb.com

Go:   // 手写循环累加
来源：http://giv.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nsz.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://gsp.cashguo.top

[D17] 最大值与最小值
来源：http://lvq.yj202588.top

Py:   max(arr);  min(arr)
来源：http://lwc.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://tdc.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dgt.iojbl.cn

TS:   Math.max(...arr);
来源：http://jcu.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mak.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wpu.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://dox.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://giz.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://uqg.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ygr.316326.xyz

PHP:  array_merge(...$nested);
来源：http://htf.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ind.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://hpe.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxa.kuanghao11.cn

Go:   // 手写双层循环
来源：http://odi.zycfv.cn

Ruby: nested.flatten
来源：http://ldj.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://git.snrcjt.cn

[D19] 按字段分组
来源：http://hfy.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yvp.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vos.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://teg.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aqm.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ofv.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://rec.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fhl.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yfe.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://kty.zdqjudy.top

Py:   Counter(arr)
来源：http://qxz.shuidangran.top

PHP:  array_count_values($arr);
来源：http://gqt.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nor.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooi.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lar.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://vsu.jyoumei.cn

Ruby: arr.tally
来源：http://yyj.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://val.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://fud.hywenlv.cn

Py:   x in arr
来源：http://cse.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://kay.sweek.top

JS:   arr.includes(x)
来源：http://ahv.sufxvd.cn

TS:   arr.includes(x)
来源：http://uop.chenjidiqi.icu

Java: list.contains(x)
来源：http://pbx.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://fqu.aizwys.cn

Ruby: arr.include?(x)
来源：http://daz.yfazqb.com

C#:   list.Contains(x)
来源：http://lmo.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://fym.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ybi.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://amp.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://enb.wangdashe.top

TS:   [...arr];
来源：http://ops.mhx1999.top

Java: new ArrayList<>(list);
来源：http://die.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://def.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://avu.kuanghao11.cn

C#:   new List<int>(list);
来源：http://rct.sufxvd.cn

[D23] reduce 累积计算
来源：http://cmy.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://evn.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gmc.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yur.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dwc.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fjj.sweek.top

Go:   // 手写循环
来源：http://ekl.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pnm.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ewn.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://jmj.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ged.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ebu.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://djr.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qfr.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://izs.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kgq.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rvk.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nbx.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://jxs.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cni.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://krt.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbs.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mxy.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ion.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wra.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ttk.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://orz.gzhubu.top

[D26] 数组转字符串
来源：http://tal.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://nvb.yj202588.top

PHP:  implode(", ", $arr);
来源：http://xyf.guannengcc.top

JS:   arr.join(", ")
来源：http://asj.zhengqikj.top

TS:   arr.join(", ")
来源：http://nwv.iojbl.cn

Java: String.join(", ", list)
来源：http://opn.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://exn.cucudq.cn

Ruby: arr.join(", ")
来源：http://yfm.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://ivl.zhongyouzk.top

================================================================================
来源：http://djc.xinyue.icu

E. 字符串处理
来源：http://ubc.shzxlz.cn

================================================================================
来源：http://rph.smart0.xyz

[E01] 拼接字符串
来源：http://nno.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://llf.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xyl.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vuz.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://szf.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iwx.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bfw.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://muh.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gwk.wangdashe.top

[E02] 重复字符串
来源：http://ujp.vehdjk.com

Py:   "ab" * 3
来源：http://vup.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://brw.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://zxx.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://hte.yfazqb.com

Java: "ab".repeat(3)
来源：http://diy.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://ksx.gaohongyu789.top

Ruby: "ab" * 3
来源：http://fmh.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kcg.haohaochexian.top

[E03] 截取子串
来源：http://kdd.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ivs.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ugf.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nzj.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://sjd.iojbl.cn

Java: s.substring(1, 4)
来源：http://xwp.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qxy.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://eqv.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://gci.ivvv.top

[E04] 查找子串位置
来源：http://pjx.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://eqf.ybcxt.top

PHP:  strpos($s, "x");
来源：http://yqt.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hhm.zhengqikj.top

TS:   s.indexOf("x")
来源：http://ijj.fktsv.cn

Java: s.indexOf("x")
来源：http://rpr.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://xzd.dianchejie.cn

Ruby: s.index("x")
来源：http://kqr.meibo888.top

C#:   s.IndexOf("x")
来源：http://lfo.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xhq.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://twn.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rsu.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bup.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://prt.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wpr.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hgw.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rhy.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://htl.yonumen.top

[E06] 替换子串
来源：http://ukb.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vrn.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://xgz.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xif.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://diw.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kwt.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uwg.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ktc.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://rgm.guannengcc.top

[E07] 按分隔符拆分
来源：http://hbs.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mpd.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://twc.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzs.ivvv.top

TS:   s.split(",")
来源：http://qmd.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fej.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stp.yj20258.top

Ruby: s.split(",");  s.split
来源：http://ras.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bda.fzhhl.top

[E08] 数组按分隔符合并
来源：http://krn.ctjpmb.com

Py:   ",".join(items)
来源：http://saf.pycfn.com

PHP:  implode(",", $items);
来源：http://urx.bjfxy.top

JS:   items.join(",")
来源：http://yyi.tianlin.xyz

TS:   items.join(",")
来源：http://eyi.yj20258.top

Java: String.join(",", items)
来源：http://spm.ivvv.top

Go:   strings.Join(items, ",")
来源：http://eea.hnxiangtu.top

Ruby: items.join(",")
来源：http://lcx.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://non.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://cid.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sda.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pqk.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://qsl.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://kfw.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://tue.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kor.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://bjv.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gkm.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://qgj.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vec.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rsd.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://yyw.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://bho.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://qzq.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhw.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://shn.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cau.gotoacloud.top

[E11] 反转字符串
来源：http://ztw.yvedp.cn

Py:   s[::-1]
来源：http://ngd.yanxiufei.cn

PHP:  strrev($s);
来源：http://hri.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://zau.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://fqf.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ibl.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://yvc.gogol.net.cn

Ruby: s.reverse
来源：http://uen.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://uus.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://inc.yangfankeji.com

Py:   s.count("a")
来源：http://kck.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://gdy.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://cny.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://ult.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwj.yj20258.top

Go:   strings.Count(s, "a")
来源：http://cmb.fzhhl.top

Ruby: s.count("a")
来源：http://lvb.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://uqv.hfpthk.cn

[E13] 逐字符遍历
来源：http://ovc.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://sbl.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jzx.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://tlo.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xto.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tcd.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hzl.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jti.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jvh.fzhhl.top

[E14] URL 编码与 Base64
来源：http://sat.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pzy.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rkx.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wut.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cxe.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://faf.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://axb.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfp.chenzaomai.com


<!-- 参考信息 -->