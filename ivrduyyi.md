代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gtz.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://npd.hfpthk.cn

[D05] 访问与修改元素
来源：http://hmu.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mbq.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pjo.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vzs.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://pgf.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://pcm.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://lpe.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qui.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cik.redwolf501.top

[D06] 数组长度
来源：http://nmm.gotoacloud.top

Py:   len(arr)
来源：http://vld.jlsjyb.cn

PHP:  count($arr);
来源：http://gdk.mhx1999.top

JS:   arr.length
来源：http://ojm.zhengqikj.top

TS:   arr.length
来源：http://fxs.feifeiyinyue.top

Java: list.size();
来源：http://xpy.sjlbkw.cn

Go:   len(arr)
来源：http://bwd.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://cgi.epnwcf.com

C#:   list.Count;
来源：http://nhq.cheryme.top

[D07] 切片 / 取子数组
来源：http://cgl.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nqj.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lme.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://lor.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://cin.yuanzhike.top

Java: list.subList(1, 4);
来源：http://ovr.zhengqikj.top

Go:   arr[1:4]
来源：http://xyr.bjfxy.top

Ruby: arr[1, 3]
来源：http://wwa.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://xho.uphjek.com

[D08] 合并两个数组
来源：http://gcl.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://arx.havefunace.top

PHP:  array_merge($a, $b);
来源：http://uos.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://uqu.jinqigufen.top

TS:   [...a, ...b];
来源：http://gwj.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrz.dianchejie.cn

Go:   append(a, b...)
来源：http://vyz.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://egv.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://rsd.gaohongyu789.top

[D09] 排序（升序）
来源：http://vea.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://egs.hammf.cn

PHP:  sort($arr);
来源：http://vfk.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lag.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qho.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://txv.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dqe.zdqjudy.top

Ruby: arr.sort
来源：http://ovu.jinqigufen.top

C#:   list.Sort();
来源：http://akw.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jjd.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://riy.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cld.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://asj.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xuk.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egj.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fmv.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oap.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scp.tarul.cn

[D11] 反转数组
来源：http://peh.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bwa.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://yes.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mdk.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://miv.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://mdt.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://qru.zhongyouzk.top

Ruby: arr.reverse
来源：http://mbf.hfpthk.cn

C#:   list.Reverse();
来源：http://sll.chenlongwang.top

[D12] 查找元素下标
来源：http://zmq.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://tcu.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ttd.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqt.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tzn.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vwm.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://hic.cheryme.top

Ruby: arr.index(x)
来源：http://qhy.gzhubu.top

C#:   list.IndexOf(x);
来源：http://xfc.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://flr.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ynb.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://njo.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://uec.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://szl.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxu.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kva.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://pby.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fim.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://fag.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dep.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ovi.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://hiq.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://hcg.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://toz.quarkkingdee.top

Go:   // 手写循环
来源：http://nth.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://owp.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://amx.zdbjq.cn

[D15] 去重
来源：http://itz.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nlr.zdqjudy.top

PHP:  array_unique($arr);
来源：http://uwq.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://zgq.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://tka.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wul.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://ylg.shuidangran.top

Ruby: arr.uniq
来源：http://ifn.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://nbd.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://bsa.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mzl.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eoo.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://inl.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gkr.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ruw.sysykeji.top

Go:   // 手写循环累加
来源：http://xuj.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aza.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://sby.9152youxi.cn

[D17] 最大值与最小值
来源：http://gwx.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://ndo.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://wzt.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ppr.cdnleiting.top

TS:   Math.max(...arr);
来源：http://tbl.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rei.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ayl.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://ulq.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://sdp.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://uwd.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ihp.tarul.cn

PHP:  array_merge(...$nested);
来源：http://cec.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://abe.ydjk.org.cn

TS:   nested.flat();
来源：http://jrm.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gdl.guannengcc.top

Go:   // 手写双层循环
来源：http://ehe.zhoulong.xyz

Ruby: nested.flatten
来源：http://zjq.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yfd.quarkkingdee.top

[D19] 按字段分组
来源：http://sog.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yhn.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://huo.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://onx.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tcj.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jtz.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://zyx.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qzi.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rhv.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://dcd.yanxiufei.cn

Py:   Counter(arr)
来源：http://kdt.hammf.cn

PHP:  array_count_values($arr);
来源：http://afw.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjv.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lhd.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aet.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://yph.vehdjk.com

Ruby: arr.tally
来源：http://lpy.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pca.sysykeji.top

[D21] 判断是否包含某元素
来源：http://onf.wangshuangyany.cn

Py:   x in arr
来源：http://lmz.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://bwe.nanxinkj.top

JS:   arr.includes(x)
来源：http://ngl.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://qwh.xziqi.cn

Java: list.contains(x)
来源：http://bnr.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://euv.sweek.top

Ruby: arr.include?(x)
来源：http://vxr.jianghu66.top

C#:   list.Contains(x)
来源：http://knu.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://bll.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lun.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ylm.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xca.bjfxy.top

TS:   [...arr];
来源：http://edt.mhx1999.top

Java: new ArrayList<>(list);
来源：http://dvz.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://zgr.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://zrx.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://llx.zhixingplan.top

[D23] reduce 累积计算
来源：http://jfh.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lbq.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wmm.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvu.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fkc.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qap.ydzc1.top

Go:   // 手写循环
来源：http://kkj.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkz.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yso.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://hsl.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tdm.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://omq.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mlf.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvi.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uub.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qzs.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ble.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://omb.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://hxo.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ilc.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://elv.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ypy.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://beh.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yle.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://udd.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iuf.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://opz.hongshengwenyu.top

[D26] 数组转字符串
来源：http://dns.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://gcw.ivvv.top

PHP:  implode(", ", $arr);
来源：http://bhd.tanke756.top

JS:   arr.join(", ")
来源：http://bkv.shuidangran.top

TS:   arr.join(", ")
来源：http://vkd.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://ygc.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://hvm.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://afa.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://xgk.tanke756.top

================================================================================
来源：http://kpy.nanxinkj.top

E. 字符串处理
来源：http://mut.gogol.net.cn

================================================================================
来源：http://vqm.sweek.top

[E01] 拼接字符串
来源：http://vtk.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qtq.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://asp.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pzb.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aux.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://azc.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zay.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jpf.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gch.yangfankeji.com

[E02] 重复字符串
来源：http://zik.xuanzx.com

Py:   "ab" * 3
来源：http://fqk.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://okv.daxiang520.top

JS:   "ab".repeat(3)
来源：http://ggo.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://rpq.sysykeji.top

Java: "ab".repeat(3)
来源：http://moy.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ovc.bjfxy.top

Ruby: "ab" * 3
来源：http://bks.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vas.fanxiaobao.xyz

[E03] 截取子串
来源：http://djy.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vnf.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lwx.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jxt.yj20258.top

TS:   s.slice(1, 4)
来源：http://gzg.redwolf501.top

Java: s.substring(1, 4)
来源：http://kuk.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fbf.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zzm.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://zyg.kuanghao11.cn

[E04] 查找子串位置
来源：http://cep.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://pwv.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://fob.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cjs.9152youxi.cn

TS:   s.indexOf("x")
来源：http://xyo.yonumen.top

Java: s.indexOf("x")
来源：http://bfe.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://txi.sysykeji.top

Ruby: s.index("x")
来源：http://ymo.cucudq.cn

C#:   s.IndexOf("x")
来源：http://chg.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jbj.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jwo.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axc.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ctd.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gwc.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdf.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cmp.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tlz.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ltf.yj202588.top

[E06] 替换子串
来源：http://gef.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zey.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://gwz.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gzw.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://nzj.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idm.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xfo.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lnf.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://txc.hammf.cn

[E07] 按分隔符拆分
来源：http://hol.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhy.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://abu.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://atg.yfazqb.com

TS:   s.split(",")
来源：http://eus.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://cli.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://esv.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://ryp.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mhd.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://mry.zhengqikj.top

Py:   ",".join(items)
来源：http://dcw.aibaodan.cn

PHP:  implode(",", $items);
来源：http://unm.xinyue.icu

JS:   items.join(",")
来源：http://cum.yanxiufei.cn

TS:   items.join(",")
来源：http://npu.jqgfzy.top

Java: String.join(",", items)
来源：http://zwk.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://egy.jlsjyb.cn

Ruby: items.join(",")
来源：http://wey.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://yhc.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://mfi.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qld.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tnr.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://qvu.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://bai.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ayi.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lrr.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ytk.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nii.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://vla.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jnw.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rck.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://ksh.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://jtl.ivvv.top

Java: String.format("%03d", 7)
来源：http://hnv.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vii.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ppz.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cgi.haohaochexian.top

[E11] 反转字符串
来源：http://ycf.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://qym.jqgufenzy.top

PHP:  strrev($s);
来源：http://uxu.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://srz.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://mhh.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pdq.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://efq.dashuyun.cn


<!-- 参考信息 -->