代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://dok.fzhhl.top

[D08] 合并两个数组
来源：http://uvy.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://qyd.316326.xyz

PHP:  array_merge($a, $b);
来源：http://sra.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lty.0kj1m.cn

TS:   [...a, ...b];
来源：http://kus.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qgz.pycfn.com

Go:   append(a, b...)
来源：http://smz.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://sqk.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://etl.ehwqpu.com

[D09] 排序（升序）
来源：http://tth.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://mrx.fzhhl.top

PHP:  sort($arr);
来源：http://kvx.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pgm.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rrm.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rwk.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://viq.quarkkingdee.top

Ruby: arr.sort
来源：http://grq.chenlongwang.top

C#:   list.Sort();
来源：http://bfk.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihf.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ppu.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bps.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://psy.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lzf.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdw.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zwo.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xmi.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svm.sweek.top

[D11] 反转数组
来源：http://vin.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://opa.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://jyy.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zpq.hysaishi.cn

TS:   [...arr].reverse();
来源：http://xut.fehbvm.com

Java: Collections.reverse(list);
来源：http://etg.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://pap.jqgfzy.top

Ruby: arr.reverse
来源：http://yew.shangyingyoupin.top

C#:   list.Reverse();
来源：http://ftg.pengpengdd.cyou

[D12] 查找元素下标
来源：http://fbm.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://qio.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vyy.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zii.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nmg.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cyj.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://udu.316326.xyz

Ruby: arr.index(x)
来源：http://tay.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://dkp.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://jmd.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kec.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fmw.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://kmn.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://enx.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pym.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xet.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ujm.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://bet.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://osd.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgn.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fls.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://qab.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://ozv.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oxi.yongpay.top

Go:   // 手写循环
来源：http://dzk.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://nll.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uzp.vehdjk.com

[D15] 去重
来源：http://lst.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yon.andypj.xyz

PHP:  array_unique($arr);
来源：http://hlk.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://pee.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://xot.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jpm.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://swq.xziqi.cn

Ruby: arr.uniq
来源：http://rpq.yj20258.top

C#:   list.Distinct().ToList()
来源：http://cxk.dianchejie.cn

[D16] 求和与平均值
来源：http://czw.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fzm.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://san.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bmd.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ouj.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jse.yvedp.cn

Go:   // 手写循环累加
来源：http://uck.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yos.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://hrb.bjfxy.top

[D17] 最大值与最小值
来源：http://jwj.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://qmq.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://kqo.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vqg.fehbvm.com

TS:   Math.max(...arr);
来源：http://wkg.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xck.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://soc.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://xxn.yj202588.top

C#:   list.Max();  list.Min()
来源：http://aiq.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://nhr.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xzz.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://jzt.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://voj.fengsongda.top

TS:   nested.flat();
来源：http://dxo.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qnh.dianchejie.cn

Go:   // 手写双层循环
来源：http://wmd.yongpay.top

Ruby: nested.flatten
来源：http://etg.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://tbd.daria6918.cn

[D19] 按字段分组
来源：http://yhs.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ypg.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ujd.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cwj.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gfk.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ajb.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://ahc.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://exi.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tsv.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://ktq.iojbl.cn

Py:   Counter(arr)
来源：http://uhj.hnqzz.top

PHP:  array_count_values($arr);
来源：http://imj.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ytv.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ana.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mua.tian-w.cn

Go:   // 手写 map[T]int
来源：http://bxa.9152youxi.cn

Ruby: arr.tally
来源：http://hui.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uyu.yuxming.cn

[D21] 判断是否包含某元素
来源：http://mwo.dashuyun.cn

Py:   x in arr
来源：http://avq.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://ilh.zycfv.cn

JS:   arr.includes(x)
来源：http://kkl.nwbrower.top

TS:   arr.includes(x)
来源：http://wqs.havefunace.top

Java: list.contains(x)
来源：http://kew.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://alo.aizwys.cn

Ruby: arr.include?(x)
来源：http://okt.gotoacloud.top

C#:   list.Contains(x)
来源：http://aot.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://fap.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bah.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rrp.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dfy.hcnkem.com

TS:   [...arr];
来源：http://dkr.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://tbs.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://dcs.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://sbr.yj202588.top

C#:   new List<int>(list);
来源：http://hvf.haohaochexian.top

[D23] reduce 累积计算
来源：http://nwm.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xdf.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baq.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nuz.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://flq.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ujw.hongshengwenyu.top

Go:   // 手写循环
来源：http://hfi.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wer.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vjz.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://nmk.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kib.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://png.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sbd.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://khu.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://usn.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mtm.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cpz.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gzn.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://jgd.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pct.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohh.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tkk.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ayc.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gtu.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://atk.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://euz.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://faw.tian-w.cn

[D26] 数组转字符串
来源：http://zam.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://dev.birdmap.top

PHP:  implode(", ", $arr);
来源：http://vsy.jinqigfzy.top

JS:   arr.join(", ")
来源：http://jnl.mhx1999.top

TS:   arr.join(", ")
来源：http://uqj.tarul.cn

Java: String.join(", ", list)
来源：http://pvt.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://ppq.bbcook.cn

Ruby: arr.join(", ")
来源：http://ypw.mhx1999.top

C#:   string.Join(", ", list)
来源：http://mrr.uphjek.com

================================================================================
来源：http://vje.jyoumei.cn

E. 字符串处理
来源：http://kkt.nanxinkj.top

================================================================================
来源：http://gfx.hfpthk.cn

[E01] 拼接字符串
来源：http://ayd.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pqb.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hho.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jps.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gif.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zwj.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kva.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gze.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdu.gotoacloud.top

[E02] 重复字符串
来源：http://ute.guowangkeji.top

Py:   "ab" * 3
来源：http://bji.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://dav.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://mfr.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://wly.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://jzv.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://rsl.fktsv.cn

Ruby: "ab" * 3
来源：http://cnl.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zne.hfpthk.cn

[E03] 截取子串
来源：http://cut.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bmj.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kxi.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vgo.sysykeji.top

TS:   s.slice(1, 4)
来源：http://ibk.52xcode.cn

Java: s.substring(1, 4)
来源：http://iog.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cnz.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pek.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://vql.aizwys.cn

[E04] 查找子串位置
来源：http://qat.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://oyb.guannengcc.top

PHP:  strpos($s, "x");
来源：http://aaw.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tuz.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://ubh.epnwcf.com

Java: s.indexOf("x")
来源：http://zbs.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://woz.xziqi.cn

Ruby: s.index("x")
来源：http://gom.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://elx.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://fcv.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shq.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dlk.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbf.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lca.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qjb.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gub.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://six.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://apk.jianghu66.top

[E06] 替换子串
来源：http://dzj.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mwr.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://gfs.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayc.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://ojv.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iou.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oap.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sel.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://var.ehwqpu.com

[E07] 按分隔符拆分
来源：http://dgx.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ykj.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wkr.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xef.gogol.net.cn

TS:   s.split(",")
来源：http://bpl.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://xcb.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wer.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://wox.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kwz.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://ljk.daxiang520.top

Py:   ",".join(items)
来源：http://adl.yonumen.top

PHP:  implode(",", $items);
来源：http://yln.tanke756.top

JS:   items.join(",")
来源：http://mko.cdnleiting.top

TS:   items.join(",")
来源：http://dns.hnxiangtu.top

Java: String.join(",", items)
来源：http://dxv.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://odj.tanke756.top

Ruby: items.join(",")
来源：http://rrg.daxiang520.top

C#:   string.Join(",", items)
来源：http://wvi.epnwcf.com

[E09] 去除所有空白字符
来源：http://eii.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bnq.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zjg.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://jyg.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://hgf.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://ugp.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ioa.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://psg.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgk.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://hyq.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ciz.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lwx.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://fvf.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://kov.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://hmb.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hfw.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iui.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wqy.haohaochexian.top

[E11] 反转字符串
来源：http://csc.52xcode.cn

Py:   s[::-1]
来源：http://fei.haohaochexian.top

PHP:  strrev($s);
来源：http://qnz.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://toe.meibo888.top

TS:   [...s].reverse().join("")
来源：http://lfs.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vgs.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hcf.yangfankeji.com

Ruby: s.reverse
来源：http://tih.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://gcy.smart0.xyz

[E12] 统计某字符出现次数
来源：http://ipa.guowangkeji.top

Py:   s.count("a")
来源：http://ywj.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://nsv.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://jkb.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://iaj.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsg.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://wno.hammf.cn

Ruby: s.count("a")
来源：http://lan.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://clc.hfpthk.cn

[E13] 逐字符遍历
来源：http://pyb.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://rqa.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://whg.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kxh.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://bsg.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mdu.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ixh.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yqy.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kfh.cashguo.top

[E14] URL 编码与 Base64
来源：http://dtd.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ams.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wlu.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://etb.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yhs.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bpp.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://chq.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wlo.tanke756.top


<!-- 参考信息 -->