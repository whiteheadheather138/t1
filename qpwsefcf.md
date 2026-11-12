代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ugw.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ept.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rvy.xylfe.cn

[D06] 数组长度
来源：http://wyb.feifeiyinyue.top

Py:   len(arr)
来源：http://wvi.jqgfzy.top

PHP:  count($arr);
来源：http://oxv.zhengqikj.top

JS:   arr.length
来源：http://ucz.shanyushiyangtech.top

TS:   arr.length
来源：http://qfm.gotoacloud.top

Java: list.size();
来源：http://vjz.dashuyun.cn

Go:   len(arr)
来源：http://usk.sysykeji.top

Ruby: arr.length; arr.size
来源：http://huo.yj20258888.top

C#:   list.Count;
来源：http://bjz.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://puh.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://khc.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xat.yj202588.top

JS:   arr.slice(1, 4);
来源：http://jqd.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://jjd.hywenlv.cn

Java: list.subList(1, 4);
来源：http://clg.vqdsnc.cn

Go:   arr[1:4]
来源：http://qsy.aizwys.cn

Ruby: arr[1, 3]
来源：http://eof.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://ned.daxiang520.top

[D08] 合并两个数组
来源：http://fjy.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://zhe.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://xzk.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lcr.shzxlz.cn

TS:   [...a, ...b];
来源：http://dyx.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ymk.hfpthk.cn

Go:   append(a, b...)
来源：http://wxm.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://glw.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://acn.hysaishi.cn

[D09] 排序（升序）
来源：http://kcl.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://epb.andypj.xyz

PHP:  sort($arr);
来源：http://jte.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hqj.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zrr.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wcf.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aju.hongshengwenyu.top

Ruby: arr.sort
来源：http://skb.ybcxt.top

C#:   list.Sort();
来源：http://lrp.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zuc.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vwa.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sls.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lsa.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eba.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mqj.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sgo.xziqi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tmh.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hua.dianchejie.cn

[D11] 反转数组
来源：http://gau.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qaz.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://mbq.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hhd.yj20258888.top

TS:   [...arr].reverse();
来源：http://hzr.xylfe.cn

Java: Collections.reverse(list);
来源：http://jwo.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://ymh.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://hzj.c1oappe.top

C#:   list.Reverse();
来源：http://yij.shuidangran.top

[D12] 查找元素下标
来源：http://fcb.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://udl.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://voy.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tur.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cir.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://shj.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://bdl.meibo888.top

Ruby: arr.index(x)
来源：http://csa.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://zvb.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://gjx.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuo.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bhu.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://zwg.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://mmm.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://prn.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sgn.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qrw.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wtq.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://sfg.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bie.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://trx.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://odp.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://myt.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pbm.birdmap.top

Go:   // 手写循环
来源：http://hos.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://nyi.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://frr.vehdjk.com

[D15] 去重
来源：http://xxz.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lbf.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://que.fengsongda.top

JS:   [...new Set(arr)]
来源：http://axh.birdmap.top

TS:   [...new Set(arr)]
来源：http://otp.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wvd.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ycc.sufxvd.cn

Ruby: arr.uniq
来源：http://fww.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://anm.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://kzb.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ram.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ora.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://urz.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxr.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pzr.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://hsg.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pqr.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://ziq.52xcode.cn

[D17] 最大值与最小值
来源：http://tsm.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://omd.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://joz.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yey.meibo888.top

TS:   Math.max(...arr);
来源：http://gub.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qmd.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lba.hammf.cn

Ruby: arr.max;  arr.min
来源：http://cwi.ivvv.top

C#:   list.Max();  list.Min()
来源：http://qff.sweek.top

[D18] 扁平化嵌套数组
来源：http://wia.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rge.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://xcu.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hps.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://rug.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wom.iojbl.cn

Go:   // 手写双层循环
来源：http://rxa.hongshengwenyu.top

Ruby: nested.flatten
来源：http://fuj.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://otr.jiagoushi.top

[D19] 按字段分组
来源：http://res.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jwq.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sie.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nsj.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvq.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oad.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://rmy.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mxp.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cdu.pycfn.com

[D20] 统计每个元素出现次数
来源：http://nqm.mhx1999.top

Py:   Counter(arr)
来源：http://dcw.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://azn.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xat.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onk.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://okg.52xcode.cn

Go:   // 手写 map[T]int
来源：http://upv.shangyingyoupin.top

Ruby: arr.tally
来源：http://mqn.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://clj.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://tad.ehwqpu.com

Py:   x in arr
来源：http://kvo.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://tvu.hcnkem.com

JS:   arr.includes(x)
来源：http://eun.ppjwa.cn

TS:   arr.includes(x)
来源：http://pbz.quarkkingdee.top

Java: list.contains(x)
来源：http://uvo.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://pyg.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://iwg.vqdsnc.cn

C#:   list.Contains(x)
来源：http://cwz.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://fpq.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xnt.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nuc.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edq.jiagoushi.top

TS:   [...arr];
来源：http://wgf.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://vxs.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pxb.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://uzu.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://pal.yfazqb.com

[D23] reduce 累积计算
来源：http://buv.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bes.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eci.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwp.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ixa.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckg.hywenlv.cn

Go:   // 手写循环
来源：http://jti.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rgz.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://spt.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://ftr.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://klu.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hna.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aox.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nsv.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oek.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qec.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jkf.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bvm.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://tzd.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hli.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jhk.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fvr.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ncz.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nla.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hes.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vjh.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ddj.yuxming.cn

[D26] 数组转字符串
来源：http://zvb.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://efs.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://rcp.jinqigfzy.top

JS:   arr.join(", ")
来源：http://orq.sufxvd.cn

TS:   arr.join(", ")
来源：http://eeg.iojbl.cn

Java: String.join(", ", list)
来源：http://brq.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://rta.0kj1m.cn

Ruby: arr.join(", ")
来源：http://irn.daria6918.cn

C#:   string.Join(", ", list)
来源：http://ljv.jiagoushi.top

================================================================================
来源：http://ojy.shanyushiyangtech.top

E. 字符串处理
来源：http://pya.guannengcc.top

================================================================================
来源：http://jkx.sxryk.cn

[E01] 拼接字符串
来源：http://cuu.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://urg.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sgz.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sac.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vus.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://unj.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tgs.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mzk.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjn.chenjidiqi.icu

[E02] 重复字符串
来源：http://jto.fzhhl.top

Py:   "ab" * 3
来源：http://vro.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://xuw.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://ekc.gzhubu.top

TS:   "ab".repeat(3)
来源：http://ppe.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://zvz.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://syg.zhijiandao.cn

Ruby: "ab" * 3
来源：http://ccl.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xol.52xcode.cn

[E03] 截取子串
来源：http://jwt.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oyy.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eje.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cuw.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://fly.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://eay.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://roh.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nfk.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://yzd.xziqi.cn

[E04] 查找子串位置
来源：http://mus.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://rud.yfazqb.com

PHP:  strpos($s, "x");
来源：http://dku.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cnv.svipenyu.cn

TS:   s.indexOf("x")
来源：http://fxo.52xcode.cn

Java: s.indexOf("x")
来源：http://tew.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://pct.fehbvm.com

Ruby: s.index("x")
来源：http://qoi.meibo888.top

C#:   s.IndexOf("x")
来源：http://llr.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ahy.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lbv.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cbo.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qho.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://byw.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rke.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://snu.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hev.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kno.shanyushiyangkeji.top

[E06] 替换子串
来源：http://bqk.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dwd.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://wqf.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfl.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://dxk.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eoc.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zlo.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cga.havefunace.top

C#:   s.Replace("a", "b")
来源：http://xmn.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://jwp.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rql.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xxg.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gmt.jqgufenzy.top

TS:   s.split(",")
来源：http://wkc.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://myo.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://afy.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://rsy.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mnz.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://wmg.zhiwuduotai.top

Py:   ",".join(items)
来源：http://cwc.tianlin.xyz

PHP:  implode(",", $items);
来源：http://jfx.fengsongda.top

JS:   items.join(",")
来源：http://lrh.chenzaomai.com

TS:   items.join(",")
来源：http://fzq.tianlin.xyz

Java: String.join(",", items)
来源：http://zmt.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://snw.pycfn.com

Ruby: items.join(",")
来源：http://wti.xziqi.cn

C#:   string.Join(",", items)
来源：http://mth.yongpay.top

[E09] 去除所有空白字符
来源：http://zzq.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tbm.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://auj.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://xfs.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://kit.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://vqp.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://not.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://otz.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xqo.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://kql.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cbl.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://muy.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://flf.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://ggd.cucudq.cn

Java: String.format("%03d", 7)
来源：http://fso.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jft.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zwf.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ehe.hammf.cn

[E11] 反转字符串
来源：http://mbx.hesvh.cn

Py:   s[::-1]
来源：http://atn.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://nlt.yonumen.top

JS:   [...s].reverse().join("")
来源：http://aht.yongpay.top

TS:   [...s].reverse().join("")
来源：http://oxi.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bzh.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hql.yj20258.top

Ruby: s.reverse
来源：http://oiw.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://axr.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://evm.zhixingplan.top

Py:   s.count("a")
来源：http://fom.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://wsm.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://jcf.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://rhc.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zsl.aizwys.cn


<!-- 参考信息 -->