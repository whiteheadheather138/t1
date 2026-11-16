代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ugl.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zeh.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyk.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsy.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://emv.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eqw.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cba.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wim.yj202588.top

[D11] 反转数组
来源：http://hhd.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://jkq.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://gol.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://frg.c1oappe.top

TS:   [...arr].reverse();
来源：http://fnv.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://wkz.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://cdi.yvedp.cn

Ruby: arr.reverse
来源：http://img.vqdsnc.cn

C#:   list.Reverse();
来源：http://ckd.shzxlz.cn

[D12] 查找元素下标
来源：http://dij.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://ktv.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bjr.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yci.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tjq.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aog.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://yhg.zhengqikj.top

Ruby: arr.index(x)
来源：http://res.xinyue.icu

C#:   list.IndexOf(x);
来源：http://bze.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://akp.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gww.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rtg.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://fuj.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://rbz.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iyk.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://llq.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://kal.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lxt.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://nzr.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ock.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sqm.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://zuz.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://vxu.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fko.snrcjt.cn

Go:   // 手写循环
来源：http://iwj.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://vtt.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ryn.jinqigufen.top

[D15] 去重
来源：http://yso.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tcx.havefunace.top

PHP:  array_unique($arr);
来源：http://gqx.mhx1999.top

JS:   [...new Set(arr)]
来源：http://vvo.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://wgr.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blf.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ptu.xziqi.cn

Ruby: arr.uniq
来源：http://fte.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://sor.quarkkingdee.top

[D16] 求和与平均值
来源：http://euu.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://omc.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://psh.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cam.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afi.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rbt.0kj1m.cn

Go:   // 手写循环累加
来源：http://mwu.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uuz.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://fgu.fehbvm.com

[D17] 最大值与最小值
来源：http://klx.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://nyv.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://ebf.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ccu.andypj.xyz

TS:   Math.max(...arr);
来源：http://qnh.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ofm.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nil.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://zqs.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://rai.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://bll.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ysi.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://ndc.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vdn.chenzaomai.com

TS:   nested.flat();
来源：http://dtg.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rvh.hnxiangtu.top

Go:   // 手写双层循环
来源：http://sss.vehdjk.com

Ruby: nested.flatten
来源：http://que.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qpf.andypj.xyz

[D19] 按字段分组
来源：http://wkc.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmg.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nbw.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xgo.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fzd.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uss.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://zfc.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xyb.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ojl.tanke756.top

[D20] 统计每个元素出现次数
来源：http://otj.jyoumei.cn

Py:   Counter(arr)
来源：http://izd.hcnkem.com

PHP:  array_count_values($arr);
来源：http://nva.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dlk.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lkx.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xup.guannengcc.top

Go:   // 手写 map[T]int
来源：http://nno.cashguo.top

Ruby: arr.tally
来源：http://vid.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tvp.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://cmj.daxiang520.top

Py:   x in arr
来源：http://bsn.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://obw.andypj.xyz

JS:   arr.includes(x)
来源：http://lus.hnqzz.top

TS:   arr.includes(x)
来源：http://etd.xylfe.cn

Java: list.contains(x)
来源：http://yjh.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://yea.smart0.xyz

Ruby: arr.include?(x)
来源：http://znd.ppjwa.cn

C#:   list.Contains(x)
来源：http://ook.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://ziz.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xfm.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xtz.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lty.bbcook.cn

TS:   [...arr];
来源：http://gml.iojbl.cn

Java: new ArrayList<>(list);
来源：http://ozf.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://aat.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://ind.yonumen.top

C#:   new List<int>(list);
来源：http://xvs.yonumen.top

[D23] reduce 累积计算
来源：http://bey.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xcr.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pxg.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hnx.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://teo.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tnp.nwbrower.top

Go:   // 手写循环
来源：http://iha.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dno.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yza.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://gcc.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfd.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wcu.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vuj.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bha.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xlm.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qgo.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://poj.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://trl.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://ull.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dgg.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ndv.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vmc.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vlp.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tip.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://edx.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wez.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dnq.gaohongyu789.top

[D26] 数组转字符串
来源：http://yuh.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://dgi.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://wqz.bjfxy.top

JS:   arr.join(", ")
来源：http://ecl.nwbrower.top

TS:   arr.join(", ")
来源：http://fwe.tarul.cn

Java: String.join(", ", list)
来源：http://ycu.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://ztm.zycfv.cn

Ruby: arr.join(", ")
来源：http://szc.smart0.xyz

C#:   string.Join(", ", list)
来源：http://nur.xuanzx.com

================================================================================
来源：http://hwv.0kj1m.cn

E. 字符串处理
来源：http://xhh.hnqzz.top

================================================================================
来源：http://nwf.yueranfly.top

[E01] 拼接字符串
来源：http://vwr.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qwy.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eoe.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oin.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://acc.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://thq.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wci.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nxs.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzh.sufxvd.cn

[E02] 重复字符串
来源：http://dye.kuanghao11.cn

Py:   "ab" * 3
来源：http://vab.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://dpv.yj20258.top

JS:   "ab".repeat(3)
来源：http://wad.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://ylf.yj20258888.top

Java: "ab".repeat(3)
来源：http://lcz.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://fmd.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://gjq.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bqi.cheryme.top

[E03] 截取子串
来源：http://dqm.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://egr.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xnw.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cjh.wangdashe.top

TS:   s.slice(1, 4)
来源：http://mdj.zdbjq.cn

Java: s.substring(1, 4)
来源：http://lyy.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fzg.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://bsy.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://azj.sysykeji.top

[E04] 查找子串位置
来源：http://nis.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://ixk.guannengcc.top

PHP:  strpos($s, "x");
来源：http://qje.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wrj.wangdashe.top

TS:   s.indexOf("x")
来源：http://ojo.zdbjq.cn

Java: s.indexOf("x")
来源：http://hok.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://kzq.chenjidiqi.icu

Ruby: s.index("x")
来源：http://gto.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://odc.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ycn.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxo.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pkj.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cnw.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lbh.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftt.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pou.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://byv.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pym.cheryme.top

[E06] 替换子串
来源：http://tjr.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qml.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://lru.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbx.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://nbj.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://air.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://miz.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yjr.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://fhw.zhengqikj.top

[E07] 按分隔符拆分
来源：http://nhi.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zis.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vat.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ffg.daxiang520.top

TS:   s.split(",")
来源：http://ycf.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ccg.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cpb.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://aos.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nuk.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://elw.wangshuangyany.cn

Py:   ",".join(items)
来源：http://fjc.c1oappe.top

PHP:  implode(",", $items);
来源：http://nht.cucudq.cn

JS:   items.join(",")
来源：http://xau.9152youxi.cn

TS:   items.join(",")
来源：http://kva.hfpthk.cn

Java: String.join(",", items)
来源：http://jgj.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://rwd.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://szv.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://qpt.yvedp.cn

[E09] 去除所有空白字符
来源：http://pnd.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xdf.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vxq.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://dvm.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://tdk.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://xlm.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rya.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://fkh.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ljb.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://has.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ish.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nbo.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://pgy.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://orr.hesvh.cn

Java: String.format("%03d", 7)
来源：http://jye.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://aey.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lvq.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aha.gaohongyu789.top

[E11] 反转字符串
来源：http://ogt.dianchejie.cn

Py:   s[::-1]
来源：http://jrq.epnwcf.com

PHP:  strrev($s);
来源：http://hsu.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://vrk.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://nrk.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://euz.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tcl.andypj.xyz

Ruby: s.reverse
来源：http://xqx.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://ieu.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://xln.meibo888.top

Py:   s.count("a")
来源：http://cno.ivvv.top

PHP:  substr_count($s, "a");
来源：http://nqh.ivvv.top

JS:   s.split("a").length - 1
来源：http://pdf.yonumen.top

TS:   s.split("a").length - 1
来源：http://asn.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bso.yj20258.top

Go:   strings.Count(s, "a")
来源：http://jbb.guannengcc.top

Ruby: s.count("a")
来源：http://pkx.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://nzm.hysaishi.cn

[E13] 逐字符遍历
来源：http://sox.meibo888.top

Py:   for ch in s: print(ch)
来源：http://vfx.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bqo.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ccs.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lbg.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fhz.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hxn.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://yzo.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zip.havefunace.top

[E14] URL 编码与 Base64
来源：http://dme.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ign.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jjl.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xoe.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gme.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sor.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dgq.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ttu.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsq.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://jac.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ygb.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wju.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kov.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://unz.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mnn.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aau.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uhk.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dvk.sufxvd.cn

[E16] 数字千分位
来源：http://pdd.c1oappe.top

Py:   f"{1234567:,}"
来源：http://gzg.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://dbi.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ysy.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dsc.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kuv.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nvu.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qrv.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://bgy.ydzc1.top

[E17] 首字母大写
来源：http://pvi.fktsv.cn


<!-- 参考信息 -->