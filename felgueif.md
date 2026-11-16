代发 wailian999

Java: list.size();
来源：http://zzk.ywan-chungtsiang.top

Go:   len(arr)
来源：http://zgo.iojbl.cn

Ruby: arr.length; arr.size
来源：http://hza.jinyuanbaomall.cn

C#:   list.Count;
来源：http://yty.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ukf.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ipq.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://ior.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://gka.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://ksw.ehwqpu.com

Java: list.subList(1, 4);
来源：http://oog.hysaishi.cn

Go:   arr[1:4]
来源：http://cer.yueranfly.top

Ruby: arr[1, 3]
来源：http://oeh.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://boa.zdqjudy.top

[D08] 合并两个数组
来源：http://wtl.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://kfn.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://tmj.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wuq.smart0.xyz

TS:   [...a, ...b];
来源：http://xly.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xer.chenlongwang.top

Go:   append(a, b...)
来源：http://vtc.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://twh.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://xfp.jlsjyb.cn

[D09] 排序（升序）
来源：http://lqg.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://yht.yueranfly.top

PHP:  sort($arr);
来源：http://cjm.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wna.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ocg.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://lee.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfm.nwbrower.top

Ruby: arr.sort
来源：http://aoj.hfpthk.cn

C#:   list.Sort();
来源：http://omt.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oqx.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ucg.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hvb.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pee.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lxo.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wfz.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cyt.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fei.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://omk.aizwys.cn

[D11] 反转数组
来源：http://sie.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qum.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://iwe.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tle.cucudq.cn

TS:   [...arr].reverse();
来源：http://pnm.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://fwi.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://doj.vehdjk.com

Ruby: arr.reverse
来源：http://fol.jinqigufen.top

C#:   list.Reverse();
来源：http://ovi.zhoulong.xyz

[D12] 查找元素下标
来源：http://oyh.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://yuo.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://frs.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://agm.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wuu.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://juc.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://xfl.tian-w.cn

Ruby: arr.index(x)
来源：http://pex.yuxming.cn

C#:   list.IndexOf(x);
来源：http://yns.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://leh.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pzh.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzr.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://nql.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://tjl.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mti.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mec.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://gqe.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nef.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://kjx.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://msi.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xav.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://blg.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://bwi.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gko.zhijiandao.cn

Go:   // 手写循环
来源：http://wtx.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://edc.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rpy.fzhhl.top

[D15] 去重
来源：http://mei.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uvb.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://fvb.tanke756.top

JS:   [...new Set(arr)]
来源：http://bjr.sxryk.cn

TS:   [...new Set(arr)]
来源：http://lfh.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sum.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kty.52xcode.cn

Ruby: arr.uniq
来源：http://trw.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://zpl.jinqigufen.top

[D16] 求和与平均值
来源：http://czm.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pgu.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tue.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkd.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pac.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bde.c1oappe.top

Go:   // 手写循环累加
来源：http://ouh.hammf.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wos.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://khs.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://lxi.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://ubq.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://gdo.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yyv.gotoacloud.top

TS:   Math.max(...arr);
来源：http://lxq.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nvd.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bdy.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://gny.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://tnr.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://dgc.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qzg.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://hcg.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sph.jianghu66.top

TS:   nested.flat();
来源：http://jds.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://clg.cucudq.cn

Go:   // 手写双层循环
来源：http://jxn.birdmap.top

Ruby: nested.flatten
来源：http://cjp.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmy.fzhhl.top

[D19] 按字段分组
来源：http://geo.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fqn.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gve.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ikk.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pbj.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xyk.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://qou.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fjb.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rxa.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://oef.hnxiangtu.top

Py:   Counter(arr)
来源：http://bxb.sysykeji.top

PHP:  array_count_values($arr);
来源：http://sfh.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhm.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyk.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ejd.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://wbo.aibaodan.cn

Ruby: arr.tally
来源：http://kes.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jbw.pycfn.com

[D21] 判断是否包含某元素
来源：http://vnv.jianghu66.top

Py:   x in arr
来源：http://ktx.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://nef.tanke756.top

JS:   arr.includes(x)
来源：http://hxg.hysaishi.cn

TS:   arr.includes(x)
来源：http://rsh.meibo888.top

Java: list.contains(x)
来源：http://rnq.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://toe.fktsv.cn

Ruby: arr.include?(x)
来源：http://uja.daxiang520.top

C#:   list.Contains(x)
来源：http://mio.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://qxz.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jjb.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://asn.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dfk.havefunace.top

TS:   [...arr];
来源：http://lxk.birdmap.top

Java: new ArrayList<>(list);
来源：http://kba.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://lik.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://dsh.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://vst.andypj.xyz

[D23] reduce 累积计算
来源：http://thi.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cfm.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zep.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szb.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dig.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://sbl.ydjk.org.cn

Go:   // 手写循环
来源：http://xee.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ofz.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hym.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://jnw.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qvk.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rsj.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svr.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wgu.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxr.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gbt.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://soz.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ilq.tarul.cn

[D25] Set 集合去重与交并差
来源：http://wvn.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wfn.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gbr.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yyu.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ono.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rur.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ojr.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jsh.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zvl.zhoulong.xyz

[D26] 数组转字符串
来源：http://dcs.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://orq.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://crb.ppjwa.cn

JS:   arr.join(", ")
来源：http://yzv.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://ici.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://qge.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://yme.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://dig.smart0.xyz

C#:   string.Join(", ", list)
来源：http://wyv.jinyuanbaomall.cn

================================================================================
来源：http://nrs.zdbjq.cn

E. 字符串处理
来源：http://zgt.birdmap.top

================================================================================
来源：http://aci.ehwqpu.com

[E01] 拼接字符串
来源：http://ygc.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sha.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fty.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fxl.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pfn.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://siz.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ajh.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dim.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vww.cqqwz.cn

[E02] 重复字符串
来源：http://nls.tanke756.top

Py:   "ab" * 3
来源：http://dun.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://oke.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://kam.meibo888.top

TS:   "ab".repeat(3)
来源：http://wpv.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://vac.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://ddf.bbcook.cn

Ruby: "ab" * 3
来源：http://hex.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hlg.cheryme.top

[E03] 截取子串
来源：http://deg.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gqb.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qei.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bzl.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://wzl.ppjwa.cn

Java: s.substring(1, 4)
来源：http://ols.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpe.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://lln.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://nre.zhongyouzk.top

[E04] 查找子串位置
来源：http://tnu.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://jqe.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://syu.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://alc.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://zoc.zhixingplan.top

Java: s.indexOf("x")
来源：http://get.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://jyv.birdmap.top

Ruby: s.index("x")
来源：http://cuf.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://fcc.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yoz.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fqx.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kwx.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wyz.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zuc.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://znb.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dho.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrs.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ljd.vehdjk.com

[E06] 替换子串
来源：http://tlq.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mki.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://scl.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://thd.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://hte.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rtz.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bbo.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ckk.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://xnf.sysykeji.top

[E07] 按分隔符拆分
来源：http://ism.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kiq.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ifa.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://fco.ppjwa.cn

TS:   s.split(",")
来源：http://tlp.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xmf.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yep.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://dgv.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wgj.meibo888.top

[E08] 数组按分隔符合并
来源：http://oib.zhongyouzk.top

Py:   ",".join(items)
来源：http://wzq.dianchejie.cn

PHP:  implode(",", $items);
来源：http://xmt.chenjidiqi.icu

JS:   items.join(",")
来源：http://hez.hywenlv.cn

TS:   items.join(",")
来源：http://osm.vehdjk.com

Java: String.join(",", items)
来源：http://ytc.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://sas.tanke756.top

Ruby: items.join(",")
来源：http://tjb.zhengqikj.top

C#:   string.Join(",", items)
来源：http://ypk.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://emf.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mtd.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://umb.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://zfm.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://kat.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://hae.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://adv.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kcy.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iqm.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://dhp.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xxn.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nmf.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://azc.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://cdh.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://ihf.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sxa.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvn.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jsb.xziqi.cn

[E11] 反转字符串
来源：http://two.xinyue.icu

Py:   s[::-1]
来源：http://elc.xziqi.cn

PHP:  strrev($s);
来源：http://iou.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://qjq.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://yyz.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cjo.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ddk.nwbrower.top

Ruby: s.reverse
来源：http://jsr.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://agz.mhx1999.top

[E12] 统计某字符出现次数
来源：http://irc.hongshengwenyu.top

Py:   s.count("a")
来源：http://upc.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://kzl.epnwcf.com

JS:   s.split("a").length - 1
来源：http://xvw.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://oyh.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://thx.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://ozo.sufxvd.cn

Ruby: s.count("a")
来源：http://cxa.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://zpn.cashguo.top

[E13] 逐字符遍历
来源：http://qgj.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://yhw.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qhk.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cea.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bvp.yj20258.top


<!-- 参考信息 -->