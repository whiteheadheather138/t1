代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zhv.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gjx.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ngf.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://zqy.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://inb.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zio.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://quc.hnxiangtu.top

[D06] 数组长度
来源：http://paz.fengsongda.top

Py:   len(arr)
来源：http://mpg.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://yoy.ivvv.top

JS:   arr.length
来源：http://xtc.nwbrower.top

TS:   arr.length
来源：http://ljl.ywan-chungtsiang.top

Java: list.size();
来源：http://gab.yj20258.top

Go:   len(arr)
来源：http://abd.smart0.xyz

Ruby: arr.length; arr.size
来源：http://kyd.haohaochexian.top

C#:   list.Count;
来源：http://ubq.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://cfe.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ism.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://bsk.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://jnq.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://tgg.yonumen.top

Java: list.subList(1, 4);
来源：http://pfd.tian-w.cn

Go:   arr[1:4]
来源：http://vpj.ybcxt.top

Ruby: arr[1, 3]
来源：http://ryd.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://wti.yj20258.top

[D08] 合并两个数组
来源：http://tte.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://quo.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://hje.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sax.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://xze.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://acu.yueranfly.top

Go:   append(a, b...)
来源：http://alv.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://xbl.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://qtr.sjlbkw.cn

[D09] 排序（升序）
来源：http://oro.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://lqx.pengpengdd.cyou

PHP:  sort($arr);
来源：http://mqs.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jgq.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zyw.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wpz.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ufi.tian-w.cn

Ruby: arr.sort
来源：http://dld.yj20258888.top

C#:   list.Sort();
来源：http://emb.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://avr.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xqe.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ooe.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyt.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lql.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wzw.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qdz.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tyy.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gud.hysaishi.cn

[D11] 反转数组
来源：http://nca.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://bey.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://cvs.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xyv.redwolf501.top

TS:   [...arr].reverse();
来源：http://zir.redwolf501.top

Java: Collections.reverse(list);
来源：http://aau.sysykeji.top

Go:   slices.Reverse(arr)
来源：http://hmv.epnwcf.com

Ruby: arr.reverse
来源：http://jqy.havefunace.top

C#:   list.Reverse();
来源：http://rlh.hysaishi.cn

[D12] 查找元素下标
来源：http://xix.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://tko.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ebr.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gcx.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://svn.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vvs.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://pmv.fzhhl.top

Ruby: arr.index(x)
来源：http://gqi.bbcook.cn

C#:   list.IndexOf(x);
来源：http://ecw.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://uxa.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cxj.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ftw.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://nvo.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://gyo.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vuk.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emf.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ufs.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oio.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://jog.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wsh.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hmx.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://rdd.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://ijk.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jkm.yangfankeji.com

Go:   // 手写循环
来源：http://xxx.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://bbr.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mdk.yanxiufei.cn

[D15] 去重
来源：http://ips.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fiy.havefunace.top

PHP:  array_unique($arr);
来源：http://vgf.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://bco.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://gxu.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rep.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hgb.zdbjq.cn

Ruby: arr.uniq
来源：http://vyz.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://leu.bjfxy.top

[D16] 求和与平均值
来源：http://zvr.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gml.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://khb.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://brv.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tnl.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jbv.tanke756.top

Go:   // 手写循环累加
来源：http://uvd.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nud.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://bhl.zhijiandao.cn

[D17] 最大值与最小值
来源：http://sjh.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://nfv.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://ciw.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ajq.sweek.top

TS:   Math.max(...arr);
来源：http://oga.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://vok.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://geb.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://nhm.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://eio.sweek.top

[D18] 扁平化嵌套数组
来源：http://prk.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aox.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://ndh.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pha.yvedp.cn

TS:   nested.flat();
来源：http://vft.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mcb.ivvv.top

Go:   // 手写双层循环
来源：http://nce.vehdjk.com

Ruby: nested.flatten
来源：http://mie.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fgt.nwbrower.top

[D19] 按字段分组
来源：http://smy.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ysr.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dsd.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://biu.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dar.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iqi.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://oqx.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rem.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://grh.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://let.zhiwuduotai.top

Py:   Counter(arr)
来源：http://kaw.cheryme.top

PHP:  array_count_values($arr);
来源：http://zzg.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://evd.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://imu.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pzp.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://bnp.daxiang520.top

Ruby: arr.tally
来源：http://jcz.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bwp.mhx1999.top

[D21] 判断是否包含某元素
来源：http://jqp.chenlongwang.top

Py:   x in arr
来源：http://ugo.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://poo.tianlin.xyz

JS:   arr.includes(x)
来源：http://ggi.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://cvr.birdmap.top

Java: list.contains(x)
来源：http://sur.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://lxs.ivvv.top

Ruby: arr.include?(x)
来源：http://xlw.hesvh.cn

C#:   list.Contains(x)
来源：http://yvq.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://jed.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cdf.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xyi.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edw.yuanzhike.top

TS:   [...arr];
来源：http://xdj.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://gbv.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://dpx.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://swt.cucudq.cn

C#:   new List<int>(list);
来源：http://jqz.mhx1999.top

[D23] reduce 累积计算
来源：http://pqz.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rzi.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kfs.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tei.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oqa.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://sur.chenlongwang.top

Go:   // 手写循环
来源：http://ohv.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fej.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lyo.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://uhm.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://njq.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://efz.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://stz.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://spi.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bjd.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uvr.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eju.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zag.tarul.cn

[D25] Set 集合去重与交并差
来源：http://tjt.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pes.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dss.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://svr.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://moj.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ric.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://syg.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://say.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bpe.jianghu66.top

[D26] 数组转字符串
来源：http://zeh.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://aiw.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://xgh.fehbvm.com

JS:   arr.join(", ")
来源：http://hnu.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://nxs.cqqwz.cn

Java: String.join(", ", list)
来源：http://erh.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://ljg.ydzc1.top

Ruby: arr.join(", ")
来源：http://ssh.yj20258888.top

C#:   string.Join(", ", list)
来源：http://rmq.cheryme.top

================================================================================
来源：http://aeb.jinqigufen.top

E. 字符串处理
来源：http://lrp.tianlin.xyz

================================================================================
来源：http://roy.ybcxt.top

[E01] 拼接字符串
来源：http://ppd.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fjh.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yhm.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ovm.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoh.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pen.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wjz.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sbg.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aeh.havefunace.top

[E02] 重复字符串
来源：http://flw.hcnkem.com

Py:   "ab" * 3
来源：http://smk.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://fqr.smart0.xyz

JS:   "ab".repeat(3)
来源：http://euy.aizwys.cn

TS:   "ab".repeat(3)
来源：http://ktk.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://moa.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://hcr.sxryk.cn

Ruby: "ab" * 3
来源：http://eev.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lgk.andypj.xyz

[E03] 截取子串
来源：http://yjz.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://han.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vnp.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bog.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://gko.mhx1999.top

Java: s.substring(1, 4)
来源：http://xhp.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iiz.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://rdh.316326.xyz

C#:   s.Substring(1, 3)
来源：http://egj.zdqjudy.top

[E04] 查找子串位置
来源：http://shy.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://yrg.redwolf501.top

PHP:  strpos($s, "x");
来源：http://mtb.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ceb.sysykeji.top

TS:   s.indexOf("x")
来源：http://ewk.pycfn.com

Java: s.indexOf("x")
来源：http://yzw.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://ysc.wangshuangyany.cn

Ruby: s.index("x")
来源：http://din.hcnkem.com

C#:   s.IndexOf("x")
来源：http://qvb.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ikb.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://elj.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://klc.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vjc.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xkp.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dyt.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ovh.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wdt.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nxp.fanxiaobao.xyz

[E06] 替换子串
来源：http://bng.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whi.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://mwk.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vin.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://pid.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpz.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qwh.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tgy.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://cfj.jqgfzy.top

[E07] 按分隔符拆分
来源：http://vbz.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ote.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mlg.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jeb.zhongyouzk.top

TS:   s.split(",")
来源：http://inb.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rtb.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pls.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://eil.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bnj.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://rdi.andypj.xyz

Py:   ",".join(items)
来源：http://opl.ppjwa.cn

PHP:  implode(",", $items);
来源：http://wek.gogol.net.cn

JS:   items.join(",")
来源：http://wwz.svipenyu.cn

TS:   items.join(",")
来源：http://egw.yongpay.top

Java: String.join(",", items)
来源：http://qzs.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://mrx.jlsjyb.cn

Ruby: items.join(",")
来源：http://txj.yj20258.top

C#:   string.Join(",", items)
来源：http://luj.snrcjt.cn

[E09] 去除所有空白字符
来源：http://gia.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ect.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jre.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://jiv.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://doh.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://kfg.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zrq.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://iwb.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://keu.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://edp.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zsx.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsa.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://ulc.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://yqo.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://res.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xue.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lno.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ham.xinyue.icu

[E11] 反转字符串
来源：http://jby.aibaodan.cn

Py:   s[::-1]
来源：http://buf.gotoacloud.top

PHP:  strrev($s);
来源：http://vty.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://axe.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://aht.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tty.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aeb.ivvv.top

Ruby: s.reverse
来源：http://wul.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://ibv.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://pti.aizwys.cn

Py:   s.count("a")
来源：http://unu.ehwqpu.com


<!-- 参考信息 -->