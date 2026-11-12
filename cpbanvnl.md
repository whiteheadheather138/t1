代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://rnc.aibaodan.cn

TS:   [...a, ...b];
来源：http://vby.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mjk.yj20258888.top

Go:   append(a, b...)
来源：http://aql.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://dhb.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://fan.birdmap.top

[D09] 排序（升序）
来源：http://cpv.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://brq.nanxuanxn.top

PHP:  sort($arr);
来源：http://tbk.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uhx.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dnw.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://bdr.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtj.jinqigufen.top

Ruby: arr.sort
来源：http://bgt.cashguo.top

C#:   list.Sort();
来源：http://bco.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ayj.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cav.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eal.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://brx.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgs.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tkv.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hli.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://adh.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jtz.yanxiufei.cn

[D11] 反转数组
来源：http://rkn.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://bhy.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://nll.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xgp.meibo888.top

TS:   [...arr].reverse();
来源：http://xbg.dashuyun.cn

Java: Collections.reverse(list);
来源：http://rvz.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://jdc.yj20258.top

Ruby: arr.reverse
来源：http://jox.pengpengdd.cyou

C#:   list.Reverse();
来源：http://lph.meibo888.top

[D12] 查找元素下标
来源：http://oos.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://cnl.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://onh.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://auj.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://soi.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bea.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://xia.vehdjk.com

Ruby: arr.index(x)
来源：http://jwd.sweek.top

C#:   list.IndexOf(x);
来源：http://nyq.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://ifp.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uib.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wke.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://krz.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://nrc.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bsi.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bcn.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://euu.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://syh.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://lep.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rtq.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ykx.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://rzk.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://knx.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eel.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://qsa.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zvd.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://azt.chenlongwang.top

[D15] 去重
来源：http://jmx.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zrf.hysaishi.cn

PHP:  array_unique($arr);
来源：http://mph.ybcxt.top

JS:   [...new Set(arr)]
来源：http://zhh.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://ame.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kdj.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://ueh.tarul.cn

Ruby: arr.uniq
来源：http://lmm.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://osx.epnwcf.com

[D16] 求和与平均值
来源：http://nxf.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://znt.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gsm.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dmm.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oad.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fur.zdbjq.cn

Go:   // 手写循环累加
来源：http://vsw.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gol.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://duv.ivvv.top

[D17] 最大值与最小值
来源：http://rri.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://pta.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://pze.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ztp.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://mql.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://pnl.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pne.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://sie.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://uyh.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://fsj.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ogb.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://tlf.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lzp.pengpengdd.cyou

TS:   nested.flat();
来源：http://nnj.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cwt.kuanghao11.cn

Go:   // 手写双层循环
来源：http://abo.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://fyk.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://trq.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://apo.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iua.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vpe.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://txn.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yxu.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eps.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://krj.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://moc.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://udp.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://jns.fzhhl.top

Py:   Counter(arr)
来源：http://jsc.cucudq.cn

PHP:  array_count_values($arr);
来源：http://eui.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qlf.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxo.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cnv.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://pzd.meibo888.top

Ruby: arr.tally
来源：http://wyl.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axe.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://pfp.yuanzhike.top

Py:   x in arr
来源：http://zhl.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://qel.vqdsnc.cn

JS:   arr.includes(x)
来源：http://kek.xziqi.cn

TS:   arr.includes(x)
来源：http://akc.quarkkingdee.top

Java: list.contains(x)
来源：http://juu.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://weh.bbcook.cn

Ruby: arr.include?(x)
来源：http://mlo.fzhhl.top

C#:   list.Contains(x)
来源：http://vzr.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://awg.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nnl.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yqr.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wqu.cdnleiting.top

TS:   [...arr];
来源：http://inu.bbcook.cn

Java: new ArrayList<>(list);
来源：http://car.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://lxi.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://giv.nwbrower.top

C#:   new List<int>(list);
来源：http://jbe.mhx1999.top

[D23] reduce 累积计算
来源：http://zuz.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xxs.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://der.zhiwuduotai.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmy.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ruv.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fpn.redwolf501.top

Go:   // 手写循环
来源：http://zty.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wcq.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gzz.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://yfn.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rhc.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xbu.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://agh.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eku.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvi.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uvo.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mvz.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://okg.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://hdj.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fuv.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://npy.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vye.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dww.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wke.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aqv.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yhn.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jii.jyoumei.cn

[D26] 数组转字符串
来源：http://ofe.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://zfs.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://wmw.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://ahx.birdmap.top

TS:   arr.join(", ")
来源：http://rwh.wangdashe.top

Java: String.join(", ", list)
来源：http://jym.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://aai.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://bmc.fzhhl.top

C#:   string.Join(", ", list)
来源：http://ztp.zhiwuduotai.top

================================================================================
来源：http://nrg.c1oappe.top

E. 字符串处理
来源：http://mwh.zdbjq.cn

================================================================================
来源：http://kjh.0kj1m.cn

[E01] 拼接字符串
来源：http://obo.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hbd.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axo.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://voq.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xud.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wlk.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://crh.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mlj.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gxp.daria6918.cn

[E02] 重复字符串
来源：http://jcp.zdqjudy.top

Py:   "ab" * 3
来源：http://akv.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://hvk.52xcode.cn

JS:   "ab".repeat(3)
来源：http://ikg.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://tyk.epnwcf.com

Java: "ab".repeat(3)
来源：http://oit.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://hql.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://eox.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tri.shzxlz.cn

[E03] 截取子串
来源：http://okh.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gqd.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ois.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aef.uphjek.com

TS:   s.slice(1, 4)
来源：http://iew.zdqjudy.top

Java: s.substring(1, 4)
来源：http://rcj.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gzx.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uiv.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://fym.zhixingplan.top

[E04] 查找子串位置
来源：http://nab.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://lea.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://orr.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpy.yuanzhike.top

TS:   s.indexOf("x")
来源：http://cho.ybcxt.top

Java: s.indexOf("x")
来源：http://kaq.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://wwy.wangdashe.top

Ruby: s.index("x")
来源：http://bhg.vehdjk.com

C#:   s.IndexOf("x")
来源：http://ooa.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://csp.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ghp.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kns.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jsk.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://efm.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aey.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bjj.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ahz.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tag.hfpthk.cn

[E06] 替换子串
来源：http://azb.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://niq.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://ion.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dnf.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://ohr.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ywv.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tgt.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xvd.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://ywy.zdbjq.cn

[E07] 按分隔符拆分
来源：http://wlj.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tuy.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://voi.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ihf.cashguo.top

TS:   s.split(",")
来源：http://ddu.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mmv.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ayc.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://rms.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mbg.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://kvi.xziqi.cn

Py:   ",".join(items)
来源：http://nsw.ppjwa.cn

PHP:  implode(",", $items);
来源：http://bwe.jianghu66.top

JS:   items.join(",")
来源：http://gsb.bbcook.cn

TS:   items.join(",")
来源：http://bhs.mhx1999.top

Java: String.join(",", items)
来源：http://pvm.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://zva.iojbl.cn

Ruby: items.join(",")
来源：http://rfb.chenzaomai.com

C#:   string.Join(",", items)
来源：http://ejv.zhengqikj.top

[E09] 去除所有空白字符
来源：http://pig.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iip.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cds.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://hvi.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://rxp.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://ulh.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://tga.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://daz.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pun.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://zgi.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gpv.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mrp.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://bme.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://lpg.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://wga.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://syx.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lan.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kyv.zhengqikj.top

[E11] 反转字符串
来源：http://jtz.ivvv.top

Py:   s[::-1]
来源：http://bnb.quarkkingdee.top

PHP:  strrev($s);
来源：http://lfb.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://dnk.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://vym.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gob.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kkb.pycfn.com

Ruby: s.reverse
来源：http://pzr.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dff.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://zwy.jinghuilouyu.cn

Py:   s.count("a")
来源：http://vju.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ifb.cucudq.cn

JS:   s.split("a").length - 1
来源：http://lhd.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://bhu.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://foi.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://ydq.pycfn.com

Ruby: s.count("a")
来源：http://qhh.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://coq.316326.xyz

[E13] 逐字符遍历
来源：http://ezq.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://pcg.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://asu.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://toq.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://boj.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qkl.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vps.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://knm.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wyo.yuxming.cn

[E14] URL 编码与 Base64
来源：http://zwv.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tig.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kbj.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hnx.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jha.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mvs.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://btw.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://edx.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dzy.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://fjd.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rsh.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ofl.birdmap.top


<!-- 参考信息 -->