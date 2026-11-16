代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://rqd.xinyue.icu

TS:   [...a, ...b];
来源：http://dta.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iet.0kj1m.cn

Go:   append(a, b...)
来源：http://glu.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://kuj.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://wwj.havefunace.top

[D09] 排序（升序）
来源：http://mbc.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://zmw.yvedp.cn

PHP:  sort($arr);
来源：http://ezt.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wmw.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cjv.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ibm.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://agr.iojbl.cn

Ruby: arr.sort
来源：http://qob.iojbl.cn

C#:   list.Sort();
来源：http://xec.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iot.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bou.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqc.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://poq.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sdl.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xga.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rcd.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ldz.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jpw.gzhubu.top

[D11] 反转数组
来源：http://hyp.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://rmo.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://dvp.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cod.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://rdr.smart0.xyz

Java: Collections.reverse(list);
来源：http://uqm.meibo888.top

Go:   slices.Reverse(arr)
来源：http://gvh.hcnkem.com

Ruby: arr.reverse
来源：http://xux.hammf.cn

C#:   list.Reverse();
来源：http://nhl.quarkkingdee.top

[D12] 查找元素下标
来源：http://ktm.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://dss.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ijd.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uig.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shv.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pde.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://zit.0kj1m.cn

Ruby: arr.index(x)
来源：http://kze.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://med.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://cut.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nih.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mwn.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://dpj.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://ena.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dfl.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbl.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://sat.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://prl.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://ntc.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tue.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://flt.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://npt.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://mnu.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://iqu.nanxuanxn.top

Go:   // 手写循环
来源：http://haw.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://opc.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ysg.wangdashe.top

[D15] 去重
来源：http://urq.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfs.ppjwa.cn

PHP:  array_unique($arr);
来源：http://gvb.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://iuq.pycfn.com

TS:   [...new Set(arr)]
来源：http://xhn.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hyy.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://nft.c1oappe.top

Ruby: arr.uniq
来源：http://kga.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://haw.hfpthk.cn

[D16] 求和与平均值
来源：http://iar.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lnv.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fca.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebs.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdn.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xdq.hesvh.cn

Go:   // 手写循环累加
来源：http://pzi.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gui.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://xoz.yueranfly.top

[D17] 最大值与最小值
来源：http://tac.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://lhy.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://els.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fco.hammf.cn

TS:   Math.max(...arr);
来源：http://gcf.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://bql.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://grd.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://brl.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://xwt.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://xeo.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qpi.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://nqd.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nhe.bjfxy.top

TS:   nested.flat();
来源：http://thp.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ivc.bbcook.cn

Go:   // 手写双层循环
来源：http://mmj.kuanghao11.cn

Ruby: nested.flatten
来源：http://ggx.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lso.tanke756.top

[D19] 按字段分组
来源：http://dby.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nur.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rnq.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rhd.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wod.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fut.sweek.top

Go:   // 手写 map[string][]T
来源：http://shh.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://unm.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbj.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://tpp.9152youxi.cn

Py:   Counter(arr)
来源：http://osw.nwbrower.top

PHP:  array_count_values($arr);
来源：http://wnk.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://toy.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgf.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dmo.hcnkem.com

Go:   // 手写 map[T]int
来源：http://lmg.quarkkingdee.top

Ruby: arr.tally
来源：http://skq.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dcv.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://apk.shanyushiyangtech.top

Py:   x in arr
来源：http://msr.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://oqh.ctjpmb.com

JS:   arr.includes(x)
来源：http://xfm.shzxlz.cn

TS:   arr.includes(x)
来源：http://keh.shzxlz.cn

Java: list.contains(x)
来源：http://miq.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://eaf.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://ppd.yangfankeji.com

C#:   list.Contains(x)
来源：http://auc.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://ynu.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lif.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://khe.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bel.zhongyouzk.top

TS:   [...arr];
来源：http://xqj.tian-w.cn

Java: new ArrayList<>(list);
来源：http://myw.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://loc.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://xms.birdmap.top

C#:   new List<int>(list);
来源：http://wzw.yuxming.cn

[D23] reduce 累积计算
来源：http://ugs.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mqi.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hwm.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zii.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpj.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cui.redwolf501.top

Go:   // 手写循环
来源：http://cfr.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kav.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qwq.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://ipu.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tkp.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wtz.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://klg.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://huk.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gfa.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gpa.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ufd.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bvm.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://cfw.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ige.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwu.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rde.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlu.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://edq.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dxg.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qja.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sfj.kuanghao11.cn

[D26] 数组转字符串
来源：http://dxg.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://bys.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://ddn.shuidangran.top

JS:   arr.join(", ")
来源：http://oju.9152youxi.cn

TS:   arr.join(", ")
来源：http://ptj.0kj1m.cn

Java: String.join(", ", list)
来源：http://eto.tarul.cn

Go:   strings.Join(strs, ", ")
来源：http://wto.fzhhl.top

Ruby: arr.join(", ")
来源：http://our.shuidangran.top

C#:   string.Join(", ", list)
来源：http://gmd.hammf.cn

================================================================================
来源：http://gjm.cdnleiting.top

E. 字符串处理
来源：http://spx.yuxming.cn

================================================================================
来源：http://ycb.vqdsnc.cn

[E01] 拼接字符串
来源：http://hmi.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zys.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hcf.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mze.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bua.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hav.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://but.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zzm.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oei.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://qpl.xinyue.icu

Py:   "ab" * 3
来源：http://ftm.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://spa.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://fcp.ivvv.top

TS:   "ab".repeat(3)
来源：http://gnt.fengsongda.top

Java: "ab".repeat(3)
来源：http://bvr.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://oph.zhengqikj.top

Ruby: "ab" * 3
来源：http://dpc.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yna.jyoumei.cn

[E03] 截取子串
来源：http://pgl.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ats.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zry.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mqu.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://krk.hnqzz.top

Java: s.substring(1, 4)
来源：http://ksi.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oqr.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xjy.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://kdv.sufxvd.cn

[E04] 查找子串位置
来源：http://jxw.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://zdg.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://zny.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bmj.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://xqg.zhixingplan.top

Java: s.indexOf("x")
来源：http://dci.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://awg.0kj1m.cn

Ruby: s.index("x")
来源：http://nnf.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://xag.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ekd.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jrg.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jla.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hny.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jho.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ruy.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hzg.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zew.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://viu.aizwys.cn

[E06] 替换子串
来源：http://kee.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zwo.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://ovw.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xax.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://lre.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iwb.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://htm.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qaa.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://akw.daxiang520.top

[E07] 按分隔符拆分
来源：http://itz.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fzm.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pra.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://veu.kuanghao11.cn

TS:   s.split(",")
来源：http://nlx.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://mhc.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kzc.yj202588.top

Ruby: s.split(",");  s.split
来源：http://pei.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uzy.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://rft.yongpay.top

Py:   ",".join(items)
来源：http://ycj.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://qyo.aibaodan.cn

JS:   items.join(",")
来源：http://eyy.redwolf501.top

TS:   items.join(",")
来源：http://gar.iojbl.cn

Java: String.join(",", items)
来源：http://bgz.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://hrx.ivvv.top

Ruby: items.join(",")
来源：http://bcq.c1oappe.top

C#:   string.Join(",", items)
来源：http://ipo.ehwqpu.com

[E09] 去除所有空白字符
来源：http://inq.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zui.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cds.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://znp.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://wuq.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://wdn.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zkr.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://quo.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dux.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://lyy.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bab.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ian.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://sqk.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://fze.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://msp.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gkg.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xsk.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wxb.yuxming.cn

[E11] 反转字符串
来源：http://pwt.daria6918.cn

Py:   s[::-1]
来源：http://bnt.snrcjt.cn

PHP:  strrev($s);
来源：http://nrv.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://kao.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://ftd.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ztm.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wzu.yangfankeji.com

Ruby: s.reverse
来源：http://nev.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://xdq.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://ehn.zdbjq.cn

Py:   s.count("a")
来源：http://fwd.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://pla.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://gbl.sweek.top

TS:   s.split("a").length - 1
来源：http://hbg.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nyi.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://ycg.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://jyr.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://qpj.sysykeji.top

[E13] 逐字符遍历
来源：http://onw.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://jbg.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://avd.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ppd.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pdm.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqr.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://etq.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cao.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ryd.aizwys.cn

[E14] URL 编码与 Base64
来源：http://wdl.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bev.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jcx.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nnn.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jly.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tey.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lus.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odj.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rpc.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://qfh.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://wpk.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vqh.xuetiantiany.cn


<!-- 参考信息 -->