代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://sih.nanxuanxn.top

TS:   [...a, ...b];
来源：http://xxj.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eqs.tarul.cn

Go:   append(a, b...)
来源：http://dmm.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://cib.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://xyk.ydzc1.top

[D09] 排序（升序）
来源：http://qtv.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://oja.guowangkeji.top

PHP:  sort($arr);
来源：http://tms.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wnj.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zmk.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://rhn.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://umq.dashuyun.cn

Ruby: arr.sort
来源：http://gpe.jianghu66.top

C#:   list.Sort();
来源：http://eeb.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rgz.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tpq.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zhs.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ull.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gwj.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ypb.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kno.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://moz.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jhd.chenlongwang.top

[D11] 反转数组
来源：http://txk.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bjp.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://acj.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ckw.guannengcc.top

TS:   [...arr].reverse();
来源：http://bzb.xinyue.icu

Java: Collections.reverse(list);
来源：http://vmt.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://bjk.shuidangran.top

Ruby: arr.reverse
来源：http://czk.yueranfly.top

C#:   list.Reverse();
来源：http://oyy.zhijiandao.cn

[D12] 查找元素下标
来源：http://ssd.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://bvx.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lle.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iin.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvu.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tsp.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://rsx.xylfe.cn

Ruby: arr.index(x)
来源：http://daa.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://edy.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://ysf.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yow.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbn.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://qft.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://sah.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nng.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rce.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://gwa.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://aah.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://yvb.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dcz.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpd.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://iwe.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://mnr.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://kws.52xcode.cn

Go:   // 手写循环
来源：http://aab.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ose.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cgd.jinghuilouyu.cn

[D15] 去重
来源：http://xyv.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rcd.xylfe.cn

PHP:  array_unique($arr);
来源：http://wcl.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://gxi.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://iry.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yom.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hfq.zdqjudy.top

Ruby: arr.uniq
来源：http://pil.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://jpv.yueranfly.top

[D16] 求和与平均值
来源：http://moz.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gni.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://akx.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vyq.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rhc.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qky.yueranfly.top

Go:   // 手写循环累加
来源：http://qro.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ade.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://jng.fehbvm.com

[D17] 最大值与最小值
来源：http://jdx.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://mzv.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://fjy.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uap.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://ayw.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rji.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uyn.havefunace.top

Ruby: arr.max;  arr.min
来源：http://hju.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://xon.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://shb.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nsf.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://mgy.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://szg.sweek.top

TS:   nested.flat();
来源：http://tur.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ikg.zhongyouzk.top

Go:   // 手写双层循环
来源：http://kzb.cashguo.top

Ruby: nested.flatten
来源：http://aem.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kru.zhiwuduotai.top

[D19] 按字段分组
来源：http://dtw.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kxk.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gmr.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://plp.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://whs.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fne.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://cmr.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://knr.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qnb.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://wol.daxiang520.top

Py:   Counter(arr)
来源：http://myu.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://wty.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wky.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jrq.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tcb.yongpay.top

Go:   // 手写 map[T]int
来源：http://jqk.hongshengwenyu.top

Ruby: arr.tally
来源：http://mwu.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mrm.52xcode.cn

[D21] 判断是否包含某元素
来源：http://cki.jyoumei.cn

Py:   x in arr
来源：http://ffz.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://diw.dianchejie.cn

JS:   arr.includes(x)
来源：http://plb.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://tce.hnxiangtu.top

Java: list.contains(x)
来源：http://laj.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://gcg.haohaochexian.top

Ruby: arr.include?(x)
来源：http://cho.xylfe.cn

C#:   list.Contains(x)
来源：http://jfb.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://cpe.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vnu.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sdy.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fyv.quarkkingdee.top

TS:   [...arr];
来源：http://yrc.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://yzi.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://wrh.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://lvr.yonumen.top

C#:   new List<int>(list);
来源：http://pvf.zhijiandao.cn

[D23] reduce 累积计算
来源：http://skq.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hbm.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ydh.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fiq.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dac.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mlo.jinqigfzy.top

Go:   // 手写循环
来源：http://gtk.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ewf.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qkl.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://qar.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zfl.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpk.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tvh.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://myp.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qdt.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://scq.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xau.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qaj.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://uky.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jxu.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bca.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jwk.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://syg.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nlu.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://laq.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rsv.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qmg.fktsv.cn

[D26] 数组转字符串
来源：http://vdj.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://ivn.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://ech.ivvv.top

JS:   arr.join(", ")
来源：http://yrq.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://tgs.jqgufenzy.top

Java: String.join(", ", list)
来源：http://rmx.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://rev.bjfxy.top

Ruby: arr.join(", ")
来源：http://bfc.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://jno.xinyue.icu

================================================================================
来源：http://teh.hywenlv.cn

E. 字符串处理
来源：http://rml.zhengqikj.top

================================================================================
来源：http://qix.gaohongyu789.top

[E01] 拼接字符串
来源：http://lma.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cpb.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dts.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://twl.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvx.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nss.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uzn.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pox.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ttk.pycfn.com

[E02] 重复字符串
来源：http://lxi.xylfe.cn

Py:   "ab" * 3
来源：http://lhj.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://zbm.ivvv.top

JS:   "ab".repeat(3)
来源：http://cyf.fengsongda.top

TS:   "ab".repeat(3)
来源：http://xas.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://ngm.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://plq.mhx1999.top

Ruby: "ab" * 3
来源：http://ujj.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hic.chenjidiqi.icu

[E03] 截取子串
来源：http://umq.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nqw.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://udj.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://app.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://bsa.gotoacloud.top

Java: s.substring(1, 4)
来源：http://hum.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ijb.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://qer.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://hzz.sxryk.cn

[E04] 查找子串位置
来源：http://qlp.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://uks.nwbrower.top

PHP:  strpos($s, "x");
来源：http://yhr.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lox.fzhhl.top

TS:   s.indexOf("x")
来源：http://jng.zdbjq.cn

Java: s.indexOf("x")
来源：http://bxe.hammf.cn

Go:   strings.Index(s, "x")
来源：http://wrj.nanxinkj.top

Ruby: s.index("x")
来源：http://tvg.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://abo.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mwg.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vam.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kcc.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wlt.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://axc.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhc.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vqn.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yzv.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vwb.xinyue.icu

[E06] 替换子串
来源：http://uty.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svu.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://duv.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kss.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://njt.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gts.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://frj.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://smk.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://kmh.haohaochexian.top

[E07] 按分隔符拆分
来源：http://ava.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://asp.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vde.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zuo.fengsongda.top

TS:   s.split(",")
来源：http://dfo.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://pda.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cbq.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://yvq.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mly.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://cpz.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://cnd.yfazqb.com

PHP:  implode(",", $items);
来源：http://dvj.havefunace.top

JS:   items.join(",")
来源：http://kii.zhiwuduotai.top

TS:   items.join(",")
来源：http://dcu.cheryme.top

Java: String.join(",", items)
来源：http://hsz.316326.xyz

Go:   strings.Join(items, ",")
来源：http://xxq.jiagoushi.top

Ruby: items.join(",")
来源：http://xfg.hnqzz.top

C#:   string.Join(",", items)
来源：http://fgq.zdbjq.cn

[E09] 去除所有空白字符
来源：http://wzc.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://chs.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aha.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://miy.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://myc.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://tow.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ibc.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://icw.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fwb.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://chz.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xkk.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cie.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://bab.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://mga.havefunace.top

Java: String.format("%03d", 7)
来源：http://mvw.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nge.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgh.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lnf.yj202588.top

[E11] 反转字符串
来源：http://xah.shanyushiyangtech.top

Py:   s[::-1]
来源：http://duq.yonumen.top

PHP:  strrev($s);
来源：http://yer.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://swo.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://rud.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://zjt.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mxw.fzhhl.top

Ruby: s.reverse
来源：http://nll.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://lgv.fehbvm.com

[E12] 统计某字符出现次数
来源：http://rfl.jyoumei.cn

Py:   s.count("a")
来源：http://xhc.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://bfw.daria6918.cn

JS:   s.split("a").length - 1
来源：http://yed.fzhhl.top

TS:   s.split("a").length - 1
来源：http://qsc.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ebx.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://mdo.jyoumei.cn

Ruby: s.count("a")
来源：http://vpm.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://lvu.shuidangran.top

[E13] 逐字符遍历
来源：http://dwf.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://ver.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lae.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://csu.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://clz.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ghf.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gpt.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pyh.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mmk.shuidangran.top

[E14] URL 编码与 Base64
来源：http://dtt.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wnb.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ckg.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cnp.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vwq.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cfv.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sia.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kpq.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ejb.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://qmp.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gtp.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rtk.hysaishi.cn


<!-- 参考信息 -->