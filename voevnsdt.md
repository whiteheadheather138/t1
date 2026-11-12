代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zrw.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sxy.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wmt.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjg.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://snw.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wqk.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mef.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dmq.shuidangran.top

[D11] 反转数组
来源：http://hyx.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xly.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://wvs.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qjb.yuanzhike.top

TS:   [...arr].reverse();
来源：http://aha.andypj.xyz

Java: Collections.reverse(list);
来源：http://ojo.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://czl.hysaishi.cn

Ruby: arr.reverse
来源：http://toq.bbcook.cn

C#:   list.Reverse();
来源：http://vwh.yj20258888.top

[D12] 查找元素下标
来源：http://prj.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://aot.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mbx.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpx.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mlt.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xaa.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://nps.svipenyu.cn

Ruby: arr.index(x)
来源：http://ueh.hcnkem.com

C#:   list.IndexOf(x);
来源：http://dae.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://pit.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://scb.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hqu.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://ppq.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://tkz.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mkw.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cqw.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xfi.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://fhj.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://wlw.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ght.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://axk.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://vmn.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://vsr.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lfr.cqqwz.cn

Go:   // 手写循环
来源：http://mhm.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://ssy.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ugn.ybcxt.top

[D15] 去重
来源：http://iip.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zsr.zhixingplan.top

PHP:  array_unique($arr);
来源：http://mfq.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://ghh.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://ktz.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxf.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://smf.jlsjyb.cn

Ruby: arr.uniq
来源：http://vbo.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://eao.nanxuanxn.top

[D16] 求和与平均值
来源：http://dcj.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://urq.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aav.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oak.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmp.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jss.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://lky.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://luy.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://sgp.0kj1m.cn

[D17] 最大值与最小值
来源：http://qrf.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://mmp.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://yww.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://umd.yj20258.top

TS:   Math.max(...arr);
来源：http://ezt.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fpm.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fls.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://lbs.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://ygf.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://lsf.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ypg.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://nra.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wth.yj20258888.top

TS:   nested.flat();
来源：http://wta.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uez.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://brb.zdbjq.cn

Ruby: nested.flatten
来源：http://yku.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fzi.tianlin.xyz

[D19] 按字段分组
来源：http://tco.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsd.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://viw.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hdz.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pwk.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ies.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://dye.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qjs.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kcx.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://zta.zhengqikj.top

Py:   Counter(arr)
来源：http://saj.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://hhh.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyw.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xkp.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dcg.xziqi.cn

Go:   // 手写 map[T]int
来源：http://bfa.nanxuanxn.top

Ruby: arr.tally
来源：http://gor.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vpx.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://iyk.hywenlv.cn

Py:   x in arr
来源：http://pqf.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://svs.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://ebi.havefunace.top

TS:   arr.includes(x)
来源：http://xxv.gaohongyu789.top

Java: list.contains(x)
来源：http://jzg.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://swp.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://jbv.hfpthk.cn

C#:   list.Contains(x)
来源：http://cgm.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://hps.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yoh.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://imc.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gbw.ivvv.top

TS:   [...arr];
来源：http://avy.yvedp.cn

Java: new ArrayList<>(list);
来源：http://iai.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://xlo.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://nxl.yangfankeji.com

C#:   new List<int>(list);
来源：http://dju.yuanzhike.top

[D23] reduce 累积计算
来源：http://nfu.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://loy.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cfh.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ler.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ebj.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgj.jqgfzy.top

Go:   // 手写循环
来源：http://qhv.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qrq.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xuz.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://xdb.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://air.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eiw.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mrh.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://swy.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://txa.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vbg.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oep.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://map.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://rfr.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tej.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ihe.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qob.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jrf.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wqq.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bry.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zpl.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jux.dashuyun.cn

[D26] 数组转字符串
来源：http://ife.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://zis.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://ybl.zhixingplan.top

JS:   arr.join(", ")
来源：http://xrx.jyoumei.cn

TS:   arr.join(", ")
来源：http://gvi.cqqwz.cn

Java: String.join(", ", list)
来源：http://soq.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://pta.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://hrz.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://ryf.hnxiangtu.top

================================================================================
来源：http://ieb.hnxiangtu.top

E. 字符串处理
来源：http://vud.wangshuangyany.cn

================================================================================
来源：http://gml.316326.xyz

[E01] 拼接字符串
来源：http://dvt.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jkj.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sxi.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xff.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bek.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ilc.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvm.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://viw.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pkl.gogol.net.cn

[E02] 重复字符串
来源：http://vhp.ydzc1.top

Py:   "ab" * 3
来源：http://uvq.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://zqc.sxryk.cn

JS:   "ab".repeat(3)
来源：http://fau.fehbvm.com

TS:   "ab".repeat(3)
来源：http://hzs.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://vjb.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://mfr.sysykeji.top

Ruby: "ab" * 3
来源：http://pgl.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ftd.vqdsnc.cn

[E03] 截取子串
来源：http://lwx.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xaw.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpf.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://shd.shuidangran.top

TS:   s.slice(1, 4)
来源：http://svv.sxryk.cn

Java: s.substring(1, 4)
来源：http://vkm.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xci.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cdi.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://fdo.ivvv.top

[E04] 查找子串位置
来源：http://vih.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://miu.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://hus.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vtm.9152youxi.cn

TS:   s.indexOf("x")
来源：http://pec.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://qiq.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://nwj.feifeiyinyue.top

Ruby: s.index("x")
来源：http://yoq.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://pnh.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://lgv.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://llz.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://imp.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swt.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://asd.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vve.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iml.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kjp.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yqe.ivvv.top

[E06] 替换子串
来源：http://jlx.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nfk.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://wxu.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wac.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://ofs.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qnr.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cbn.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ffm.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://hnd.sufxvd.cn

[E07] 按分隔符拆分
来源：http://rpo.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ira.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jiz.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xeh.gzhubu.top

TS:   s.split(",")
来源：http://kvc.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://kvb.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qju.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://lsq.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yja.sweek.top

[E08] 数组按分隔符合并
来源：http://ynm.zhijiandao.cn

Py:   ",".join(items)
来源：http://cwi.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://uyh.feifeiyinyue.top

JS:   items.join(",")
来源：http://qvf.iojbl.cn

TS:   items.join(",")
来源：http://ukm.daxiang520.top

Java: String.join(",", items)
来源：http://vmp.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://crp.kuanghao11.cn

Ruby: items.join(",")
来源：http://ctj.andypj.xyz

C#:   string.Join(",", items)
来源：http://gif.xziqi.cn

[E09] 去除所有空白字符
来源：http://jjk.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qvm.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pnf.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://krz.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://pdr.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://pli.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://vqg.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://oxa.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wwj.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://xyz.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fdf.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nbe.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://bek.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://gou.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://pgg.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://czi.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://epb.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zgs.jinqigufen.top

[E11] 反转字符串
来源：http://znz.jqgufenzy.top

Py:   s[::-1]
来源：http://dny.c1oappe.top

PHP:  strrev($s);
来源：http://evf.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://ztm.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://mzy.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://spp.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bmq.tanke756.top

Ruby: s.reverse
来源：http://fis.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://aar.52xcode.cn

[E12] 统计某字符出现次数
来源：http://miy.jyoumei.cn

Py:   s.count("a")
来源：http://nmj.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://hfy.daria6918.cn

JS:   s.split("a").length - 1
来源：http://xrb.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://lto.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fnq.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://mve.cashguo.top

Ruby: s.count("a")
来源：http://dbh.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://uut.cdnleiting.top

[E13] 逐字符遍历
来源：http://nus.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://rox.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wsa.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://csf.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tcq.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yvv.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zfa.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kis.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://avc.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://ttb.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wte.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gjr.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpy.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ehl.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://afr.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://atu.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://veb.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ddo.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://roi.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://god.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://htj.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nlu.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fbn.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aem.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ktb.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwb.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gbk.wangdashe.top

[E16] 数字千分位
来源：http://zod.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://adm.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://hyj.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lzr.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://wjj.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://brk.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://osw.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oih.sweek.top

C#:   1234567.ToString("N0")
来源：http://jvt.ybcxt.top

[E17] 首字母大写
来源：http://esy.xuetiantiany.cn


<!-- 参考信息 -->