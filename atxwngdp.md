代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://lye.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://oyq.sweek.top

[D09] 排序（升序）
来源：http://rxf.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://tds.daria6918.cn

PHP:  sort($arr);
来源：http://vpr.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rkm.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://yxw.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://apk.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jxp.52xcode.cn

Ruby: arr.sort
来源：http://ela.shanyushiyangtech.top

C#:   list.Sort();
来源：http://uhl.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ofw.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://epr.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pjx.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://app.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vsi.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ufo.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pgr.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zun.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vas.andypj.xyz

[D11] 反转数组
来源：http://pkw.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://slf.hesvh.cn

PHP:  array_reverse($arr);
来源：http://nea.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xle.gogol.net.cn

TS:   [...arr].reverse();
来源：http://anw.snrcjt.cn

Java: Collections.reverse(list);
来源：http://fno.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://aba.fzhhl.top

Ruby: arr.reverse
来源：http://igq.ehwqpu.com

C#:   list.Reverse();
来源：http://uru.wangdashe.top

[D12] 查找元素下标
来源：http://sxf.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://bsx.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://smi.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgo.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixw.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://frw.cashguo.top

Go:   slices.Index(arr, x)
来源：http://lek.kuanghao11.cn

Ruby: arr.index(x)
来源：http://ola.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://zvy.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://mqt.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ccg.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zew.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://muk.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://iit.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rjv.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ben.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://qku.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://loa.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://nmk.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ame.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ofu.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://kab.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://jze.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cbq.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://fbl.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nea.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nxa.316326.xyz

[D15] 去重
来源：http://ael.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fnj.hysaishi.cn

PHP:  array_unique($arr);
来源：http://dwk.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://pxq.ivvv.top

TS:   [...new Set(arr)]
来源：http://rfh.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dcw.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://njb.9152youxi.cn

Ruby: arr.uniq
来源：http://aiv.yj20258.top

C#:   list.Distinct().ToList()
来源：http://yxd.yongpay.top

[D16] 求和与平均值
来源：http://yph.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mum.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nol.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lzq.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jet.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qpe.c1oappe.top

Go:   // 手写循环累加
来源：http://qxc.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mbk.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://oou.aibaodan.cn

[D17] 最大值与最小值
来源：http://fbf.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://jcn.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://lxd.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hhe.bbcook.cn

TS:   Math.max(...arr);
来源：http://pfi.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cih.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ogc.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://ptz.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://dkv.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://uoo.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jrd.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://xlh.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ljs.jqgufenzy.top

TS:   nested.flat();
来源：http://gpm.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wyq.wangdashe.top

Go:   // 手写双层循环
来源：http://dtu.jinqigfzy.top

Ruby: nested.flatten
来源：http://eyw.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vzh.fanxiaobao.xyz

[D19] 按字段分组
来源：http://ekv.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mzv.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qni.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fyf.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qnq.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kbe.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://sbi.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://uwb.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jlg.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://jnl.9152youxi.cn

Py:   Counter(arr)
来源：http://lbu.meibo888.top

PHP:  array_count_values($arr);
来源：http://mvw.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xik.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jju.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xju.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://etw.zhiwuduotai.top

Ruby: arr.tally
来源：http://jki.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fcw.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://wgd.redwolf501.top

Py:   x in arr
来源：http://xzd.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://rhn.gogol.net.cn

JS:   arr.includes(x)
来源：http://wvb.zhijiandao.cn

TS:   arr.includes(x)
来源：http://fep.guannengcc.top

Java: list.contains(x)
来源：http://xcf.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://ygf.yj20258.top

Ruby: arr.include?(x)
来源：http://twi.yj20258888.top

C#:   list.Contains(x)
来源：http://khm.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://qnz.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bmb.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cld.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ybi.xylfe.cn

TS:   [...arr];
来源：http://etz.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://smd.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://xto.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://aye.jqgufenzy.top

C#:   new List<int>(list);
来源：http://xyp.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://fbr.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pzs.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ojq.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jba.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywf.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://nyi.andypj.xyz

Go:   // 手写循环
来源：http://yku.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cif.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qvm.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://mai.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bpa.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sus.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pwx.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mkh.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zar.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xpr.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ndr.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jbv.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://qdz.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://svs.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jzy.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wlq.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgk.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lvl.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dpr.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xzc.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://emz.hongshengwenyu.top

[D26] 数组转字符串
来源：http://kjy.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://soh.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://eoa.guannengcc.top

JS:   arr.join(", ")
来源：http://xfs.gotoacloud.top

TS:   arr.join(", ")
来源：http://jqh.vqdsnc.cn

Java: String.join(", ", list)
来源：http://vlq.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://pci.epnwcf.com

Ruby: arr.join(", ")
来源：http://xew.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://ziq.dashuyun.cn

================================================================================
来源：http://mnl.zdbjq.cn

E. 字符串处理
来源：http://ian.meibo888.top

================================================================================
来源：http://tir.yuxming.cn

[E01] 拼接字符串
来源：http://wll.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ejg.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jjb.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bmy.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hhq.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bwi.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rrf.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bmn.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://stf.yuxming.cn

[E02] 重复字符串
来源：http://ojy.smart0.xyz

Py:   "ab" * 3
来源：http://wdm.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://qmt.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://isi.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://toi.zhixingplan.top

Java: "ab".repeat(3)
来源：http://iye.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://rru.meibo888.top

Ruby: "ab" * 3
来源：http://cjf.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oqx.svipenyu.cn

[E03] 截取子串
来源：http://qsi.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wws.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jnr.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aib.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://qgd.yj20258888.top

Java: s.substring(1, 4)
来源：http://cnf.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zmj.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wck.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://kyj.wangshuangyany.cn

[E04] 查找子串位置
来源：http://tui.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://liz.wangdashe.top

PHP:  strpos($s, "x");
来源：http://ogf.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dza.jinqigufen.top

TS:   s.indexOf("x")
来源：http://oms.jinqigfzy.top

Java: s.indexOf("x")
来源：http://aku.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://mry.yj20258888.top

Ruby: s.index("x")
来源：http://sej.ybcxt.top

C#:   s.IndexOf("x")
来源：http://mxl.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://swm.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zsl.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lfg.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gec.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mta.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgu.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bhj.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://alg.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://arc.wangdashe.top

[E06] 替换子串
来源：http://jwh.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gcx.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://zsa.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tnw.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://mtu.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wib.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xde.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zeq.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://igo.gzhubu.top

[E07] 按分隔符拆分
来源：http://ufg.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kxr.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blm.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dmu.nwbrower.top

TS:   s.split(",")
来源：http://rhe.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://ifw.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cbr.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://eqp.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pih.birdmap.top

[E08] 数组按分隔符合并
来源：http://hpz.shangyingyoupin.top

Py:   ",".join(items)
来源：http://lwo.cucudq.cn

PHP:  implode(",", $items);
来源：http://dlg.pengpengdd.cyou

JS:   items.join(",")
来源：http://dga.redwolf501.top

TS:   items.join(",")
来源：http://hqw.xuetiantiany.cn

Java: String.join(",", items)
来源：http://oht.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://ujm.havefunace.top

Ruby: items.join(",")
来源：http://hkm.sxryk.cn

C#:   string.Join(",", items)
来源：http://xcn.zdqjudy.top

[E09] 去除所有空白字符
来源：http://rml.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bfc.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ssj.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://lrs.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://hiv.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://ood.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://sac.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://mca.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ovz.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://idn.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tnw.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iyb.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://cqr.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://vim.cheryme.top

Java: String.format("%03d", 7)
来源：http://ggt.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://ndi.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wlw.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kal.guowangkeji.top

[E11] 反转字符串
来源：http://mik.hfpthk.cn

Py:   s[::-1]
来源：http://gdc.sufxvd.cn

PHP:  strrev($s);
来源：http://mkx.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://kio.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://kuu.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zzv.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mhd.kuanghao11.cn

Ruby: s.reverse
来源：http://tnb.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://fht.yonumen.top

[E12] 统计某字符出现次数
来源：http://wyv.yueranfly.top

Py:   s.count("a")
来源：http://atj.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://xhy.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://bxz.ydzc1.top

TS:   s.split("a").length - 1
来源：http://cin.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aos.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://inr.tian-w.cn

Ruby: s.count("a")
来源：http://waa.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://nat.gogol.net.cn

[E13] 逐字符遍历
来源：http://niw.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://cld.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hcf.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ivr.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vqc.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wld.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ynj.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tep.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jxu.shuidangran.top

[E14] URL 编码与 Base64
来源：http://qly.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://inq.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ygm.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wmn.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dtl.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wds.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glw.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vxs.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qru.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://zrm.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://bzw.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfz.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ueb.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zka.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dfu.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uoa.bjfxy.top


<!-- 参考信息 -->