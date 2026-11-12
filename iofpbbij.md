代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://nwi.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://omq.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lsk.uphjek.com

[D06] 数组长度
来源：http://xzo.ydzc1.top

Py:   len(arr)
来源：http://reb.52xcode.cn

PHP:  count($arr);
来源：http://cil.ppjwa.cn

JS:   arr.length
来源：http://rzl.jyoumei.cn

TS:   arr.length
来源：http://xjm.jinghuilouyu.cn

Java: list.size();
来源：http://bre.sysykeji.top

Go:   len(arr)
来源：http://jav.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://guu.bbcook.cn

C#:   list.Count;
来源：http://qds.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://twp.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kxj.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://bdb.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://bjd.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://iyu.iojbl.cn

Java: list.subList(1, 4);
来源：http://drz.jiagoushi.top

Go:   arr[1:4]
来源：http://bed.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://xho.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://hof.hesvh.cn

[D08] 合并两个数组
来源：http://tah.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://zyu.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://lzq.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hmw.gaohongyu789.top

TS:   [...a, ...b];
来源：http://lzl.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://enc.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://zgb.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://tmb.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://cbr.gotoacloud.top

[D09] 排序（升序）
来源：http://mzy.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hto.zhixingplan.top

PHP:  sort($arr);
来源：http://zlk.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wde.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kin.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://phh.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hru.dashuyun.cn

Ruby: arr.sort
来源：http://wiq.hammf.cn

C#:   list.Sort();
来源：http://qbw.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://wuz.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zax.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwy.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sqq.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcw.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dbw.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://doy.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://usb.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fxt.ivvv.top

[D11] 反转数组
来源：http://vrl.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://jem.xinyue.icu

PHP:  array_reverse($arr);
来源：http://wdf.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jcd.fehbvm.com

TS:   [...arr].reverse();
来源：http://arv.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://ymy.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://qrd.snrcjt.cn

Ruby: arr.reverse
来源：http://iaj.xuetiantiany.cn

C#:   list.Reverse();
来源：http://mpu.gzhubu.top

[D12] 查找元素下标
来源：http://vle.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://lde.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pzo.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdt.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugr.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czw.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://usv.meibo888.top

Ruby: arr.index(x)
来源：http://wln.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://foy.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://dwr.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwm.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ahu.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://uyg.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://dcc.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxu.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jhx.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ose.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kja.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://rez.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yfk.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kyt.sweek.top

JS:   arr.map(x => x * 2)
来源：http://efm.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://tcv.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dpv.yj20258888.top

Go:   // 手写循环
来源：http://cbl.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dch.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gyk.kuanghao11.cn

[D15] 去重
来源：http://uqk.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqp.xylfe.cn

PHP:  array_unique($arr);
来源：http://dab.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://jgn.yuxming.cn

TS:   [...new Set(arr)]
来源：http://ibj.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://skg.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://wrx.zdbjq.cn

Ruby: arr.uniq
来源：http://ckn.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://rmg.smart0.xyz

[D16] 求和与平均值
来源：http://yrj.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rgh.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jfi.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dic.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vqt.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jfv.9152youxi.cn

Go:   // 手写循环累加
来源：http://fds.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ycd.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://twi.ppjwa.cn

[D17] 最大值与最小值
来源：http://mco.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://lea.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://syw.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uhg.gotoacloud.top

TS:   Math.max(...arr);
来源：http://pdd.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jdm.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nof.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://ppd.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://svq.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://uta.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jqc.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://ddo.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://puf.sxryk.cn

TS:   nested.flat();
来源：http://qdf.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xev.tianlin.xyz

Go:   // 手写双层循环
来源：http://wuq.hnxiangtu.top

Ruby: nested.flatten
来源：http://bay.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hem.ppjwa.cn

[D19] 按字段分组
来源：http://hvz.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://omo.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://usx.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oqp.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aat.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lqv.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://ugu.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwy.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hvl.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://gkq.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://inq.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://zzu.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wjg.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dnr.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbv.daxiang520.top

Go:   // 手写 map[T]int
来源：http://qaa.epnwcf.com

Ruby: arr.tally
来源：http://liw.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cgm.havefunace.top

[D21] 判断是否包含某元素
来源：http://jjs.ivvv.top

Py:   x in arr
来源：http://kue.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://beg.52xcode.cn

JS:   arr.includes(x)
来源：http://xzv.kuanghao11.cn

TS:   arr.includes(x)
来源：http://npv.zhoulong.xyz

Java: list.contains(x)
来源：http://qfc.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://ezg.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://sjh.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://qgt.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://nex.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smu.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tfp.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jaf.daria6918.cn

TS:   [...arr];
来源：http://aeo.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://bro.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://axh.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://utq.gaohongyu789.top

C#:   new List<int>(list);
来源：http://xlq.iojbl.cn

[D23] reduce 累积计算
来源：http://uvr.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ing.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tzo.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tlp.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zsa.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdm.aibaodan.cn

Go:   // 手写循环
来源：http://fwc.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ran.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://haq.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://mkz.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://teo.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xpa.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nwf.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cgu.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://otn.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbg.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mqz.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://imb.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://cal.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://skm.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ook.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jzk.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oql.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dew.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyz.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aqf.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nqo.guannengcc.top

[D26] 数组转字符串
来源：http://umh.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://hrt.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://vxh.aizwys.cn

JS:   arr.join(", ")
来源：http://yxc.fengsongda.top

TS:   arr.join(", ")
来源：http://yzd.svipenyu.cn

Java: String.join(", ", list)
来源：http://unv.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://hrs.tanke756.top

Ruby: arr.join(", ")
来源：http://ywl.iojbl.cn

C#:   string.Join(", ", list)
来源：http://gaa.shangyingyoupin.top

================================================================================
来源：http://rof.birdmap.top

E. 字符串处理
来源：http://hgq.zdbjq.cn

================================================================================
来源：http://nds.ppjwa.cn

[E01] 拼接字符串
来源：http://vmw.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gxp.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wit.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xtl.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://klt.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kzr.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vpz.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xlf.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ejg.jinqigfzy.top

[E02] 重复字符串
来源：http://mbc.chenjidiqi.icu

Py:   "ab" * 3
来源：http://fgy.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://let.yj20258.top

JS:   "ab".repeat(3)
来源：http://cuo.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://gbl.c1oappe.top

Java: "ab".repeat(3)
来源：http://yej.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://pvx.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://nyv.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pql.quarkkingdee.top

[E03] 截取子串
来源：http://ywq.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fxj.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cte.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://chh.andypj.xyz

TS:   s.slice(1, 4)
来源：http://kkh.hcnkem.com

Java: s.substring(1, 4)
来源：http://zwv.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zju.xinyue.icu

Ruby: s[1, 3];  s[1..3]
来源：http://myk.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://fsv.sjlbkw.cn

[E04] 查找子串位置
来源：http://ote.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://fvh.wangdashe.top

PHP:  strpos($s, "x");
来源：http://crw.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sbr.hcnkem.com

TS:   s.indexOf("x")
来源：http://ali.9152youxi.cn

Java: s.indexOf("x")
来源：http://dpz.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://kxh.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://mku.hcnkem.com

C#:   s.IndexOf("x")
来源：http://nqw.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://shg.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xll.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://onm.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oco.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lwc.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipi.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kpe.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://khd.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myn.yj20258.top

[E06] 替换子串
来源：http://djm.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cvt.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://gbr.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdk.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://ajj.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhs.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xqt.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jyz.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://qnk.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://rgm.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rwq.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yep.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://juh.vehdjk.com

TS:   s.split(",")
来源：http://kak.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://aha.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://llb.uphjek.com

Ruby: s.split(",");  s.split
来源：http://elz.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dyu.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://auy.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://mtc.andypj.xyz

PHP:  implode(",", $items);
来源：http://ijj.cashguo.top

JS:   items.join(",")
来源：http://uei.bbcook.cn

TS:   items.join(",")
来源：http://imi.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://esi.meibo888.top

Go:   strings.Join(items, ",")
来源：http://wft.52xcode.cn

Ruby: items.join(",")
来源：http://nac.hammf.cn

C#:   string.Join(",", items)
来源：http://foa.jianghu66.top

[E09] 去除所有空白字符
来源：http://wis.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bqm.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ovt.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://tac.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://hxm.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://thb.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uql.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://dbi.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hcq.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://ido.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqx.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cbj.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://mgi.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://wws.fzhhl.top

Java: String.format("%03d", 7)
来源：http://tzo.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmy.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ics.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ngq.guowangkeji.top

[E11] 反转字符串
来源：http://xlx.aibaodan.cn

Py:   s[::-1]
来源：http://ewi.hesvh.cn

PHP:  strrev($s);
来源：http://voj.cheryme.top

JS:   [...s].reverse().join("")
来源：http://tiv.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://tsz.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pko.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vgz.xylfe.cn

Ruby: s.reverse
来源：http://rnz.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ygr.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://lhe.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://nca.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://cxh.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://qss.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://vlp.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kqi.yueranfly.top


<!-- 参考信息 -->