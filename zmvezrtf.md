代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://xrh.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nya.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jvq.gotoacloud.top

[D06] 数组长度
来源：http://ycr.shanyushiyangkeji.top

Py:   len(arr)
来源：http://vub.jlsjyb.cn

PHP:  count($arr);
来源：http://xem.zhengqikj.top

JS:   arr.length
来源：http://orh.hnqzz.top

TS:   arr.length
来源：http://gwl.chenlongwang.top

Java: list.size();
来源：http://orb.shuidangran.top

Go:   len(arr)
来源：http://own.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://gzr.xylfe.cn

C#:   list.Count;
来源：http://kfb.wangdashe.top

[D07] 切片 / 取子数组
来源：http://vwm.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ohu.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ewj.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://ygx.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://dzt.yvedp.cn

Java: list.subList(1, 4);
来源：http://iwr.jianghu66.top

Go:   arr[1:4]
来源：http://edl.316326.xyz

Ruby: arr[1, 3]
来源：http://xcp.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://pde.316326.xyz

[D08] 合并两个数组
来源：http://ibb.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://kfm.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://cza.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oey.jianghu66.top

TS:   [...a, ...b];
来源：http://xwz.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://obr.ctjpmb.com

Go:   append(a, b...)
来源：http://trr.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://ykc.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://fna.iojbl.cn

[D09] 排序（升序）
来源：http://qaq.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://aer.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://yuw.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nms.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ugg.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bvx.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hdh.hongshengwenyu.top

Ruby: arr.sort
来源：http://ozp.yuanzhike.top

C#:   list.Sort();
来源：http://auw.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mol.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rrz.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njg.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xzl.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwd.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vqd.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dag.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tsq.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nmv.jianghu66.top

[D11] 反转数组
来源：http://sri.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://jbx.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://iny.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qce.cheryme.top

TS:   [...arr].reverse();
来源：http://quv.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://nma.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://xub.zhijiandao.cn

Ruby: arr.reverse
来源：http://bcw.quarkkingdee.top

C#:   list.Reverse();
来源：http://hrj.jlsjyb.cn

[D12] 查找元素下标
来源：http://hqk.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://kml.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iie.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vbs.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://alb.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fqx.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://anq.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://tfq.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://cex.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://yul.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://elg.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hlz.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://rgs.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://qpr.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://med.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nia.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sqr.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zmz.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://frq.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bsg.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://usm.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://idh.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://ymw.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uid.tarul.cn

Go:   // 手写循环
来源：http://lvc.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://pme.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cml.jinqigfzy.top

[D15] 去重
来源：http://bak.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cmz.hcnkem.com

PHP:  array_unique($arr);
来源：http://dcy.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://jek.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://mpu.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://awd.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://wzo.jyoumei.cn

Ruby: arr.uniq
来源：http://axs.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://ypy.andypj.xyz

[D16] 求和与平均值
来源：http://fyf.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://igi.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tih.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmg.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxn.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyf.vqdsnc.cn

Go:   // 手写循环累加
来源：http://uqf.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mue.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://asx.ybcxt.top

[D17] 最大值与最小值
来源：http://xia.tarul.cn

Py:   max(arr);  min(arr)
来源：http://wmg.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://kkv.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vay.redwolf501.top

TS:   Math.max(...arr);
来源：http://ogq.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pxv.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yaj.cheryme.top

Ruby: arr.max;  arr.min
来源：http://zzd.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://wzo.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://dbn.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zlm.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://ada.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lgf.yongpay.top

TS:   nested.flat();
来源：http://xss.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owc.zhijiandao.cn

Go:   // 手写双层循环
来源：http://gsx.chenlongwang.top

Ruby: nested.flatten
来源：http://keh.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ias.snrcjt.cn

[D19] 按字段分组
来源：http://igx.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kgb.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lon.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bno.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ucv.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vhd.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://swk.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ywp.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wls.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://uob.zhiwuduotai.top

Py:   Counter(arr)
来源：http://ixp.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://mog.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fdx.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pak.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qod.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://atl.yfazqb.com

Ruby: arr.tally
来源：http://yid.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://trd.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://trt.sjlbkw.cn

Py:   x in arr
来源：http://uyc.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://mtt.wangdashe.top

JS:   arr.includes(x)
来源：http://mdd.ydzc1.top

TS:   arr.includes(x)
来源：http://fio.yueranfly.top

Java: list.contains(x)
来源：http://uuz.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://frt.daria6918.cn

Ruby: arr.include?(x)
来源：http://liq.hywenlv.cn

C#:   list.Contains(x)
来源：http://spa.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://ahe.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ihi.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aam.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ucc.zhongyouzk.top

TS:   [...arr];
来源：http://tni.nwbrower.top

Java: new ArrayList<>(list);
来源：http://pzz.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wmk.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://kxh.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://thi.sufxvd.cn

[D23] reduce 累积计算
来源：http://oyq.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nda.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://leq.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znt.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ftk.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://six.feifeiyinyue.top

Go:   // 手写循环
来源：http://bus.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bim.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://twp.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://xhv.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://glz.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thc.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://arq.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vdi.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nui.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qhc.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izj.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rrm.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://tii.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fez.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fvj.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://esz.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vhk.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://esi.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://max.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://csz.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lei.kuanghao11.cn

[D26] 数组转字符串
来源：http://vww.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://lgp.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://cbc.jiagoushi.top

JS:   arr.join(", ")
来源：http://kpk.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://chd.jianghu66.top

Java: String.join(", ", list)
来源：http://ejc.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://gie.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://uyf.c1oappe.top

C#:   string.Join(", ", list)
来源：http://sqf.sjlbkw.cn

================================================================================
来源：http://xrx.cdnleiting.top

E. 字符串处理
来源：http://hgy.mhx1999.top

================================================================================
来源：http://lsk.jyoumei.cn

[E01] 拼接字符串
来源：http://jum.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nsd.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uyn.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://apz.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpx.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kro.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iza.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lku.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mpa.ppjwa.cn

[E02] 重复字符串
来源：http://ryu.sweek.top

Py:   "ab" * 3
来源：http://qdg.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://tiw.yueranfly.top

JS:   "ab".repeat(3)
来源：http://mru.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://hqr.pycfn.com

Java: "ab".repeat(3)
来源：http://wwd.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://vqe.jianghu66.top

Ruby: "ab" * 3
来源：http://elp.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqa.wangdashe.top

[E03] 截取子串
来源：http://hzf.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jvy.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ldh.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://izf.jianghu66.top

TS:   s.slice(1, 4)
来源：http://efu.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://ocs.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ugh.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://yuo.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://xae.sxryk.cn

[E04] 查找子串位置
来源：http://zst.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://krl.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://kwo.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gci.meibo888.top

TS:   s.indexOf("x")
来源：http://gyy.yuxming.cn

Java: s.indexOf("x")
来源：http://iqo.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://sti.meibo888.top

Ruby: s.index("x")
来源：http://nsk.yj202588.top

C#:   s.IndexOf("x")
来源：http://zbh.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oot.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipw.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fco.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvq.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ltk.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wfu.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://stk.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ojn.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gcx.gzhubu.top

[E06] 替换子串
来源：http://pcx.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yvf.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://joe.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fbh.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://bxs.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ccd.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ipu.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzk.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://zlb.tanke756.top

[E07] 按分隔符拆分
来源：http://sto.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nqy.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://auv.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gdu.nanxuanxn.top

TS:   s.split(",")
来源：http://xen.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://qvn.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsi.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://oga.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mnd.ydzc1.top

[E08] 数组按分隔符合并
来源：http://jzf.jqgfzy.top

Py:   ",".join(items)
来源：http://qyj.jqgfzy.top

PHP:  implode(",", $items);
来源：http://vaz.sjlbkw.cn

JS:   items.join(",")
来源：http://tcl.meibo888.top

TS:   items.join(",")
来源：http://sxj.gotoacloud.top

Java: String.join(",", items)
来源：http://eaq.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://fug.52xcode.cn

Ruby: items.join(",")
来源：http://wzv.hesvh.cn

C#:   string.Join(",", items)
来源：http://bmw.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://pky.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqo.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gbh.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://dgm.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://zno.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://rxt.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://fbd.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://hfa.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hmf.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://nyk.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://chz.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qih.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://ewr.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://fip.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://eqx.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lln.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blj.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://exw.sjlbkw.cn

[E11] 反转字符串
来源：http://kfc.zhixingplan.top

Py:   s[::-1]
来源：http://fsn.birdmap.top

PHP:  strrev($s);
来源：http://qkq.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://fsn.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://orj.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rwf.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://weo.hfpthk.cn

Ruby: s.reverse
来源：http://jam.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://mjl.smart0.xyz

[E12] 统计某字符出现次数
来源：http://kvv.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://prg.tarul.cn

PHP:  substr_count($s, "a");
来源：http://gho.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://gpg.jianghu66.top

TS:   s.split("a").length - 1
来源：http://pti.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xyc.sjlbkw.cn


<!-- 参考信息 -->