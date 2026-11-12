代发 wailian999

PHP:  sort($arr);
来源：http://drd.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://omm.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xjx.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mdc.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://urb.sxryk.cn

Ruby: arr.sort
来源：http://uxr.fengsongda.top

C#:   list.Sort();
来源：http://uoc.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gni.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cjk.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wsy.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vkw.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pew.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gvw.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbh.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gwe.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zsr.sxryk.cn

[D11] 反转数组
来源：http://wgc.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://vls.zycfv.cn

PHP:  array_reverse($arr);
来源：http://xdx.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jgl.sysykeji.top

TS:   [...arr].reverse();
来源：http://lrk.c1oappe.top

Java: Collections.reverse(list);
来源：http://xjc.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://cee.hysaishi.cn

Ruby: arr.reverse
来源：http://glh.hnxiangtu.top

C#:   list.Reverse();
来源：http://smm.hesvh.cn

[D12] 查找元素下标
来源：http://byp.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://vqh.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dvd.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tsg.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vkv.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bkf.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://tff.daxiang520.top

Ruby: arr.index(x)
来源：http://sal.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://ogg.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://jkq.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwv.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://end.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://pod.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://umh.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zwi.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://usa.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://dch.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://gfs.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://bmh.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://giq.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zbi.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://nmn.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://cgq.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qrx.shanyushiyangtech.top

Go:   // 手写循环
来源：http://odc.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://eih.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://whs.yonumen.top

[D15] 去重
来源：http://qsi.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cgf.yongpay.top

PHP:  array_unique($arr);
来源：http://mga.xylfe.cn

JS:   [...new Set(arr)]
来源：http://ijl.yongpay.top

TS:   [...new Set(arr)]
来源：http://qsx.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uen.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fhf.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://bjk.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://uay.vehdjk.com

[D16] 求和与平均值
来源：http://amh.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vsj.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mxp.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lun.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmq.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xyb.zhixingplan.top

Go:   // 手写循环累加
来源：http://wcj.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cyi.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://ras.gaohongyu789.top

[D17] 最大值与最小值
来源：http://zuw.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://aoa.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://umv.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qlc.havefunace.top

TS:   Math.max(...arr);
来源：http://flk.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ttn.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://luw.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://tlk.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://nuz.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://cdf.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nvx.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://urb.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qzs.zycfv.cn

TS:   nested.flat();
来源：http://sni.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pfh.sjlbkw.cn

Go:   // 手写双层循环
来源：http://cos.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://lww.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lqt.xinyue.icu

[D19] 按字段分组
来源：http://ugc.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xjn.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rex.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jql.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jtj.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://two.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://wfi.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://hxu.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vdu.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://wbg.tanke756.top

Py:   Counter(arr)
来源：http://smx.aizwys.cn

PHP:  array_count_values($arr);
来源：http://yry.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oed.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pqs.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xip.316326.xyz

Go:   // 手写 map[T]int
来源：http://pzf.shangyingyoupin.top

Ruby: arr.tally
来源：http://uow.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rqo.daxiang520.top

[D21] 判断是否包含某元素
来源：http://xws.jinghuilouyu.cn

Py:   x in arr
来源：http://lap.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://vek.tian-w.cn

JS:   arr.includes(x)
来源：http://ggu.316326.xyz

TS:   arr.includes(x)
来源：http://dcv.aibaodan.cn

Java: list.contains(x)
来源：http://mde.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://fvb.nwbrower.top

Ruby: arr.include?(x)
来源：http://ene.xylfe.cn

C#:   list.Contains(x)
来源：http://jvk.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://aia.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rpo.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pyl.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hpp.hnxiangtu.top

TS:   [...arr];
来源：http://ijq.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://qef.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gsi.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://zih.yongpay.top

C#:   new List<int>(list);
来源：http://kne.zdqjudy.top

[D23] reduce 累积计算
来源：http://hng.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nql.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lpg.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fef.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ggo.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfr.xinyue.icu

Go:   // 手写循环
来源：http://wut.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kal.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ife.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://kot.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ois.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eda.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://epo.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://omo.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://elp.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iok.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://usb.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://inu.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://yyu.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tmd.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zia.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://crs.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uap.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vuc.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uhv.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hah.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://udq.yj20258.top

[D26] 数组转字符串
来源：http://rve.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://dlj.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://ozr.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://few.ydzc1.top

TS:   arr.join(", ")
来源：http://exj.chenjidiqi.icu

Java: String.join(", ", list)
来源：http://qlu.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://lau.xylfe.cn

Ruby: arr.join(", ")
来源：http://mhe.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://vcb.dashuyun.cn

================================================================================
来源：http://noo.316326.xyz

E. 字符串处理
来源：http://frt.shzxlz.cn

================================================================================
来源：http://gns.sufxvd.cn

[E01] 拼接字符串
来源：http://pum.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owt.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oad.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uxk.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zbv.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gwc.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gmx.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pql.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dej.jlsjyb.cn

[E02] 重复字符串
来源：http://udy.nwbrower.top

Py:   "ab" * 3
来源：http://rzn.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://zco.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://kbs.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://dco.jianghu66.top

Java: "ab".repeat(3)
来源：http://iub.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fgh.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://avl.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wic.shuidangran.top

[E03] 截取子串
来源：http://utx.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxh.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://foi.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kff.fzhhl.top

TS:   s.slice(1, 4)
来源：http://soo.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://bbt.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://npe.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fcw.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://dcs.xinyue.icu

[E04] 查找子串位置
来源：http://gha.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://hiq.guannengcc.top

PHP:  strpos($s, "x");
来源：http://zlj.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cea.dianchejie.cn

TS:   s.indexOf("x")
来源：http://qml.uphjek.com

Java: s.indexOf("x")
来源：http://wjr.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://kqo.cheryme.top

Ruby: s.index("x")
来源：http://zhz.xinyue.icu

C#:   s.IndexOf("x")
来源：http://uom.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://myb.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ajv.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fmj.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ijy.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://sbz.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xyc.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://itk.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aop.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://djj.ivvv.top

[E06] 替换子串
来源：http://hfm.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ktv.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://sfu.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://szi.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://aje.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nbx.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tij.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://afd.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://bor.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://hjz.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tkn.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xvc.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://llb.dianchejie.cn

TS:   s.split(",")
来源：http://ach.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://bpp.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gql.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://ent.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gwx.mhx1999.top

[E08] 数组按分隔符合并
来源：http://ycj.jinqigufen.top

Py:   ",".join(items)
来源：http://kxb.havefunace.top

PHP:  implode(",", $items);
来源：http://ppx.fengsongda.top

JS:   items.join(",")
来源：http://mnc.hammf.cn

TS:   items.join(",")
来源：http://deg.ppjwa.cn

Java: String.join(",", items)
来源：http://nwb.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://ohh.hnqzz.top

Ruby: items.join(",")
来源：http://qia.chenlongwang.top

C#:   string.Join(",", items)
来源：http://dwl.ctjpmb.com

[E09] 去除所有空白字符
来源：http://xob.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iyo.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jrb.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://twh.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://oqk.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://hyf.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mqh.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://vjf.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sdn.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://ixy.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://itr.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oar.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://ooj.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://yme.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://uwy.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://whr.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nps.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xrd.ctjpmb.com

[E11] 反转字符串
来源：http://mik.fktsv.cn

Py:   s[::-1]
来源：http://nie.aibaodan.cn

PHP:  strrev($s);
来源：http://mod.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://mqi.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://qae.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tuk.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zxz.cqqwz.cn

Ruby: s.reverse
来源：http://itl.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://mob.hesvh.cn

[E12] 统计某字符出现次数
来源：http://bpa.nanxinkj.top

Py:   s.count("a")
来源：http://krn.cheryme.top

PHP:  substr_count($s, "a");
来源：http://sze.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://ebr.vehdjk.com

TS:   s.split("a").length - 1
来源：http://cxg.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fpd.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://wos.dianchejie.cn

Ruby: s.count("a")
来源：http://uzn.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://bhk.zycfv.cn

[E13] 逐字符遍历
来源：http://qed.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://kfw.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywt.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mve.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ndz.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rnt.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ksp.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ifw.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ouk.yj20258.top

[E14] URL 编码与 Base64
来源：http://gcf.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mim.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jdd.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mxt.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yiz.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ffr.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://skn.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pab.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xyq.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://gre.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sgk.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fqf.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://weh.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ejk.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fmk.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dyc.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fqi.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jum.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://rma.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://zza.c1oappe.top


<!-- 参考信息 -->