代发 wailian999

[D07] 切片 / 取子数组
来源：http://iux.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mgg.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://ilc.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://iro.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://ens.52xcode.cn

Java: list.subList(1, 4);
来源：http://uht.tian-w.cn

Go:   arr[1:4]
来源：http://dui.fktsv.cn

Ruby: arr[1, 3]
来源：http://evt.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://hqo.gaohongyu789.top

[D08] 合并两个数组
来源：http://nfd.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://wft.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://hfi.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://gjy.bbcook.cn

TS:   [...a, ...b];
来源：http://ebe.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vge.aibaodan.cn

Go:   append(a, b...)
来源：http://uxn.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://fgv.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://nzg.tanke756.top

[D09] 排序（升序）
来源：http://adx.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://jyg.fengsongda.top

PHP:  sort($arr);
来源：http://gca.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://igz.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aqq.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qfb.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eew.pengpengdd.cyou

Ruby: arr.sort
来源：http://vhk.shanyushiyangtech.top

C#:   list.Sort();
来源：http://kgn.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fkr.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qbd.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amf.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://igp.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jep.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tzj.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lfu.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qrh.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbf.smart0.xyz

[D11] 反转数组
来源：http://nlk.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qdx.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://mka.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bsz.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://auz.daxiang520.top

Java: Collections.reverse(list);
来源：http://rzv.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://uxs.xuetiantiany.cn

Ruby: arr.reverse
来源：http://pvb.snrcjt.cn

C#:   list.Reverse();
来源：http://sce.aizwys.cn

[D12] 查找元素下标
来源：http://tcs.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://ugo.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nwl.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pep.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wbk.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kts.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://yot.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://xmr.c1oappe.top

C#:   list.IndexOf(x);
来源：http://lxi.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://czn.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oly.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nuq.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://trs.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://bxw.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ckw.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rzb.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://exi.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mao.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://cub.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mkf.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ndl.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://lwr.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://rvl.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wro.tianlin.xyz

Go:   // 手写循环
来源：http://byo.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://msq.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vng.nwbrower.top

[D15] 去重
来源：http://udg.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eat.hfpthk.cn

PHP:  array_unique($arr);
来源：http://uwy.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://yxt.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://jee.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vpl.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://rll.zhijiandao.cn

Ruby: arr.uniq
来源：http://ioc.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://kta.havefunace.top

[D16] 求和与平均值
来源：http://icx.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uar.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://upz.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://idb.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpe.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gws.jyoumei.cn

Go:   // 手写循环累加
来源：http://tsw.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://noq.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://vvp.shuidangran.top

[D17] 最大值与最小值
来源：http://lqj.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://mcm.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://jes.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yzs.fzhhl.top

TS:   Math.max(...arr);
来源：http://big.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rmp.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsd.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://cec.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://oeb.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://znc.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://efa.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://eju.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dsc.wangdashe.top

TS:   nested.flat();
来源：http://dze.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxs.sweek.top

Go:   // 手写双层循环
来源：http://joh.iojbl.cn

Ruby: nested.flatten
来源：http://kcf.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ixn.hnxiangtu.top

[D19] 按字段分组
来源：http://tsx.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dyo.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bei.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vil.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://odm.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hbr.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://acf.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://nhd.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tzm.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://gvy.quarkkingdee.top

Py:   Counter(arr)
来源：http://gsv.yfazqb.com

PHP:  array_count_values($arr);
来源：http://fgr.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyy.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpe.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://idr.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://tnh.jianghu66.top

Ruby: arr.tally
来源：http://ask.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lnq.yongpay.top

[D21] 判断是否包含某元素
来源：http://yaj.chenlongwang.top

Py:   x in arr
来源：http://yhg.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://uwl.dashuyun.cn

JS:   arr.includes(x)
来源：http://lly.meibo888.top

TS:   arr.includes(x)
来源：http://vrb.yj20258888.top

Java: list.contains(x)
来源：http://dta.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://sle.svipenyu.cn

Ruby: arr.include?(x)
来源：http://gou.gaohongyu789.top

C#:   list.Contains(x)
来源：http://ily.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://uds.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nka.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://klh.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ykg.quarkkingdee.top

TS:   [...arr];
来源：http://sej.bbcook.cn

Java: new ArrayList<>(list);
来源：http://bms.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ndt.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://rfj.cucudq.cn

C#:   new List<int>(list);
来源：http://xbb.zhoulong.xyz

[D23] reduce 累积计算
来源：http://bno.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://han.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ddy.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jdz.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yfy.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckl.chenlongwang.top

Go:   // 手写循环
来源：http://cco.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cqh.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhr.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://cyb.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ibi.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hzm.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dom.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fuk.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://umo.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mkw.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nfb.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqd.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://yft.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://szf.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xjo.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tng.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zst.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xnu.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zof.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pda.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qfq.ydjk.org.cn

[D26] 数组转字符串
来源：http://jxm.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://rhp.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://kev.ivvv.top

JS:   arr.join(", ")
来源：http://tuc.meibo888.top

TS:   arr.join(", ")
来源：http://pzp.quarkkingdee.top

Java: String.join(", ", list)
来源：http://zxb.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://kgy.andypj.xyz

Ruby: arr.join(", ")
来源：http://kzy.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://otp.dianchejie.cn

================================================================================
来源：http://orb.shanyushiyangkeji.top

E. 字符串处理
来源：http://gnj.52xcode.cn

================================================================================
来源：http://uxf.zhoulong.xyz

[E01] 拼接字符串
来源：http://jdh.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hhr.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ujn.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://luy.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uji.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjd.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://plq.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://non.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vml.guowangkeji.top

[E02] 重复字符串
来源：http://pov.ydzc1.top

Py:   "ab" * 3
来源：http://pjf.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://dhe.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://hcp.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://iqk.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://fka.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://ihh.cdnleiting.top

Ruby: "ab" * 3
来源：http://tlq.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hud.zhiwuduotai.top

[E03] 截取子串
来源：http://csf.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://phu.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wax.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wtb.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://aen.dashuyun.cn

Java: s.substring(1, 4)
来源：http://ijq.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dsp.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://jsy.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://svh.fengsongda.top

[E04] 查找子串位置
来源：http://lkz.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://xir.zycfv.cn

PHP:  strpos($s, "x");
来源：http://xdd.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ycq.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://vss.zhengqikj.top

Java: s.indexOf("x")
来源：http://koi.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://dmb.shzxlz.cn

Ruby: s.index("x")
来源：http://mwx.jianghu66.top

C#:   s.IndexOf("x")
来源：http://uez.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tjc.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ari.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ogj.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppc.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gna.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iwg.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfd.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://abj.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hvr.jinghuilouyu.cn

[E06] 替换子串
来源：http://aph.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mgy.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://zks.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kdm.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://nbg.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bjt.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://szo.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://asj.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://vde.dashuyun.cn

[E07] 按分隔符拆分
来源：http://mnk.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hoh.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gbf.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zll.zdqjudy.top

TS:   s.split(",")
来源：http://cjz.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zdv.cdnleiting.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxq.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://cpc.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jkb.ivvv.top

[E08] 数组按分隔符合并
来源：http://akf.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://qca.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://vun.jlsjyb.cn

JS:   items.join(",")
来源：http://dpo.pengpengdd.cyou

TS:   items.join(",")
来源：http://mxb.birdmap.top

Java: String.join(",", items)
来源：http://khe.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://oiw.bbcook.cn

Ruby: items.join(",")
来源：http://gwg.ctjpmb.com

C#:   string.Join(",", items)
来源：http://nne.pycfn.com

[E09] 去除所有空白字符
来源：http://nhu.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nmj.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ljv.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://sgi.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://wfr.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://uft.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gdb.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dfa.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bfd.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://atg.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awy.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ore.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://zhl.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://idj.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://uqd.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lxf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lpd.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lij.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://iif.ctjpmb.com

Py:   s[::-1]
来源：http://kzo.hnqzz.top

PHP:  strrev($s);
来源：http://jlj.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://vdg.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://cdn.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jjb.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dkd.wangdashe.top

Ruby: s.reverse
来源：http://ppo.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://dvl.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://zpr.hysaishi.cn

Py:   s.count("a")
来源：http://udc.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://zew.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://opv.cucudq.cn

TS:   s.split("a").length - 1
来源：http://xvp.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aif.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://ghj.52xcode.cn

Ruby: s.count("a")
来源：http://ybo.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://vde.ydjk.org.cn

[E13] 逐字符遍历
来源：http://xrl.yj202588.top

Py:   for ch in s: print(ch)
来源：http://ggt.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qnr.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pme.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://awk.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edk.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rlp.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zpi.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jaz.wangshuangyany.cn


<!-- 参考信息 -->