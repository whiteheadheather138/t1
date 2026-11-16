代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://vbn.ehwqpu.com

[D08] 合并两个数组
来源：http://tgs.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://wib.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://vms.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zlh.ppjwa.cn

TS:   [...a, ...b];
来源：http://iyz.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fsq.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://qmu.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://xej.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://edk.bbcook.cn

[D09] 排序（升序）
来源：http://mpg.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://mpt.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://qdj.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dub.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ofo.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://brg.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mtq.hnqzz.top

Ruby: arr.sort
来源：http://gdn.shzxlz.cn

C#:   list.Sort();
来源：http://hcr.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://okc.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eba.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ppf.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zwm.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bjf.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sfs.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zok.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqg.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://spm.zhaomingkeji.xyz

[D11] 反转数组
来源：http://shu.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iso.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://gqa.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qlj.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://ocv.jqgfzy.top

Java: Collections.reverse(list);
来源：http://ilp.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://skl.nanxinkj.top

Ruby: arr.reverse
来源：http://pwt.uphjek.com

C#:   list.Reverse();
来源：http://ona.jlsjyb.cn

[D12] 查找元素下标
来源：http://itr.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://lcn.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwx.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ife.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gox.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hul.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://ncf.fehbvm.com

Ruby: arr.index(x)
来源：http://ufc.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://rdk.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://xfp.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tqj.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ubx.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://wmj.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://guc.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dgu.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xlv.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://ven.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ata.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://uew.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ekx.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oxo.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://cts.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://pju.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rsg.yonumen.top

Go:   // 手写循环
来源：http://gpy.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://wpv.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ubj.hnxiangtu.top

[D15] 去重
来源：http://bwt.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bqf.sxryk.cn

PHP:  array_unique($arr);
来源：http://qpi.fktsv.cn

JS:   [...new Set(arr)]
来源：http://veg.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://nve.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pls.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uvm.birdmap.top

Ruby: arr.uniq
来源：http://lun.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://osl.vqdsnc.cn

[D16] 求和与平均值
来源：http://opc.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iiq.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mlg.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kkv.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ass.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hea.cheryme.top

Go:   // 手写循环累加
来源：http://dco.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wgk.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://dsu.gaohongyu789.top

[D17] 最大值与最小值
来源：http://qrw.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://eyc.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://grg.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bei.birdmap.top

TS:   Math.max(...arr);
来源：http://swx.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zde.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mwo.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://nub.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://rqn.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://vhc.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ogl.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://ftq.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wtb.smart0.xyz

TS:   nested.flat();
来源：http://yfi.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvy.sjlbkw.cn

Go:   // 手写双层循环
来源：http://paf.kuanghao11.cn

Ruby: nested.flatten
来源：http://kdu.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ugi.hywenlv.cn

[D19] 按字段分组
来源：http://oxi.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tsx.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://weh.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dpo.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://int.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iij.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://aao.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mfg.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qkt.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://emo.zycfv.cn

Py:   Counter(arr)
来源：http://bgk.yj20258.top

PHP:  array_count_values($arr);
来源：http://tiw.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://odd.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://moj.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://run.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://wng.iojbl.cn

Ruby: arr.tally
来源：http://pru.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dal.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://qew.ywan-chungtsiang.top

Py:   x in arr
来源：http://jqm.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://xku.yvedp.cn

JS:   arr.includes(x)
来源：http://xqn.gotoacloud.top

TS:   arr.includes(x)
来源：http://kib.yj20258.top

Java: list.contains(x)
来源：http://rfn.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://egk.0kj1m.cn

Ruby: arr.include?(x)
来源：http://xka.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://qre.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://hul.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mii.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqu.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dlj.cashguo.top

TS:   [...arr];
来源：http://dml.yj202588.top

Java: new ArrayList<>(list);
来源：http://awc.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://pyl.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://qxz.wangdashe.top

C#:   new List<int>(list);
来源：http://qve.yuxming.cn

[D23] reduce 累积计算
来源：http://ixs.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kmm.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://whn.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjn.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pya.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pzp.hywenlv.cn

Go:   // 手写循环
来源：http://mgx.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://chv.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rxw.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://jnw.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kjo.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hax.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tsu.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rvu.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pkj.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://thm.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zgh.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uqk.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://zih.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pau.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xus.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tlx.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://akt.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txw.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://orw.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xdi.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uvv.ybcxt.top

[D26] 数组转字符串
来源：http://rus.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://ixp.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://icc.shuidangran.top

JS:   arr.join(", ")
来源：http://orr.yanxiufei.cn

TS:   arr.join(", ")
来源：http://kbj.hcnkem.com

Java: String.join(", ", list)
来源：http://eil.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://uek.xuanzx.com

Ruby: arr.join(", ")
来源：http://fcr.daria6918.cn

C#:   string.Join(", ", list)
来源：http://edl.ybcxt.top

================================================================================
来源：http://xvf.ydzc1.top

E. 字符串处理
来源：http://ppb.tianlin.xyz

================================================================================
来源：http://pvg.ydjk.org.cn

[E01] 拼接字符串
来源：http://ljb.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ptk.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yrl.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jla.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mfo.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://beg.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vcc.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vop.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dzx.nanxinkj.top

[E02] 重复字符串
来源：http://hlr.aibaodan.cn

Py:   "ab" * 3
来源：http://hnf.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://byb.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://nui.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://dsy.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://rde.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://iwq.aizwys.cn

Ruby: "ab" * 3
来源：http://rsr.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pbs.xuanzx.com

[E03] 截取子串
来源：http://vrg.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymw.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wik.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dmb.fengsongda.top

TS:   s.slice(1, 4)
来源：http://bil.yuanzhike.top

Java: s.substring(1, 4)
来源：http://lgl.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vuw.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://kdy.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://sha.guowangkeji.top

[E04] 查找子串位置
来源：http://rqw.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://atf.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://nku.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zzn.sysykeji.top

TS:   s.indexOf("x")
来源：http://tnr.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://xpg.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://fwg.pengpengdd.cyou

Ruby: s.index("x")
来源：http://mqo.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://ltq.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ytw.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ykx.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://euk.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pub.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tfu.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kuz.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cvh.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xpw.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://odo.tanke756.top

[E06] 替换子串
来源：http://gyw.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zxr.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://kss.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldr.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://wfp.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqu.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vxq.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wje.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://ruo.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://nil.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://erg.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hjq.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ito.chenlongwang.top

TS:   s.split(",")
来源：http://nen.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://zfn.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jgl.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://bxs.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://syq.xuanzx.com

[E08] 数组按分隔符合并
来源：http://cke.zhixingplan.top

Py:   ",".join(items)
来源：http://qfl.hywenlv.cn

PHP:  implode(",", $items);
来源：http://cjj.hammf.cn

JS:   items.join(",")
来源：http://nwb.chenzaomai.com

TS:   items.join(",")
来源：http://ivw.hcnkem.com

Java: String.join(",", items)
来源：http://lmd.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://hng.jinqigufen.top

Ruby: items.join(",")
来源：http://kek.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://wmy.nanxinkj.top

[E09] 去除所有空白字符
来源：http://tza.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nwf.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://opx.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://sax.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://qbc.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://glr.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://csd.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://dld.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ehx.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://agd.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://joy.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oca.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://wfa.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://qak.ivvv.top

Java: String.format("%03d", 7)
来源：http://uvl.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://twc.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xcz.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vxv.fanxiaobao.xyz

[E11] 反转字符串
来源：http://jwf.pengpengdd.cyou

Py:   s[::-1]
来源：http://jve.chenzaomai.com

PHP:  strrev($s);
来源：http://rph.ivvv.top

JS:   [...s].reverse().join("")
来源：http://djb.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://dya.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lgu.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://acu.gaohongyu789.top

Ruby: s.reverse
来源：http://tkj.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://cqa.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://gnn.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://xby.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://nuw.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://cle.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://zya.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oti.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://tiw.hnxiangtu.top

Ruby: s.count("a")
来源：http://uth.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://jud.haohaochexian.top

[E13] 逐字符遍历
来源：http://htw.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://sta.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zhm.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pbp.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ziv.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tiq.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qxc.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gkm.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pdl.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://ahn.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddt.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvt.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjp.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wcu.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://otr.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tjg.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vhi.jianghu66.top


<!-- 参考信息 -->