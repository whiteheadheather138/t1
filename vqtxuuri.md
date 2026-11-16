代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://ubm.jianghu66.top

TS:   [...a, ...b];
来源：http://mlk.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xmq.nanxinkj.top

Go:   append(a, b...)
来源：http://oba.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://woi.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://drb.nanxuanxn.top

[D09] 排序（升序）
来源：http://zag.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://wam.zhiwuduotai.top

PHP:  sort($arr);
来源：http://oox.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bul.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rbo.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://oym.hongshengwenyu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zhv.iojbl.cn

Ruby: arr.sort
来源：http://uxc.yj202588.top

C#:   list.Sort();
来源：http://oiy.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://whj.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kug.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qto.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ddp.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xah.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kgo.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ivf.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vxi.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hdf.zhongyouzk.top

[D11] 反转数组
来源：http://ypz.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://knn.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://pid.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lmz.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://tvg.cucudq.cn

Java: Collections.reverse(list);
来源：http://egv.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://tyw.cqqwz.cn

Ruby: arr.reverse
来源：http://vjq.xuetiantiany.cn

C#:   list.Reverse();
来源：http://ijq.guowangkeji.top

[D12] 查找元素下标
来源：http://ano.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://avl.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uvc.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vtc.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uyw.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://poi.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://vvv.ppjwa.cn

Ruby: arr.index(x)
来源：http://acj.smart0.xyz

C#:   list.IndexOf(x);
来源：http://fnl.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://lto.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wzy.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wow.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://npv.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://tjz.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hfr.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://apa.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://vlw.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hxl.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://cqo.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://swb.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dpa.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://rwb.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://iru.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hzh.daxiang520.top

Go:   // 手写循环
来源：http://amw.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hqu.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wlf.sufxvd.cn

[D15] 去重
来源：http://onz.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sem.ehwqpu.com

PHP:  array_unique($arr);
来源：http://fix.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://afv.epnwcf.com

TS:   [...new Set(arr)]
来源：http://cyd.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yok.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tpz.0kj1m.cn

Ruby: arr.uniq
来源：http://xhb.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://cfi.gogol.net.cn

[D16] 求和与平均值
来源：http://tyi.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yqt.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://awu.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sox.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkn.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljv.yj20258888.top

Go:   // 手写循环累加
来源：http://qcf.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rww.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://ovh.yuanzhike.top

[D17] 最大值与最小值
来源：http://uej.316326.xyz

Py:   max(arr);  min(arr)
来源：http://qly.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://mnk.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yhw.yueranfly.top

TS:   Math.max(...arr);
来源：http://wsr.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ipm.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tpv.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://sys.sweek.top

C#:   list.Max();  list.Min()
来源：http://ttn.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://qth.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sdm.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://ate.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbl.zhongyouzk.top

TS:   nested.flat();
来源：http://fvz.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zma.yj202588.top

Go:   // 手写双层循环
来源：http://sww.yj20258888.top

Ruby: nested.flatten
来源：http://wdg.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mza.tanke756.top

[D19] 按字段分组
来源：http://kmd.shzxlz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fzk.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ean.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://olc.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mse.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kje.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://eqd.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cbr.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wyh.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://npt.gzhubu.top

Py:   Counter(arr)
来源：http://nqp.ydzc1.top

PHP:  array_count_values($arr);
来源：http://euw.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pfn.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bwe.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lfr.pycfn.com

Go:   // 手写 map[T]int
来源：http://qpp.vqdsnc.cn

Ruby: arr.tally
来源：http://yqy.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lkd.gzhubu.top

[D21] 判断是否包含某元素
来源：http://mji.0kj1m.cn

Py:   x in arr
来源：http://lvw.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://szk.cashguo.top

JS:   arr.includes(x)
来源：http://jce.9152youxi.cn

TS:   arr.includes(x)
来源：http://ewn.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://nsj.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://evn.snrcjt.cn

Ruby: arr.include?(x)
来源：http://mkx.yongpay.top

C#:   list.Contains(x)
来源：http://sea.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://wwx.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dbd.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tck.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pxm.cqqwz.cn

TS:   [...arr];
来源：http://auf.mhx1999.top

Java: new ArrayList<>(list);
来源：http://npq.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://jad.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://ldk.wangdashe.top

C#:   new List<int>(list);
来源：http://xhp.yuanzhike.top

[D23] reduce 累积计算
来源：http://cfz.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://unq.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://myv.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ugz.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://drw.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zhl.sxryk.cn

Go:   // 手写循环
来源：http://sqk.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqy.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qff.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://apb.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dic.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dcv.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jln.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://smp.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oca.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mab.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ubh.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dcb.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://oqv.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lgb.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fin.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpc.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://olx.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jsg.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fnr.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bvb.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pez.quarkkingdee.top

[D26] 数组转字符串
来源：http://xaq.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://jji.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://owu.hnqzz.top

JS:   arr.join(", ")
来源：http://oqj.svipenyu.cn

TS:   arr.join(", ")
来源：http://esx.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://ail.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://ydk.yj202588.top

Ruby: arr.join(", ")
来源：http://znx.pycfn.com

C#:   string.Join(", ", list)
来源：http://iss.wangshuangyany.cn

================================================================================
来源：http://ktq.aizwys.cn

E. 字符串处理
来源：http://dsg.pengpengdd.cyou

================================================================================
来源：http://efp.hongshengwenyu.top

[E01] 拼接字符串
来源：http://poc.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://olc.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tif.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yen.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ked.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dwd.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://itv.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lny.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zxy.sjlbkw.cn

[E02] 重复字符串
来源：http://hyd.pengpengdd.cyou

Py:   "ab" * 3
来源：http://wxy.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://mhr.yonumen.top

JS:   "ab".repeat(3)
来源：http://anw.yvedp.cn

TS:   "ab".repeat(3)
来源：http://oea.zdbjq.cn

Java: "ab".repeat(3)
来源：http://fvr.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://aac.pycfn.com

Ruby: "ab" * 3
来源：http://rur.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gbn.vqdsnc.cn

[E03] 截取子串
来源：http://ooc.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qfl.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rfs.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aix.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://qho.ehwqpu.com

Java: s.substring(1, 4)
来源：http://yep.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wdo.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://ety.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://pkb.dashuyun.cn

[E04] 查找子串位置
来源：http://fhj.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://mra.birdmap.top

PHP:  strpos($s, "x");
来源：http://gbh.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kos.gogol.net.cn

TS:   s.indexOf("x")
来源：http://lzh.epnwcf.com

Java: s.indexOf("x")
来源：http://xiw.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://zkg.cashguo.top

Ruby: s.index("x")
来源：http://kjh.zycfv.cn

C#:   s.IndexOf("x")
来源：http://ydw.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://czt.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uwz.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ixl.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ycv.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jcw.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fef.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dhe.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jut.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xnz.cheryme.top

[E06] 替换子串
来源：http://qqn.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tny.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://lim.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fgx.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://fib.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pma.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mts.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://chg.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://lyf.zhixingplan.top

[E07] 按分隔符拆分
来源：http://nvk.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ktt.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qkv.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://auo.zhixingplan.top

TS:   s.split(",")
来源：http://zsk.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://zfm.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mla.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://xep.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hvt.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://bbb.tianlin.xyz

Py:   ",".join(items)
来源：http://wdp.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://ata.quarkkingdee.top

JS:   items.join(",")
来源：http://ofs.chenjidiqi.icu

TS:   items.join(",")
来源：http://zam.hywenlv.cn

Java: String.join(",", items)
来源：http://yym.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://jxy.hnxiangtu.top

Ruby: items.join(",")
来源：http://cod.wangdashe.top

C#:   string.Join(",", items)
来源：http://sfl.redwolf501.top

[E09] 去除所有空白字符
来源：http://hrx.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jry.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nhi.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://ftx.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://wph.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ocp.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zhk.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://aju.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hhf.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://wpn.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mon.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lux.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://bnm.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://qpw.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://etb.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tqw.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://arw.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hjx.yangfankeji.com

[E11] 反转字符串
来源：http://naj.nanxuanxn.top

Py:   s[::-1]
来源：http://lii.nanxinkj.top

PHP:  strrev($s);
来源：http://ndn.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://djf.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://ptc.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://keg.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lqa.shanyushiyangtech.top

Ruby: s.reverse
来源：http://nfk.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://oen.iojbl.cn

[E12] 统计某字符出现次数
来源：http://hed.ctjpmb.com

Py:   s.count("a")
来源：http://hus.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://lzr.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://pxi.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://bce.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://amh.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://qsg.snrcjt.cn

Ruby: s.count("a")
来源：http://uva.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://ldk.yangfankeji.com

[E13] 逐字符遍历
来源：http://qpm.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://bee.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://isa.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zcm.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://shb.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aba.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ecp.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://brk.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ner.mhx1999.top

[E14] URL 编码与 Base64
来源：http://dxn.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pdf.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://guk.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hqn.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zbl.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kuj.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hed.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://srm.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://doj.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://vld.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dyd.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nle.nanxinkj.top


<!-- 参考信息 -->