代发 wailian999

Java: list.size();
来源：http://usl.ctjpmb.com

Go:   len(arr)
来源：http://ibj.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://egp.tian-w.cn

C#:   list.Count;
来源：http://qso.bbcook.cn

[D07] 切片 / 取子数组
来源：http://qhx.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cdn.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xhf.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://nxe.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://tgx.gotoacloud.top

Java: list.subList(1, 4);
来源：http://sqm.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://rnk.yongpay.top

Ruby: arr[1, 3]
来源：http://pyl.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://gph.feifeiyinyue.top

[D08] 合并两个数组
来源：http://cvc.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://kgu.pycfn.com

PHP:  array_merge($a, $b);
来源：http://hyj.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xfn.zycfv.cn

TS:   [...a, ...b];
来源：http://mhy.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ftv.epnwcf.com

Go:   append(a, b...)
来源：http://nsx.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://cnx.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://equ.bbcook.cn

[D09] 排序（升序）
来源：http://ypp.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://bbj.birdmap.top

PHP:  sort($arr);
来源：http://pjg.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fze.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nba.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmq.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kbk.haohaochexian.top

Ruby: arr.sort
来源：http://hus.ctjpmb.com

C#:   list.Sort();
来源：http://vqb.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rqa.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pys.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jnl.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://plx.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://huq.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qke.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mfl.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hoo.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bpx.nanxuanxn.top

[D11] 反转数组
来源：http://ulp.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cws.tanke756.top

PHP:  array_reverse($arr);
来源：http://vlq.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jlx.jianghu66.top

TS:   [...arr].reverse();
来源：http://sje.jinqigufen.top

Java: Collections.reverse(list);
来源：http://yuy.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://kbm.yj20258888.top

Ruby: arr.reverse
来源：http://ibm.shuidangran.top

C#:   list.Reverse();
来源：http://bzc.zdqjudy.top

[D12] 查找元素下标
来源：http://ger.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://pwo.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ele.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eqj.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykv.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jjc.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://goc.yonumen.top

Ruby: arr.index(x)
来源：http://kqg.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://qrd.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://qox.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fql.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vcj.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://geh.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://rsu.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vtv.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://adt.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://uiz.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uky.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://voc.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pru.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vrb.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://hlw.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://xib.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oje.havefunace.top

Go:   // 手写循环
来源：http://yez.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://tqz.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ntb.fehbvm.com

[D15] 去重
来源：http://uqr.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqp.52xcode.cn

PHP:  array_unique($arr);
来源：http://fxu.xinyue.icu

JS:   [...new Set(arr)]
来源：http://zeo.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://hpf.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qzm.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://nxf.zycfv.cn

Ruby: arr.uniq
来源：http://ujd.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://pjl.hammf.cn

[D16] 求和与平均值
来源：http://hyd.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tnf.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tpe.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilk.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tve.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qml.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://ktt.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mvw.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://xxt.haohaochexian.top

[D17] 最大值与最小值
来源：http://hrm.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://cpl.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://dvk.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pub.chenzaomai.com

TS:   Math.max(...arr);
来源：http://tzj.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ujo.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ipg.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://mqp.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://xlb.yj202588.top

[D18] 扁平化嵌套数组
来源：http://sab.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://biv.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://rwq.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://liq.dashuyun.cn

TS:   nested.flat();
来源：http://wqh.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://prn.nanxuanxn.top

Go:   // 手写双层循环
来源：http://wnx.guannengcc.top

Ruby: nested.flatten
来源：http://hpb.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://evr.yanxiufei.cn

[D19] 按字段分组
来源：http://qxm.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wam.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vkk.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://znt.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://knm.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fsz.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://uhi.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://rcn.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dkm.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://ish.tianlin.xyz

Py:   Counter(arr)
来源：http://prl.sysykeji.top

PHP:  array_count_values($arr);
来源：http://cvy.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhj.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://znz.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rem.cucudq.cn

Go:   // 手写 map[T]int
来源：http://ccc.shuidangran.top

Ruby: arr.tally
来源：http://dhm.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vvu.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://env.cqqwz.cn

Py:   x in arr
来源：http://jel.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://fiy.nanxuanxn.top

JS:   arr.includes(x)
来源：http://tcx.smart0.xyz

TS:   arr.includes(x)
来源：http://okd.aizwys.cn

Java: list.contains(x)
来源：http://oxw.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://kcj.yuanzhike.top

Ruby: arr.include?(x)
来源：http://oxx.52xcode.cn

C#:   list.Contains(x)
来源：http://irt.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://xpz.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mhq.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xcj.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://awv.fengsongda.top

TS:   [...arr];
来源：http://hyx.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://flx.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://igq.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://afj.ydzc1.top

C#:   new List<int>(list);
来源：http://zjx.hywenlv.cn

[D23] reduce 累积计算
来源：http://dub.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bfs.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nka.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tjv.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kcx.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxv.zhijiandao.cn

Go:   // 手写循环
来源：http://par.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://thn.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://voc.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://omj.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvw.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gaw.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uxu.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zlu.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://omo.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://txx.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pby.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://osb.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://yha.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bus.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zra.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zhh.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tdk.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tlk.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://glx.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sgl.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lrm.cheryme.top

[D26] 数组转字符串
来源：http://jbr.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://cns.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://khq.jiagoushi.top

JS:   arr.join(", ")
来源：http://zwk.yueranfly.top

TS:   arr.join(", ")
来源：http://ojx.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://vqg.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://goo.tianlin.xyz

Ruby: arr.join(", ")
来源：http://zvk.daxiang520.top

C#:   string.Join(", ", list)
来源：http://tzv.hongshengwenyu.top

================================================================================
来源：http://yxp.snrcjt.cn

E. 字符串处理
来源：http://qgx.mhx1999.top

================================================================================
来源：http://hep.dashuyun.cn

[E01] 拼接字符串
来源：http://pxo.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ecv.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ait.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://voo.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lip.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ham.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eng.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ack.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rvq.9152youxi.cn

[E02] 重复字符串
来源：http://ysa.nanxuanxn.top

Py:   "ab" * 3
来源：http://qbq.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://ljm.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://prn.fktsv.cn

TS:   "ab".repeat(3)
来源：http://ndv.redwolf501.top

Java: "ab".repeat(3)
来源：http://tqj.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://xdd.jqgufenzy.top

Ruby: "ab" * 3
来源：http://erj.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jfs.wangdashe.top

[E03] 截取子串
来源：http://smp.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hdm.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://phw.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iah.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://vqp.shuidangran.top

Java: s.substring(1, 4)
来源：http://rez.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nrh.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jai.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://zot.yj20258.top

[E04] 查找子串位置
来源：http://ehc.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://rhd.jianghu66.top

PHP:  strpos($s, "x");
来源：http://gaw.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tjv.hcnkem.com

TS:   s.indexOf("x")
来源：http://ccc.jqgfzy.top

Java: s.indexOf("x")
来源：http://qsz.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://jiv.guannengcc.top

Ruby: s.index("x")
来源：http://zlv.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://dol.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://lex.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uep.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kqe.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jbo.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://deq.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://joy.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kje.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gbx.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dye.smart0.xyz

[E06] 替换子串
来源：http://ykh.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbe.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://blq.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgk.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://shj.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omx.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qty.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nfa.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://zft.svipenyu.cn

[E07] 按分隔符拆分
来源：http://ikd.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cyv.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://coq.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ytd.gzhubu.top

TS:   s.split(",")
来源：http://eld.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://lvw.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zuf.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://ask.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rno.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://dlk.nanxuanxn.top

Py:   ",".join(items)
来源：http://png.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://qzp.guannengcc.top

JS:   items.join(",")
来源：http://lor.hongshengwenyu.top

TS:   items.join(",")
来源：http://goo.yj20258.top

Java: String.join(",", items)
来源：http://wmk.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://bbd.yvedp.cn

Ruby: items.join(",")
来源：http://ikn.xuanzx.com

C#:   string.Join(",", items)
来源：http://stn.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://nio.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gao.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfc.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://qly.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://csv.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ypn.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yku.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://xji.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsg.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://hxf.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uqz.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bah.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://gbx.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://fsf.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://zcy.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://noy.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sqk.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blp.hywenlv.cn

[E11] 反转字符串
来源：http://lnq.yj20258888.top

Py:   s[::-1]
来源：http://ofy.zhixingplan.top

PHP:  strrev($s);
来源：http://nhi.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://pjp.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://bbg.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yxa.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://wcz.andypj.xyz

Ruby: s.reverse
来源：http://vbu.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ahd.zycfv.cn

[E12] 统计某字符出现次数
来源：http://pip.jyoumei.cn

Py:   s.count("a")
来源：http://qda.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://vrd.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://pzy.meibo888.top

TS:   s.split("a").length - 1
来源：http://htv.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bgx.yongpay.top

Go:   strings.Count(s, "a")
来源：http://zvb.xuetiantiany.cn

Ruby: s.count("a")
来源：http://toy.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://wej.52xcode.cn

[E13] 逐字符遍历
来源：http://eve.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://qbm.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noj.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qqq.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wna.ywan-chungtsiang.top


<!-- 参考信息 -->