代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://fwz.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://zqu.hesvh.cn

[D09] 排序（升序）
来源：http://jna.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kas.hongshengwenyu.top

PHP:  sort($arr);
来源：http://oez.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://unk.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aoz.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hjj.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hzj.ivvv.top

Ruby: arr.sort
来源：http://xxl.ehwqpu.com

C#:   list.Sort();
来源：http://azg.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jue.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://emy.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://agc.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://luc.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zpg.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mxb.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qij.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://old.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nmk.hfpthk.cn

[D11] 反转数组
来源：http://nua.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pvx.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://ipj.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yhf.yj20258888.top

TS:   [...arr].reverse();
来源：http://ouw.havefunace.top

Java: Collections.reverse(list);
来源：http://tkr.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://frw.ydzc1.top

Ruby: arr.reverse
来源：http://mdl.hesvh.cn

C#:   list.Reverse();
来源：http://elj.sjlbkw.cn

[D12] 查找元素下标
来源：http://zux.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://tjy.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://taq.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjp.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yia.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ioo.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://ini.yangfankeji.com

Ruby: arr.index(x)
来源：http://pyt.daria6918.cn

C#:   list.IndexOf(x);
来源：http://grl.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://zvo.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uld.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zjl.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://izq.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://yvg.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rfq.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xuh.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tua.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cit.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://fqg.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imn.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qro.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://csw.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://lxp.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mrx.bjfxy.top

Go:   // 手写循环
来源：http://jpu.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bna.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fxx.smart0.xyz

[D15] 去重
来源：http://keh.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://drz.chenzaomai.com

PHP:  array_unique($arr);
来源：http://bal.fengsongda.top

JS:   [...new Set(arr)]
来源：http://fgm.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://pki.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://brf.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://taq.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://joz.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://ycp.zdbjq.cn

[D16] 求和与平均值
来源：http://lmb.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyf.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ubm.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kaj.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xkr.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tmi.jinqigfzy.top

Go:   // 手写循环累加
来源：http://kbm.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lil.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://xmq.gotoacloud.top

[D17] 最大值与最小值
来源：http://gee.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://wjp.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://joh.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wik.tian-w.cn

TS:   Math.max(...arr);
来源：http://cad.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nrq.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xsb.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://hjs.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://asx.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://emf.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://glq.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://lgk.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nkw.sysykeji.top

TS:   nested.flat();
来源：http://tkd.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://esh.gzhubu.top

Go:   // 手写双层循环
来源：http://flu.chenjidiqi.icu

Ruby: nested.flatten
来源：http://cxa.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ydd.daria6918.cn

[D19] 按字段分组
来源：http://wpd.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mns.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zli.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pkc.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://cuf.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kxd.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://kyg.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://myh.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pse.hammf.cn

[D20] 统计每个元素出现次数
来源：http://isb.jianghu66.top

Py:   Counter(arr)
来源：http://twy.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://gyx.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpz.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://chj.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ixr.meibo888.top

Go:   // 手写 map[T]int
来源：http://hka.zhijiandao.cn

Ruby: arr.tally
来源：http://vbt.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ubr.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://goh.shzxlz.cn

Py:   x in arr
来源：http://vzt.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://fhx.quarkkingdee.top

JS:   arr.includes(x)
来源：http://aze.ydzc1.top

TS:   arr.includes(x)
来源：http://vxe.yj202588.top

Java: list.contains(x)
来源：http://hfs.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://kfg.ppjwa.cn

Ruby: arr.include?(x)
来源：http://cai.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://tle.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://tzq.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kfn.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://paf.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://opy.vehdjk.com

TS:   [...arr];
来源：http://yqw.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://vks.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://ovr.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://uhc.ehwqpu.com

C#:   new List<int>(list);
来源：http://auq.jinqigufen.top

[D23] reduce 累积计算
来源：http://ixq.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zjd.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jib.zhiwuduotai.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://add.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kln.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nje.snrcjt.cn

Go:   // 手写循环
来源：http://anr.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qcm.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vor.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://ihq.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqr.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ovb.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://upj.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mmp.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dqc.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pry.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qei.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://alv.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://bix.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hgc.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xha.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ncg.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zzd.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://czb.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qfr.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vbg.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tsb.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://kqh.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://ukv.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://goc.quarkkingdee.top

JS:   arr.join(", ")
来源：http://guh.jinqigufen.top

TS:   arr.join(", ")
来源：http://zco.haohaochexian.top

Java: String.join(", ", list)
来源：http://qkx.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://idp.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://pzw.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://joy.xziqi.cn

================================================================================
来源：http://rqx.sysykeji.top

E. 字符串处理
来源：http://iwx.zdqjudy.top

================================================================================
来源：http://zwp.smart0.xyz

[E01] 拼接字符串
来源：http://xgs.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yzc.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cov.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xau.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxy.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lue.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lmx.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vvl.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://awu.daxiang520.top

[E02] 重复字符串
来源：http://rug.chenjidiqi.icu

Py:   "ab" * 3
来源：http://pma.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://zti.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://jfs.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://phd.wangdashe.top

Java: "ab".repeat(3)
来源：http://qik.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://raa.sjlbkw.cn

Ruby: "ab" * 3
来源：http://kbr.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jnk.sufxvd.cn

[E03] 截取子串
来源：http://qzq.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://adt.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pdt.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dhu.xziqi.cn

TS:   s.slice(1, 4)
来源：http://shp.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://yfb.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cmc.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zte.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://lzc.xylfe.cn

[E04] 查找子串位置
来源：http://ium.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://elo.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://gem.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ltf.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://avo.tian-w.cn

Java: s.indexOf("x")
来源：http://aae.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://sqe.tianlin.xyz

Ruby: s.index("x")
来源：http://rzb.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://koh.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hhy.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fis.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hld.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kws.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jdx.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyy.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lnh.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://opm.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bah.hywenlv.cn

[E06] 替换子串
来源：http://azq.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ybz.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://rxr.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mci.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://zft.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikb.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mxy.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmv.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://ljb.snrcjt.cn

[E07] 按分隔符拆分
来源：http://llp.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kdb.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rpp.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aie.mhx1999.top

TS:   s.split(",")
来源：http://eap.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://ecm.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lfi.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://qhh.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ddq.fehbvm.com

[E08] 数组按分隔符合并
来源：http://gex.meibo888.top

Py:   ",".join(items)
来源：http://knj.shzxlz.cn

PHP:  implode(",", $items);
来源：http://nwp.yj20258.top

JS:   items.join(",")
来源：http://vle.fktsv.cn

TS:   items.join(",")
来源：http://yyq.chenlongwang.top

Java: String.join(",", items)
来源：http://sjd.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://hiz.meibo888.top

Ruby: items.join(",")
来源：http://fqg.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://bpa.havefunace.top

[E09] 去除所有空白字符
来源：http://jew.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oes.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ibm.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://zsx.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://fga.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://zha.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yak.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://vny.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xdw.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://jrk.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fja.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://asf.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://kvt.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://fra.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://zar.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iem.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fev.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ebg.svipenyu.cn

[E11] 反转字符串
来源：http://yno.hnxiangtu.top

Py:   s[::-1]
来源：http://atx.yj20258.top

PHP:  strrev($s);
来源：http://aiq.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://gus.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://ofv.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://evx.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ctx.hongshengwenyu.top

Ruby: s.reverse
来源：http://eae.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://veo.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://rtb.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://plc.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://elq.smart0.xyz

JS:   s.split("a").length - 1
来源：http://xsm.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://cqa.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ybc.birdmap.top

Go:   strings.Count(s, "a")
来源：http://bhm.nanxuanxn.top

Ruby: s.count("a")
来源：http://nol.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://xns.xziqi.cn

[E13] 逐字符遍历
来源：http://cyu.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://piw.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://edm.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hxv.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://kpo.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rak.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ayn.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://dfz.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ngh.fehbvm.com

[E14] URL 编码与 Base64
来源：http://bwx.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fqs.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://drf.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tke.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://igy.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nrh.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pkq.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://obz.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hil.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://muf.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zua.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vmz.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wun.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dit.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rhe.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhz.vehdjk.com


<!-- 参考信息 -->