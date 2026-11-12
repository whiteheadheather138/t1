代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://dvi.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://haj.ctjpmb.com

[D09] 排序（升序）
来源：http://daq.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://mwk.jqgfzy.top

PHP:  sort($arr);
来源：http://dmc.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rll.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://foy.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nbl.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjx.ppjwa.cn

Ruby: arr.sort
来源：http://dac.hywenlv.cn

C#:   list.Sort();
来源：http://xcj.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vqq.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ptj.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://clm.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://phf.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jjh.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dne.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wal.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cap.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yni.snrcjt.cn

[D11] 反转数组
来源：http://ypx.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://hji.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://nav.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bmd.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://eex.52xcode.cn

Java: Collections.reverse(list);
来源：http://zyj.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://lje.hammf.cn

Ruby: arr.reverse
来源：http://osk.fehbvm.com

C#:   list.Reverse();
来源：http://vhm.redwolf501.top

[D12] 查找元素下标
来源：http://dnl.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://mzn.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sow.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gch.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oxb.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fsa.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://nyb.kuanghao11.cn

Ruby: arr.index(x)
来源：http://hlw.ybcxt.top

C#:   list.IndexOf(x);
来源：http://lwc.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://dzl.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jnt.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nrn.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://ynb.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://gkj.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oav.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://syq.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://kyq.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ihh.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://dtg.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xmp.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tvw.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://fex.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://rrp.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nxy.ctjpmb.com

Go:   // 手写循环
来源：http://myp.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://qrh.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tha.wangdashe.top

[D15] 去重
来源：http://jcm.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ufe.jiagoushi.top

PHP:  array_unique($arr);
来源：http://wit.bjfxy.top

JS:   [...new Set(arr)]
来源：http://cgi.cucudq.cn

TS:   [...new Set(arr)]
来源：http://fmr.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wxb.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://owc.chenjidiqi.icu

Ruby: arr.uniq
来源：http://rfm.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://fdv.jianghu66.top

[D16] 求和与平均值
来源：http://grt.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://axt.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vni.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ivj.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ouf.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uhl.tianlin.xyz

Go:   // 手写循环累加
来源：http://mkj.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ckv.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://rjd.shzxlz.cn

[D17] 最大值与最小值
来源：http://pvg.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://acz.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://ajb.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tgz.cucudq.cn

TS:   Math.max(...arr);
来源：http://ggs.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yan.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://chq.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://mvy.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://fqk.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://cue.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://isl.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://bkm.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pwp.fzhhl.top

TS:   nested.flat();
来源：http://bwe.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zrr.cdnleiting.top

Go:   // 手写双层循环
来源：http://xzl.haohaochexian.top

Ruby: nested.flatten
来源：http://kjb.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vqb.shanyushiyangtech.top

[D19] 按字段分组
来源：http://vbt.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rqu.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://prk.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://euw.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kfz.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rjs.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://lqy.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://heh.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xfv.yonumen.top

[D20] 统计每个元素出现次数
来源：http://rxq.hcnkem.com

Py:   Counter(arr)
来源：http://xua.andypj.xyz

PHP:  array_count_values($arr);
来源：http://res.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oeb.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cmz.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://spl.316326.xyz

Go:   // 手写 map[T]int
来源：http://mtl.havefunace.top

Ruby: arr.tally
来源：http://oyb.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://esz.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://hzp.vehdjk.com

Py:   x in arr
来源：http://rjy.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://cge.chenzaomai.com

JS:   arr.includes(x)
来源：http://rfy.yj202588.top

TS:   arr.includes(x)
来源：http://gha.haohaochexian.top

Java: list.contains(x)
来源：http://zgv.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://mpl.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://zvx.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://ijq.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://vtu.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rbr.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pjm.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://emp.0kj1m.cn

TS:   [...arr];
来源：http://wdh.gzhubu.top

Java: new ArrayList<>(list);
来源：http://cxg.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pqc.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://yzv.jianghu66.top

C#:   new List<int>(list);
来源：http://cxj.nanxinkj.top

[D23] reduce 累积计算
来源：http://oux.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://umw.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://exd.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syl.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tsn.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tvh.gzhubu.top

Go:   // 手写循环
来源：http://tku.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wrd.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xku.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://zwm.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yfb.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://luw.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qkt.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://etp.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rgl.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ley.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://whl.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dee.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://kwv.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wep.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ndj.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pie.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://onq.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ayh.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nbu.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pho.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dnn.gzhubu.top

[D26] 数组转字符串
来源：http://csx.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://qvy.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://umq.zdqjudy.top

JS:   arr.join(", ")
来源：http://bxr.redwolf501.top

TS:   arr.join(", ")
来源：http://hfo.cdnleiting.top

Java: String.join(", ", list)
来源：http://lpr.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://axs.epnwcf.com

Ruby: arr.join(", ")
来源：http://yho.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://kvp.fehbvm.com

================================================================================
来源：http://hmu.shanyushiyangkeji.top

E. 字符串处理
来源：http://htm.shzxlz.cn

================================================================================
来源：http://dtp.ivvv.top

[E01] 拼接字符串
来源：http://msp.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mmg.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://frm.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zpc.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lzm.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aac.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ckh.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ots.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://trg.jinqigufen.top

[E02] 重复字符串
来源：http://vqa.yangfankeji.com

Py:   "ab" * 3
来源：http://oyk.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://sib.sweek.top

JS:   "ab".repeat(3)
来源：http://irc.fengsongda.top

TS:   "ab".repeat(3)
来源：http://ecf.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://vjw.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://xqe.wangdashe.top

Ruby: "ab" * 3
来源：http://ejd.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eie.shanyushiyangtech.top

[E03] 截取子串
来源：http://cbh.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://atj.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ujo.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yfd.shuidangran.top

TS:   s.slice(1, 4)
来源：http://zva.xylfe.cn

Java: s.substring(1, 4)
来源：http://wve.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rvf.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mle.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://lhr.daria6918.cn

[E04] 查找子串位置
来源：http://zys.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://wvo.iojbl.cn

PHP:  strpos($s, "x");
来源：http://boa.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://byq.zhixingplan.top

TS:   s.indexOf("x")
来源：http://jzz.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://gsa.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://hag.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://aze.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://hgd.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://umy.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uyq.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://psm.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qyw.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://aek.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://czn.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wfg.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wzq.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vih.zdqjudy.top

[E06] 替换子串
来源：http://nca.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fso.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://dmt.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mib.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://eyb.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hcu.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wab.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lyv.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://bfl.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://gpf.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://stc.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xhq.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qxj.zhoulong.xyz

TS:   s.split(",")
来源：http://pyc.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://bjq.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tie.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://fdb.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sdq.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://vgt.feifeiyinyue.top

Py:   ",".join(items)
来源：http://hsp.xylfe.cn

PHP:  implode(",", $items);
来源：http://wxk.shanyushiyangtech.top

JS:   items.join(",")
来源：http://clt.pycfn.com

TS:   items.join(",")
来源：http://lme.chenzaomai.com

Java: String.join(",", items)
来源：http://npo.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://ybp.yonumen.top

Ruby: items.join(",")
来源：http://hwb.jianghu66.top

C#:   string.Join(",", items)
来源：http://esc.cucudq.cn

[E09] 去除所有空白字符
来源：http://vli.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dfo.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uaa.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://djf.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://dfj.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://pzv.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uaw.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://zsw.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hkm.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://mgh.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://abd.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eag.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://igy.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://fqk.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://zun.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nqx.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xuy.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ulb.shanyushiyangtech.top

[E11] 反转字符串
来源：http://zjq.yj202588.top

Py:   s[::-1]
来源：http://zfr.zhengqikj.top

PHP:  strrev($s);
来源：http://moz.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://plp.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://amz.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jzy.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hci.zhixingplan.top

Ruby: s.reverse
来源：http://vok.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://gnx.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://uxg.yj20258888.top

Py:   s.count("a")
来源：http://gqf.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://wok.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://vjf.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://dmv.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jbv.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://jwq.fzhhl.top

Ruby: s.count("a")
来源：http://hon.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://feh.guowangkeji.top

[E13] 逐字符遍历
来源：http://jdh.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://eto.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ojn.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tqn.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://txy.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xvr.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uha.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://svo.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://exo.hammf.cn

[E14] URL 编码与 Base64
来源：http://ktf.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vfh.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://xrd.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://axh.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ydr.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://opi.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lzs.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bux.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://crl.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://bwx.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vcl.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kwb.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jrh.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ffb.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://age.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xeo.fehbvm.com


<!-- 参考信息 -->