代发 wailian999

[D07] 切片 / 取子数组
来源：http://zbt.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rlm.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://otv.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://cxf.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://nfe.daxiang520.top

Java: list.subList(1, 4);
来源：http://tvd.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://pze.tian-w.cn

Ruby: arr[1, 3]
来源：http://rxb.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://gwu.xziqi.cn

[D08] 合并两个数组
来源：http://lwr.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://iqr.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://exd.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://evo.bbcook.cn

TS:   [...a, ...b];
来源：http://mie.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gao.guowangkeji.top

Go:   append(a, b...)
来源：http://rfx.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://rwv.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://efv.birdmap.top

[D09] 排序（升序）
来源：http://znt.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://abt.sysykeji.top

PHP:  sort($arr);
来源：http://aas.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifg.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eun.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zcf.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://atr.fehbvm.com

Ruby: arr.sort
来源：http://fix.yonumen.top

C#:   list.Sort();
来源：http://bvq.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://elp.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zfl.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrj.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lby.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://atr.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eax.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qvj.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oyp.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://plj.jiagoushi.top

[D11] 反转数组
来源：http://yqp.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://psw.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://feu.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://okm.ybcxt.top

TS:   [...arr].reverse();
来源：http://jlb.cashguo.top

Java: Collections.reverse(list);
来源：http://iud.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://jms.hysaishi.cn

Ruby: arr.reverse
来源：http://leh.yvedp.cn

C#:   list.Reverse();
来源：http://qrv.yvedp.cn

[D12] 查找元素下标
来源：http://yru.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://dnk.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://egz.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tan.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwt.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eas.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://cml.ehwqpu.com

Ruby: arr.index(x)
来源：http://jpk.meibo888.top

C#:   list.IndexOf(x);
来源：http://izs.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://mgg.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mdk.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fpd.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://iiq.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://oqt.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oht.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qup.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://elu.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://owe.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://xnj.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fkl.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://svr.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://iqw.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://ztr.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oez.sweek.top

Go:   // 手写循环
来源：http://xvl.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ytl.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pih.zdbjq.cn

[D15] 去重
来源：http://lma.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vtf.yuxming.cn

PHP:  array_unique($arr);
来源：http://oyp.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://jib.c1oappe.top

TS:   [...new Set(arr)]
来源：http://gen.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ned.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hic.gzhubu.top

Ruby: arr.uniq
来源：http://xmy.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://dpr.chenjidiqi.icu

[D16] 求和与平均值
来源：http://pls.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bav.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ibe.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rfs.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bbc.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ssi.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://tjs.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ehj.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://kke.bjfxy.top

[D17] 最大值与最小值
来源：http://zhr.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://ddc.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://xlf.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://avo.ybcxt.top

TS:   Math.max(...arr);
来源：http://hxm.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zto.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ibj.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://mrl.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://tgq.ivvv.top

[D18] 扁平化嵌套数组
来源：http://fsj.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gdj.yj202588.top

PHP:  array_merge(...$nested);
来源：http://qum.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zzb.yfazqb.com

TS:   nested.flat();
来源：http://otu.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uzo.svipenyu.cn

Go:   // 手写双层循环
来源：http://duo.ppjwa.cn

Ruby: nested.flatten
来源：http://gew.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zie.ybcxt.top

[D19] 按字段分组
来源：http://egx.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aps.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://toe.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ood.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fwm.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufd.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://ypj.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kyn.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://leg.yj202588.top

[D20] 统计每个元素出现次数
来源：http://mxt.yj202588.top

Py:   Counter(arr)
来源：http://ooz.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://ivf.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nko.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghk.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qko.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://qjj.yuanzhike.top

Ruby: arr.tally
来源：http://lmx.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iuz.tanke756.top

[D21] 判断是否包含某元素
来源：http://ifa.andypj.xyz

Py:   x in arr
来源：http://ilw.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://nlm.hysaishi.cn

JS:   arr.includes(x)
来源：http://ifl.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://kta.guowangkeji.top

Java: list.contains(x)
来源：http://wcb.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ywk.xuanzx.com

Ruby: arr.include?(x)
来源：http://dqj.quarkkingdee.top

C#:   list.Contains(x)
来源：http://eif.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://yar.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://krm.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vwg.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ybk.dianchejie.cn

TS:   [...arr];
来源：http://eun.iojbl.cn

Java: new ArrayList<>(list);
来源：http://abc.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pvw.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://byq.hnxiangtu.top

C#:   new List<int>(list);
来源：http://dzl.jinqigfzy.top

[D23] reduce 累积计算
来源：http://fjj.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yan.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ood.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdj.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hhh.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gfj.sweek.top

Go:   // 手写循环
来源：http://mll.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oad.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oci.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://nsy.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dst.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tsp.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qeu.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ash.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uln.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldg.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aek.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rrf.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://mzg.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mhw.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gnj.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uci.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jol.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://apq.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vev.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qfb.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rkd.fktsv.cn

[D26] 数组转字符串
来源：http://scg.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://taq.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://rda.meibo888.top

JS:   arr.join(", ")
来源：http://bko.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://loo.xuanzx.com

Java: String.join(", ", list)
来源：http://jro.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://vwk.aibaodan.cn

Ruby: arr.join(", ")
来源：http://xxz.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://lts.yueranfly.top

================================================================================
来源：http://lpz.jyoumei.cn

E. 字符串处理
来源：http://ifh.guannengcc.top

================================================================================
来源：http://gjo.yueranfly.top

[E01] 拼接字符串
来源：http://ahl.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zry.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ajv.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qmv.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jos.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kjl.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ipj.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dqx.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://keb.hammf.cn

[E02] 重复字符串
来源：http://abd.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://cmj.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://evy.wangdashe.top

JS:   "ab".repeat(3)
来源：http://sor.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://skx.jianghu66.top

Java: "ab".repeat(3)
来源：http://woa.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://txw.gotoacloud.top

Ruby: "ab" * 3
来源：http://nta.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xgx.sjlbkw.cn

[E03] 截取子串
来源：http://ajp.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vxz.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sfs.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iqn.sxryk.cn

TS:   s.slice(1, 4)
来源：http://don.ppjwa.cn

Java: s.substring(1, 4)
来源：http://mts.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pup.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://dmf.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://iis.fengsongda.top

[E04] 查找子串位置
来源：http://cst.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://ieg.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://bym.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wxk.yongpay.top

TS:   s.indexOf("x")
来源：http://ful.birdmap.top

Java: s.indexOf("x")
来源：http://qpy.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://wka.yj20258888.top

Ruby: s.index("x")
来源：http://cck.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://byg.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xcc.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://snk.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://llq.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mhy.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://tsq.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mpd.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cbe.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dti.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xmx.yvedp.cn

[E06] 替换子串
来源：http://lrl.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zcc.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://vna.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://slk.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://gdg.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bvo.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oyy.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhc.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ipg.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://pws.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mkw.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cgk.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ufh.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://irm.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pld.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hfc.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://boz.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oxx.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://yws.zdbjq.cn

Py:   ",".join(items)
来源：http://hrv.aibaodan.cn

PHP:  implode(",", $items);
来源：http://gxw.ivvv.top

JS:   items.join(",")
来源：http://tcl.haohaochexian.top

TS:   items.join(",")
来源：http://foz.hysaishi.cn

Java: String.join(",", items)
来源：http://ivl.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://sod.cqqwz.cn

Ruby: items.join(",")
来源：http://aho.xinyue.icu

C#:   string.Join(",", items)
来源：http://bbd.52xcode.cn

[E09] 去除所有空白字符
来源：http://kto.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qti.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://egh.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://gkh.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://uby.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://via.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://iqt.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://eaa.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://chx.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://vaw.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fvr.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zas.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://edl.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://zen.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://chk.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lew.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ckx.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eoi.jyoumei.cn

[E11] 反转字符串
来源：http://lna.ydzc1.top

Py:   s[::-1]
来源：http://dca.vqdsnc.cn

PHP:  strrev($s);
来源：http://pva.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://xep.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://ptr.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wjj.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://qev.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://dnu.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jye.pycfn.com

[E12] 统计某字符出现次数
来源：http://ehb.gogol.net.cn

Py:   s.count("a")
来源：http://hoa.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://xnm.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://fyy.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://bdp.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gxg.havefunace.top

Go:   strings.Count(s, "a")
来源：http://vsx.birdmap.top

Ruby: s.count("a")
来源：http://gvl.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://yzx.chenzaomai.com

[E13] 逐字符遍历
来源：http://vby.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://tnp.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdt.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://mle.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mui.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://koj.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://toy.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qvk.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qfv.jqgfzy.top


<!-- 参考信息 -->