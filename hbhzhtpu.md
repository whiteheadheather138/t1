代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://uem.sxryk.cn

[D08] 合并两个数组
来源：http://jhe.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://hoi.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://pqz.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hnw.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://anu.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hfg.cashguo.top

Go:   append(a, b...)
来源：http://zvn.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://tfn.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://iik.tianlin.xyz

[D09] 排序（升序）
来源：http://ikr.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://qqw.xziqi.cn

PHP:  sort($arr);
来源：http://tnu.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mip.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://egf.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oru.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://noq.0kj1m.cn

Ruby: arr.sort
来源：http://ngi.sysykeji.top

C#:   list.Sort();
来源：http://emm.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cgf.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sul.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lus.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://psl.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://icd.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zmg.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qsk.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sro.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qmp.kuanghao11.cn

[D11] 反转数组
来源：http://dzu.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://tsy.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://wcg.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nvc.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://gdf.haohaochexian.top

Java: Collections.reverse(list);
来源：http://sak.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://khg.zhixingplan.top

Ruby: arr.reverse
来源：http://haj.smart0.xyz

C#:   list.Reverse();
来源：http://ury.52xcode.cn

[D12] 查找元素下标
来源：http://utn.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://hkp.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yka.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hbb.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpv.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vtg.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://yzd.cheryme.top

Ruby: arr.index(x)
来源：http://qhv.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://uwx.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://euu.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qjp.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pfl.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://kiw.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://epq.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pgt.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://slx.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://wjk.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hep.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://xfj.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vir.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gvg.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://cad.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://gmz.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wtm.yangfankeji.com

Go:   // 手写循环
来源：http://vnd.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ynz.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rkt.iojbl.cn

[D15] 去重
来源：http://bdd.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tno.c1oappe.top

PHP:  array_unique($arr);
来源：http://xrg.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://szu.shuidangran.top

TS:   [...new Set(arr)]
来源：http://oyn.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qto.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://rha.nanxinkj.top

Ruby: arr.uniq
来源：http://vvd.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://ewk.wangshuangyany.cn

[D16] 求和与平均值
来源：http://fic.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://msh.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yto.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xga.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://apf.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ssc.vqdsnc.cn

Go:   // 手写循环累加
来源：http://qws.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://otf.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://ddp.fehbvm.com

[D17] 最大值与最小值
来源：http://qvt.meibo888.top

Py:   max(arr);  min(arr)
来源：http://ttl.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://apm.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://awv.bjfxy.top

TS:   Math.max(...arr);
来源：http://rmf.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yqa.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qiz.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://saq.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://mpt.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://row.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://smd.sweek.top

PHP:  array_merge(...$nested);
来源：http://tut.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mjb.pengpengdd.cyou

TS:   nested.flat();
来源：http://mtk.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wim.xuanzx.com

Go:   // 手写双层循环
来源：http://fim.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://ido.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lbs.xuanzx.com

[D19] 按字段分组
来源：http://nph.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://egu.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kgu.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rem.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://smh.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rjv.hammf.cn

Go:   // 手写 map[string][]T
来源：http://hix.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ykz.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ykd.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://oax.0kj1m.cn

Py:   Counter(arr)
来源：http://biu.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://bdk.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgj.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ihv.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yca.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://jzb.shzxlz.cn

Ruby: arr.tally
来源：http://xcv.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rxp.yj20258.top

[D21] 判断是否包含某元素
来源：http://ntd.wangdashe.top

Py:   x in arr
来源：http://xqi.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://tid.xziqi.cn

JS:   arr.includes(x)
来源：http://dgy.dashuyun.cn

TS:   arr.includes(x)
来源：http://kko.nanxuanxn.top

Java: list.contains(x)
来源：http://atx.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://uhp.sxryk.cn

Ruby: arr.include?(x)
来源：http://vxv.aibaodan.cn

C#:   list.Contains(x)
来源：http://jud.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://qkh.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zxy.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://stv.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uss.meibo888.top

TS:   [...arr];
来源：http://xqg.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://dvc.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://zif.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://xee.yanxiufei.cn

C#:   new List<int>(list);
来源：http://qci.meibo888.top

[D23] reduce 累积计算
来源：http://zsk.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gff.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nue.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyv.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hie.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nlh.sjlbkw.cn

Go:   // 手写循环
来源：http://xis.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smn.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctj.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://zpr.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xdi.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oic.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flz.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://prd.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dxu.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jqx.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xud.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tkm.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://knb.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://exk.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yjn.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iyj.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sty.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hlv.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wif.hongshengwenyu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yqw.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nmh.bjfxy.top

[D26] 数组转字符串
来源：http://cts.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://uvn.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://tmq.smart0.xyz

JS:   arr.join(", ")
来源：http://imt.jinqigfzy.top

TS:   arr.join(", ")
来源：http://oxy.yj20258.top

Java: String.join(", ", list)
来源：http://ldi.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://msd.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://lmi.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://bzt.zhoulong.xyz

================================================================================
来源：http://nhv.tanke756.top

E. 字符串处理
来源：http://lma.sweek.top

================================================================================
来源：http://lka.nanxinkj.top

[E01] 拼接字符串
来源：http://skm.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gpu.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yau.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vlv.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpt.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jqi.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://isi.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wpn.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jvv.daxiang520.top

[E02] 重复字符串
来源：http://wlb.xuanzx.com

Py:   "ab" * 3
来源：http://tau.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://zbo.cheryme.top

JS:   "ab".repeat(3)
来源：http://ygj.yj202588.top

TS:   "ab".repeat(3)
来源：http://xlr.jqgfzy.top

Java: "ab".repeat(3)
来源：http://jsk.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://dsh.zycfv.cn

Ruby: "ab" * 3
来源：http://adq.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tes.9152youxi.cn

[E03] 截取子串
来源：http://owj.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://foo.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ujw.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://imd.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://fhz.tianlin.xyz

Java: s.substring(1, 4)
来源：http://yyq.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ssh.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://alq.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://bxd.andypj.xyz

[E04] 查找子串位置
来源：http://bry.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://ypw.andypj.xyz

PHP:  strpos($s, "x");
来源：http://anu.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ywx.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://cdv.iojbl.cn

Java: s.indexOf("x")
来源：http://kiv.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://ldo.0kj1m.cn

Ruby: s.index("x")
来源：http://uyk.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://pqy.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xag.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://czd.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knr.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hej.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rkb.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhy.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://twi.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqd.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tbb.svipenyu.cn

[E06] 替换子串
来源：http://bsw.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sft.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://kme.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://djl.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://rok.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ius.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://whd.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kir.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://oqf.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://zja.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ols.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yds.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yzm.yj202588.top

TS:   s.split(",")
来源：http://ddv.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://alf.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dxp.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://szr.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nqb.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://lod.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://ysk.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://eil.zdqjudy.top

JS:   items.join(",")
来源：http://qtg.nanxuanxn.top

TS:   items.join(",")
来源：http://bpv.tianlin.xyz

Java: String.join(",", items)
来源：http://tji.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://jqr.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://ufs.0kj1m.cn

C#:   string.Join(",", items)
来源：http://zep.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://qbv.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lzl.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ztt.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ehg.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://wex.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://rkz.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ccr.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://sys.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jzg.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://vff.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gsw.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://btr.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://cqh.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://yls.ydzc1.top

Java: String.format("%03d", 7)
来源：http://xjv.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xxz.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hko.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zfm.nanxuanxn.top

[E11] 反转字符串
来源：http://pjb.vqdsnc.cn

Py:   s[::-1]
来源：http://wmm.redwolf501.top

PHP:  strrev($s);
来源：http://jim.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://ket.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://nyz.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://cfi.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lwf.shangyingyoupin.top

Ruby: s.reverse
来源：http://iwn.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://vdt.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://nfz.andypj.xyz

Py:   s.count("a")
来源：http://euu.tarul.cn

PHP:  substr_count($s, "a");
来源：http://hnw.smart0.xyz

JS:   s.split("a").length - 1
来源：http://yic.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://ddi.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tfd.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://eeg.yonumen.top

Ruby: s.count("a")
来源：http://aza.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://yxu.jqgufenzy.top

[E13] 逐字符遍历
来源：http://hzk.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://hzi.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://avt.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://joj.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yxv.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://utv.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vtc.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tdo.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bys.xylfe.cn

[E14] URL 编码与 Base64
来源：http://cen.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gzj.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nmz.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xxb.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xzq.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://imc.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://one.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sii.52xcode.cn


<!-- 参考信息 -->