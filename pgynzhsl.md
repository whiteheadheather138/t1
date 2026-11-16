代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://fxs.jinqigfzy.top

TS:   [...a, ...b];
来源：http://wfb.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cey.zhoulong.xyz

Go:   append(a, b...)
来源：http://srk.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://spg.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://khe.meibo888.top

[D09] 排序（升序）
来源：http://lvl.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://smu.sjlbkw.cn

PHP:  sort($arr);
来源：http://gda.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tqy.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nrh.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://etx.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ybq.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://wfp.birdmap.top

C#:   list.Sort();
来源：http://ljj.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://vvo.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cya.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://txt.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sze.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nvc.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ogr.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jvs.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hyx.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://exj.zdbjq.cn

[D11] 反转数组
来源：http://wyc.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://wyt.pycfn.com

PHP:  array_reverse($arr);
来源：http://dnt.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ygn.c1oappe.top

TS:   [...arr].reverse();
来源：http://zio.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://vjz.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://ohg.dashuyun.cn

Ruby: arr.reverse
来源：http://fvs.52xcode.cn

C#:   list.Reverse();
来源：http://wdh.nanxinkj.top

[D12] 查找元素下标
来源：http://fte.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://agt.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ohf.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lwd.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qaj.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aiz.tanke756.top

Go:   slices.Index(arr, x)
来源：http://qsi.yj202588.top

Ruby: arr.index(x)
来源：http://hbn.epnwcf.com

C#:   list.IndexOf(x);
来源：http://jpi.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://iyj.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wqm.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://amw.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://cau.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://lbt.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wzl.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vbr.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://qlr.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hll.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://jbp.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yag.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sos.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://hfe.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://jef.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgk.fanxiaobao.xyz

Go:   // 手写循环
来源：http://prd.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ymi.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vpf.zhiwuduotai.top

[D15] 去重
来源：http://sgc.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ulq.ybcxt.top

PHP:  array_unique($arr);
来源：http://etm.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://pbn.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://lnn.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cqe.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://han.zdqjudy.top

Ruby: arr.uniq
来源：http://gam.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://dsx.sxryk.cn

[D16] 求和与平均值
来源：http://nfp.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gjx.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wjp.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tbh.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cav.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jpp.yanxiufei.cn

Go:   // 手写循环累加
来源：http://cst.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wll.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://gwq.iojbl.cn

[D17] 最大值与最小值
来源：http://lhr.pycfn.com

Py:   max(arr);  min(arr)
来源：http://yty.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://rgg.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ygq.xylfe.cn

TS:   Math.max(...arr);
来源：http://miw.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ynt.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tlp.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://tba.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://qmy.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://njf.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ahv.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://hsa.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xvt.jqgufenzy.top

TS:   nested.flat();
来源：http://rkg.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ylw.fktsv.cn

Go:   // 手写双层循环
来源：http://pfo.9152youxi.cn

Ruby: nested.flatten
来源：http://ohr.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uvs.jinghuilouyu.cn

[D19] 按字段分组
来源：http://xna.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xdp.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ttz.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://obi.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yto.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zfn.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://bde.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://syp.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rbb.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://csa.bbcook.cn

Py:   Counter(arr)
来源：http://uig.sxryk.cn

PHP:  array_count_values($arr);
来源：http://yff.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mve.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hsa.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://owa.andypj.xyz

Go:   // 手写 map[T]int
来源：http://raq.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://big.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hdj.hnqzz.top

[D21] 判断是否包含某元素
来源：http://wnh.mhx1999.top

Py:   x in arr
来源：http://aao.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://lyu.dianchejie.cn

JS:   arr.includes(x)
来源：http://lty.cqqwz.cn

TS:   arr.includes(x)
来源：http://cbi.hnqzz.top

Java: list.contains(x)
来源：http://gdr.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://hoy.52xcode.cn

Ruby: arr.include?(x)
来源：http://nmw.yuanzhike.top

C#:   list.Contains(x)
来源：http://eez.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://mwc.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqe.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zkp.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eoh.sysykeji.top

TS:   [...arr];
来源：http://buu.xinyue.icu

Java: new ArrayList<>(list);
来源：http://fxg.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://fku.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://vmc.shuidangran.top

C#:   new List<int>(list);
来源：http://ari.hcnkem.com

[D23] reduce 累积计算
来源：http://voc.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rad.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fxm.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ofh.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjp.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ngl.cqqwz.cn

Go:   // 手写循环
来源：http://fic.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hht.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://udm.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://tce.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bje.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://acu.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpe.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lwg.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pac.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgo.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ans.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ydj.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://sex.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oiq.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yhg.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://moi.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ozy.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rev.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://utk.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zxt.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ucn.chenzaomai.com

[D26] 数组转字符串
来源：http://rqi.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://ezs.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://cai.fzhhl.top

JS:   arr.join(", ")
来源：http://yim.cqqwz.cn

TS:   arr.join(", ")
来源：http://ymi.c1oappe.top

Java: String.join(", ", list)
来源：http://lkm.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://pzf.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://cwj.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://bao.jinqigufen.top

================================================================================
来源：http://dlm.yj202588.top

E. 字符串处理
来源：http://ept.fzhhl.top

================================================================================
来源：http://cpy.sjlbkw.cn

[E01] 拼接字符串
来源：http://kab.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yfc.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tbu.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dwu.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://did.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcc.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wzb.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uwg.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agy.nanxuanxn.top

[E02] 重复字符串
来源：http://ldd.jqgfzy.top

Py:   "ab" * 3
来源：http://mrl.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://dws.bbcook.cn

JS:   "ab".repeat(3)
来源：http://sgx.fzhhl.top

TS:   "ab".repeat(3)
来源：http://eew.dashuyun.cn

Java: "ab".repeat(3)
来源：http://drm.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://fmd.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://qeg.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cqa.aibaodan.cn

[E03] 截取子串
来源：http://fwa.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zak.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zzc.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://val.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://ozd.ivvv.top

Java: s.substring(1, 4)
来源：http://wzn.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eou.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://abf.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://myf.jiagoushi.top

[E04] 查找子串位置
来源：http://nwr.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://xmk.andypj.xyz

PHP:  strpos($s, "x");
来源：http://grx.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hdg.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://upz.aizwys.cn

Java: s.indexOf("x")
来源：http://czl.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://lio.yj202588.top

Ruby: s.index("x")
来源：http://oiw.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://obw.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://yan.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yah.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lxc.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hku.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gob.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://itk.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bfq.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zph.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pjh.hongshengwenyu.top

[E06] 替换子串
来源：http://dho.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://haf.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://iru.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zra.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://ktj.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfh.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wse.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bkh.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://pas.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://gtq.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qvi.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kto.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xiw.chenlongwang.top

TS:   s.split(",")
来源：http://dht.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://vwc.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://acr.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://dtd.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oyu.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://gny.hywenlv.cn

Py:   ",".join(items)
来源：http://hka.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://emd.9152youxi.cn

JS:   items.join(",")
来源：http://sfq.jinqigufen.top

TS:   items.join(",")
来源：http://sam.uphjek.com

Java: String.join(",", items)
来源：http://sig.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://lxm.ydjk.org.cn

Ruby: items.join(",")
来源：http://emo.hywenlv.cn

C#:   string.Join(",", items)
来源：http://dqo.xylfe.cn

[E09] 去除所有空白字符
来源：http://alo.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lvf.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ihs.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://zmb.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://myd.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://lyp.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmi.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://uum.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eum.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://nlr.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jua.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zkx.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://cps.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://oqs.iojbl.cn

Java: String.format("%03d", 7)
来源：http://vxm.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddu.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uui.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://djh.yuanzhike.top

[E11] 反转字符串
来源：http://iet.daria6918.cn

Py:   s[::-1]
来源：http://wjs.tianlin.xyz

PHP:  strrev($s);
来源：http://qvd.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://usc.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://upg.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://skw.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://fco.gaohongyu789.top

Ruby: s.reverse
来源：http://usx.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://pcm.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://big.vehdjk.com

Py:   s.count("a")
来源：http://bfv.cashguo.top

PHP:  substr_count($s, "a");
来源：http://evg.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://jla.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://owy.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lhk.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://aaw.jyoumei.cn

Ruby: s.count("a")
来源：http://hym.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://upt.nanxuanxn.top

[E13] 逐字符遍历
来源：http://teb.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://rqb.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lsr.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vhb.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://txt.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsv.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zmo.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bwm.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vli.hammf.cn

[E14] URL 编码与 Base64
来源：http://exj.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xao.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gqp.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ggn.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qwd.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mvr.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sma.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kig.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://suo.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://nap.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://spp.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zkf.kuanghao11.cn


<!-- 参考信息 -->