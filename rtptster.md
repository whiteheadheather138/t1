代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://jta.hnqzz.top

[D08] 合并两个数组
来源：http://hgm.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://tgk.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://rfk.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hwo.redwolf501.top

TS:   [...a, ...b];
来源：http://gqk.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://anp.xinyue.icu

Go:   append(a, b...)
来源：http://lum.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://vwh.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://epl.tian-w.cn

[D09] 排序（升序）
来源：http://ebj.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://rez.shzxlz.cn

PHP:  sort($arr);
来源：http://kto.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uof.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bgr.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nsl.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nod.birdmap.top

Ruby: arr.sort
来源：http://gny.gogol.net.cn

C#:   list.Sort();
来源：http://oyj.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ubx.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://neo.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wug.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wua.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://msn.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ves.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ckp.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://azt.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ebe.chenjidiqi.icu

[D11] 反转数组
来源：http://olb.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://klt.bbcook.cn

PHP:  array_reverse($arr);
来源：http://fnh.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pwu.nwbrower.top

TS:   [...arr].reverse();
来源：http://pku.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://kvl.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://jvh.cashguo.top

Ruby: arr.reverse
来源：http://rch.jianghu66.top

C#:   list.Reverse();
来源：http://lhu.jqgfzy.top

[D12] 查找元素下标
来源：http://vxp.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://bmb.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgv.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpb.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ssy.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qiw.yj202588.top

Go:   slices.Index(arr, x)
来源：http://mgh.bjfxy.top

Ruby: arr.index(x)
来源：http://zqb.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://upn.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://kgm.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jxp.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzd.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://lfc.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://nyr.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jbe.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hib.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ubo.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uyn.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://lpy.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wuy.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fhh.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://vus.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://dvn.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tpx.zdbjq.cn

Go:   // 手写循环
来源：http://yom.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nkv.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nwk.fehbvm.com

[D15] 去重
来源：http://qfv.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://arz.yj20258.top

PHP:  array_unique($arr);
来源：http://rmn.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://ory.shuidangran.top

TS:   [...new Set(arr)]
来源：http://ede.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fcc.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://auf.tian-w.cn

Ruby: arr.uniq
来源：http://jjx.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://mcd.birdmap.top

[D16] 求和与平均值
来源：http://grh.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ufh.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yhh.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jnv.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eby.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xzp.nanxuanxn.top

Go:   // 手写循环累加
来源：http://auj.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ehd.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://eir.hcnkem.com

[D17] 最大值与最小值
来源：http://rxq.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://cjl.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://mxd.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xlz.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://qid.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ima.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://img.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://sbh.cheryme.top

C#:   list.Max();  list.Min()
来源：http://gga.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://lni.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iil.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://qhq.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sdl.yanxiufei.cn

TS:   nested.flat();
来源：http://jsw.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://piq.sxryk.cn

Go:   // 手写双层循环
来源：http://mhd.gzhubu.top

Ruby: nested.flatten
来源：http://tiy.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bxk.gaohongyu789.top

[D19] 按字段分组
来源：http://snh.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nyh.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uyv.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hba.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://huk.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hey.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://iii.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sbt.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yqo.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://lis.daria6918.cn

Py:   Counter(arr)
来源：http://eom.yvedp.cn

PHP:  array_count_values($arr);
来源：http://zhf.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eue.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ugf.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://syl.yuxming.cn

Go:   // 手写 map[T]int
来源：http://nob.chenjidiqi.icu

Ruby: arr.tally
来源：http://fug.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hfa.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://phd.gogol.net.cn

Py:   x in arr
来源：http://okm.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://vje.hammf.cn

JS:   arr.includes(x)
来源：http://uba.hnqzz.top

TS:   arr.includes(x)
来源：http://yol.smart0.xyz

Java: list.contains(x)
来源：http://eyu.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://njf.aibaodan.cn

Ruby: arr.include?(x)
来源：http://vpv.redwolf501.top

C#:   list.Contains(x)
来源：http://wpa.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://dvz.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rov.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sjg.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brs.svipenyu.cn

TS:   [...arr];
来源：http://pvs.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://gry.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hoz.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://qdx.tanke756.top

C#:   new List<int>(list);
来源：http://fsx.yfazqb.com

[D23] reduce 累积计算
来源：http://msm.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://awg.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rbr.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zux.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjj.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ayx.hnqzz.top

Go:   // 手写循环
来源：http://upn.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://evj.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kjc.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://vza.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ucx.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yve.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hoa.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://coe.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fow.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hsc.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zfi.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://srs.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://pac.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vlw.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://czx.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kwz.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uik.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jfm.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bpz.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mjz.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jdg.zhixingplan.top

[D26] 数组转字符串
来源：http://yip.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://jff.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://txr.ppjwa.cn

JS:   arr.join(", ")
来源：http://ahy.yuxming.cn

TS:   arr.join(", ")
来源：http://gdh.hammf.cn

Java: String.join(", ", list)
来源：http://bfd.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://hpw.guowangkeji.top

Ruby: arr.join(", ")
来源：http://tot.tian-w.cn

C#:   string.Join(", ", list)
来源：http://rxf.birdmap.top

================================================================================
来源：http://tla.316326.xyz

E. 字符串处理
来源：http://zre.zhaomingkeji.xyz

================================================================================
来源：http://ovd.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://vnr.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aux.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zxb.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gar.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbi.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tjw.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vub.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fca.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qid.xziqi.cn

[E02] 重复字符串
来源：http://gif.smart0.xyz

Py:   "ab" * 3
来源：http://esg.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://sgb.guannengcc.top

JS:   "ab".repeat(3)
来源：http://dtm.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://pjd.hcnkem.com

Java: "ab".repeat(3)
来源：http://ghr.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hwl.ppjwa.cn

Ruby: "ab" * 3
来源：http://vjp.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tmo.hammf.cn

[E03] 截取子串
来源：http://zsc.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://art.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rby.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://edp.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://uwe.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://anw.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uem.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wor.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://eyd.mhx1999.top

[E04] 查找子串位置
来源：http://lud.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://wfu.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://moi.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fhv.pycfn.com

TS:   s.indexOf("x")
来源：http://khn.gaohongyu789.top

Java: s.indexOf("x")
来源：http://hds.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://peh.fengsongda.top

Ruby: s.index("x")
来源：http://nis.hcnkem.com

C#:   s.IndexOf("x")
来源：http://kft.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wad.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vlj.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nuu.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kul.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gjk.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://usu.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cht.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://los.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rlk.yuanzhike.top

[E06] 替换子串
来源：http://sxv.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xst.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://ayq.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgp.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://nvg.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wnp.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ttg.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rab.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://eyq.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://pgq.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kgu.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ehl.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lwi.bbcook.cn

TS:   s.split(",")
来源：http://zqt.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://eys.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zii.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://qph.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lyu.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://jvm.zhixingplan.top

Py:   ",".join(items)
来源：http://xuz.cucudq.cn

PHP:  implode(",", $items);
来源：http://ftx.cqqwz.cn

JS:   items.join(",")
来源：http://ofi.jianghu66.top

TS:   items.join(",")
来源：http://qkc.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://stz.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://occ.hesvh.cn

Ruby: items.join(",")
来源：http://ame.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://fus.epnwcf.com

[E09] 去除所有空白字符
来源：http://vua.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wmu.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oep.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://xgu.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vuf.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://tul.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ztr.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://bhc.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tbw.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://lgo.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://otu.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ncs.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://nql.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://vsu.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://edq.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rgs.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aog.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kyq.chenjidiqi.icu

[E11] 反转字符串
来源：http://wvm.bjfxy.top

Py:   s[::-1]
来源：http://ypi.dianchejie.cn

PHP:  strrev($s);
来源：http://kyt.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://jsu.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://bsu.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://kig.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://lcf.jinqigufen.top

Ruby: s.reverse
来源：http://lbg.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://prr.bbcook.cn

[E12] 统计某字符出现次数
来源：http://yoh.zhijiandao.cn

Py:   s.count("a")
来源：http://xzg.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://wzy.jianghu66.top

JS:   s.split("a").length - 1
来源：http://yrk.ybcxt.top

TS:   s.split("a").length - 1
来源：http://bhl.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cnz.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://pjz.hesvh.cn

Ruby: s.count("a")
来源：http://kvc.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://ykz.daria6918.cn

[E13] 逐字符遍历
来源：http://uun.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://ets.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kyq.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tuu.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qgk.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://quv.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wtq.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://myn.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zed.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://ffi.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jwx.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ifc.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iyg.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rtk.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ody.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uzs.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hkb.pycfn.com


<!-- 参考信息 -->