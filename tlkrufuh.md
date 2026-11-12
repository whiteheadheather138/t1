代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://nhp.aizwys.cn

TS:   [...a, ...b];
来源：http://phd.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tsm.svipenyu.cn

Go:   append(a, b...)
来源：http://zoj.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://uzl.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://aqe.fengsongda.top

[D09] 排序（升序）
来源：http://kwb.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://dec.fzhhl.top

PHP:  sort($arr);
来源：http://tjd.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://thq.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ixk.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ezw.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mpl.gotoacloud.top

Ruby: arr.sort
来源：http://fie.yj20258.top

C#:   list.Sort();
来源：http://smx.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nfo.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hvz.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zis.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ein.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nue.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bsh.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://amd.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwj.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://htw.jinqigufen.top

[D11] 反转数组
来源：http://gtz.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nml.guannengcc.top

PHP:  array_reverse($arr);
来源：http://axr.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://guc.jqgfzy.top

TS:   [...arr].reverse();
来源：http://jvv.9152youxi.cn

Java: Collections.reverse(list);
来源：http://ala.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://wmu.jlsjyb.cn

Ruby: arr.reverse
来源：http://imn.xuetiantiany.cn

C#:   list.Reverse();
来源：http://juy.birdmap.top

[D12] 查找元素下标
来源：http://dkg.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://nfs.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://byi.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrx.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dyo.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qvh.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://egc.yanxiufei.cn

Ruby: arr.index(x)
来源：http://qlp.cheryme.top

C#:   list.IndexOf(x);
来源：http://tur.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://pwy.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://twu.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://smf.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://jvd.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://jci.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ukc.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mex.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://xzz.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ueb.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://ojr.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yzz.haohaochexian.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xcf.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://xuq.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://lpa.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qyt.epnwcf.com

Go:   // 手写循环
来源：http://qil.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://sqv.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jdc.chenjidiqi.icu

[D15] 去重
来源：http://pvn.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dtf.tian-w.cn

PHP:  array_unique($arr);
来源：http://kcb.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://yvz.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://tcf.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cxh.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://vlv.wangshuangyany.cn

Ruby: arr.uniq
来源：http://qwi.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://vim.fengsongda.top

[D16] 求和与平均值
来源：http://pya.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wul.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://orf.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bpm.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zwq.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ayg.c1oappe.top

Go:   // 手写循环累加
来源：http://jsm.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://anx.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://bdc.chenlongwang.top

[D17] 最大值与最小值
来源：http://ovn.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://msb.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://eyd.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mhb.cucudq.cn

TS:   Math.max(...arr);
来源：http://wbz.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aou.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sed.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://awi.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://ton.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://xez.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kry.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://grs.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ihv.aizwys.cn

TS:   nested.flat();
来源：http://pof.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wpj.zhongyouzk.top

Go:   // 手写双层循环
来源：http://uha.gotoacloud.top

Ruby: nested.flatten
来源：http://ctx.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sms.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://ggg.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mdr.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ywf.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tkc.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jfj.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://glb.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://liy.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gtl.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgv.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://cfy.gotoacloud.top

Py:   Counter(arr)
来源：http://tft.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://sls.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cuv.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooj.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aer.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://ucu.yj20258888.top

Ruby: arr.tally
来源：http://uxh.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jra.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://kxz.epnwcf.com

Py:   x in arr
来源：http://nbl.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://exk.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://rus.mhx1999.top

TS:   arr.includes(x)
来源：http://tub.bjfxy.top

Java: list.contains(x)
来源：http://sps.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://pgc.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://zep.c1oappe.top

C#:   list.Contains(x)
来源：http://ibr.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://dhp.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ewm.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jmg.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rnb.fehbvm.com

TS:   [...arr];
来源：http://cpi.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://cec.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qye.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://ilk.hammf.cn

C#:   new List<int>(list);
来源：http://fne.hysaishi.cn

[D23] reduce 累积计算
来源：http://luy.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nsi.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cex.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zhd.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iid.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fsa.quarkkingdee.top

Go:   // 手写循环
来源：http://aty.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jye.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pml.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://cor.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xol.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzr.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yrb.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xoi.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sqr.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sda.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jnj.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkh.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://bkk.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ybx.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://frt.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rpr.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bib.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cci.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gbm.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cuk.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pdv.0kj1m.cn

[D26] 数组转字符串
来源：http://bfn.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://yci.cashguo.top

PHP:  implode(", ", $arr);
来源：http://pbj.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://tjx.zdbjq.cn

TS:   arr.join(", ")
来源：http://gqp.uphjek.com

Java: String.join(", ", list)
来源：http://inv.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://sno.yj20258.top

Ruby: arr.join(", ")
来源：http://cke.bjfxy.top

C#:   string.Join(", ", list)
来源：http://doj.sxryk.cn

================================================================================
来源：http://vrd.xuanzx.com

E. 字符串处理
来源：http://fzp.shanyushiyangtech.top

================================================================================
来源：http://szs.ydjk.org.cn

[E01] 拼接字符串
来源：http://nuw.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tnf.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ukn.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://obo.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://llx.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oms.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xlk.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://puf.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ckf.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://xnc.fehbvm.com

Py:   "ab" * 3
来源：http://jjz.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://xbe.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://lkw.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://rua.ydzc1.top

Java: "ab".repeat(3)
来源：http://akt.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://kdr.mhx1999.top

Ruby: "ab" * 3
来源：http://yjy.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mvn.tian-w.cn

[E03] 截取子串
来源：http://dyj.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ptb.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jym.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lpj.havefunace.top

TS:   s.slice(1, 4)
来源：http://wua.sxryk.cn

Java: s.substring(1, 4)
来源：http://umx.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lrf.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://aqw.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://gtw.gaohongyu789.top

[E04] 查找子串位置
来源：http://znq.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://olb.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://nmo.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vof.9152youxi.cn

TS:   s.indexOf("x")
来源：http://occ.kuanghao11.cn

Java: s.indexOf("x")
来源：http://min.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://phz.quarkkingdee.top

Ruby: s.index("x")
来源：http://pxm.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://vso.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ceb.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://swl.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqk.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oks.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://uqt.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cfc.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kta.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ryk.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sax.chenjidiqi.icu

[E06] 替换子串
来源：http://fyt.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://enc.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://scm.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://otk.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://frg.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jhd.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uhc.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xky.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://nld.wangdashe.top

[E07] 按分隔符拆分
来源：http://mpr.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xrw.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jwt.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ups.hongshengwenyu.top

TS:   s.split(",")
来源：http://djj.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://axu.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ekz.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://lav.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ljj.yj20258.top

[E08] 数组按分隔符合并
来源：http://qrh.havefunace.top

Py:   ",".join(items)
来源：http://tht.shuidangran.top

PHP:  implode(",", $items);
来源：http://etr.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://lge.yanxiufei.cn

TS:   items.join(",")
来源：http://gjl.jqgfzy.top

Java: String.join(",", items)
来源：http://dgi.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://mnl.hysaishi.cn

Ruby: items.join(",")
来源：http://tcg.ppjwa.cn

C#:   string.Join(",", items)
来源：http://jhc.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://vmf.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mot.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ssl.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://qch.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://pvl.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://lkq.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lzc.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://uwp.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wrc.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://pux.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kzh.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://snw.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://fyf.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://ise.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://bsi.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zff.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dgh.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tmb.chenlongwang.top

[E11] 反转字符串
来源：http://tii.fehbvm.com

Py:   s[::-1]
来源：http://voc.jqgfzy.top

PHP:  strrev($s);
来源：http://nra.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://qul.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://mbq.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xic.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://hth.chenjidiqi.icu

Ruby: s.reverse
来源：http://abp.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://qdn.hnqzz.top

[E12] 统计某字符出现次数
来源：http://fyx.fehbvm.com

Py:   s.count("a")
来源：http://mhw.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://jgp.mhx1999.top

JS:   s.split("a").length - 1
来源：http://hbq.hammf.cn

TS:   s.split("a").length - 1
来源：http://cgq.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lns.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://nwb.hnxiangtu.top

Ruby: s.count("a")
来源：http://rxh.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://gdu.birdmap.top

[E13] 逐字符遍历
来源：http://vnp.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://bms.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oxq.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wjy.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://bzz.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fwb.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pji.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lao.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aeh.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://vkj.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qbj.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://swx.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjl.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyo.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tbn.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hji.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dam.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lcc.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://kac.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nnt.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jcy.vqdsnc.cn


<!-- 参考信息 -->