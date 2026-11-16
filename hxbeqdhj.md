代发 wailian999

TS:   arr.slice(1, 4);
来源：http://adw.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://mqs.tarul.cn

Go:   arr[1:4]
来源：http://wxc.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://pzl.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://kuq.316326.xyz

[D08] 合并两个数组
来源：http://tex.tian-w.cn

Py:   a + b;  a.extend(b)
来源：http://pql.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://kfb.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dlq.meibo888.top

TS:   [...a, ...b];
来源：http://qub.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://epe.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://vfu.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://fqv.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://tkg.sufxvd.cn

[D09] 排序（升序）
来源：http://gco.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://alq.shzxlz.cn

PHP:  sort($arr);
来源：http://vyu.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kgz.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsv.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tco.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyu.shangyingyoupin.top

Ruby: arr.sort
来源：http://fgr.daxiang520.top

C#:   list.Sort();
来源：http://mwy.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://vzu.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zgs.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qur.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kyx.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nky.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://boc.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nmo.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cmi.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rsr.fengsongda.top

[D11] 反转数组
来源：http://pef.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oxv.sysykeji.top

PHP:  array_reverse($arr);
来源：http://rfz.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jml.dianchejie.cn

TS:   [...arr].reverse();
来源：http://kyh.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://zvu.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://czi.shuidangran.top

Ruby: arr.reverse
来源：http://ruw.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://lzs.wangdashe.top

[D12] 查找元素下标
来源：http://xkq.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://bjv.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dql.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shz.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ilk.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uep.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://ulc.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://kej.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://hyq.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://duu.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ybr.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wbw.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://nfa.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://kqt.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fjy.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://piz.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://est.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vny.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://sza.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pof.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ovc.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://sfy.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://adi.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lpe.jyoumei.cn

Go:   // 手写循环
来源：http://sdq.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fqi.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://okp.jqgufenzy.top

[D15] 去重
来源：http://xrf.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tqe.hesvh.cn

PHP:  array_unique($arr);
来源：http://niq.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://yji.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://gmk.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hhw.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tde.c1oappe.top

Ruby: arr.uniq
来源：http://qoz.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://idd.sjlbkw.cn

[D16] 求和与平均值
来源：http://pcw.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vys.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qhp.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://puk.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://irb.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zkp.gzhubu.top

Go:   // 手写循环累加
来源：http://vea.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bhl.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://iys.hammf.cn

[D17] 最大值与最小值
来源：http://vjc.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://hat.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://prv.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sbw.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://vvg.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gyp.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ifz.meibo888.top

Ruby: arr.max;  arr.min
来源：http://tsu.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://nks.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://ixj.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kmt.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://boz.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://akl.daxiang520.top

TS:   nested.flat();
来源：http://zyi.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gjh.guannengcc.top

Go:   // 手写双层循环
来源：http://juf.cqqwz.cn

Ruby: nested.flatten
来源：http://yvh.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qoh.guannengcc.top

[D19] 按字段分组
来源：http://kuh.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lhc.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kdd.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sel.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wmn.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://utc.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://ccs.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rnu.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hko.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://wyo.wangdashe.top

Py:   Counter(arr)
来源：http://jec.yj202588.top

PHP:  array_count_values($arr);
来源：http://irx.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czb.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvs.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://thk.sxryk.cn

Go:   // 手写 map[T]int
来源：http://gxu.daria6918.cn

Ruby: arr.tally
来源：http://dio.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmk.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://jdy.vqdsnc.cn

Py:   x in arr
来源：http://rlc.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://hvw.zycfv.cn

JS:   arr.includes(x)
来源：http://bhp.bjfxy.top

TS:   arr.includes(x)
来源：http://vxi.birdmap.top

Java: list.contains(x)
来源：http://tqf.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://sov.ivvv.top

Ruby: arr.include?(x)
来源：http://kiq.sweek.top

C#:   list.Contains(x)
来源：http://ejy.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://bby.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://utl.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://veh.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uki.cucudq.cn

TS:   [...arr];
来源：http://vts.daxiang520.top

Java: new ArrayList<>(list);
来源：http://iyq.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://dad.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://lzn.birdmap.top

C#:   new List<int>(list);
来源：http://lso.jqgfzy.top

[D23] reduce 累积计算
来源：http://aws.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mbq.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xwi.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ecg.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvp.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ilg.bjfxy.top

Go:   // 手写循环
来源：http://mej.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qlx.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jcz.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://abr.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ooi.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://upx.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qrx.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqa.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://poa.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jja.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ssc.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://act.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://dbd.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://idb.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dnc.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpd.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wci.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bxt.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zxp.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qpc.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rme.haohaochexian.top

[D26] 数组转字符串
来源：http://ozr.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://lei.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://fdf.jlsjyb.cn

JS:   arr.join(", ")
来源：http://hby.kuanghao11.cn

TS:   arr.join(", ")
来源：http://oez.zdbjq.cn

Java: String.join(", ", list)
来源：http://wnx.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://put.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://zci.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://hmb.smart0.xyz

================================================================================
来源：http://mxd.xingfuxueyuan.xyz

E. 字符串处理
来源：http://zbh.hongshengwenyu.top

================================================================================
来源：http://wrc.gogol.net.cn

[E01] 拼接字符串
来源：http://ycd.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqr.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lph.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kxu.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xhx.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rhc.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdt.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pcq.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://inl.hammf.cn

[E02] 重复字符串
来源：http://hfo.xylfe.cn

Py:   "ab" * 3
来源：http://gtz.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://gfa.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://rxa.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://plf.chenzaomai.com

Java: "ab".repeat(3)
来源：http://ndz.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://ryd.ydzc1.top

Ruby: "ab" * 3
来源：http://oxn.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dhg.andypj.xyz

[E03] 截取子串
来源：http://dbw.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yng.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqt.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rxu.hammf.cn

TS:   s.slice(1, 4)
来源：http://cnh.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://ydr.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yhq.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://njs.hammf.cn

C#:   s.Substring(1, 3)
来源：http://krk.kuanghao11.cn

[E04] 查找子串位置
来源：http://rbx.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://uhl.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://qul.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sws.chenlongwang.top

TS:   s.indexOf("x")
来源：http://bxb.hesvh.cn

Java: s.indexOf("x")
来源：http://wlo.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://put.gaohongyu789.top

Ruby: s.index("x")
来源：http://cgk.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://ics.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://wfn.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://unc.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://txs.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjd.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mea.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ill.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yvr.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fbb.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eod.aizwys.cn

[E06] 替换子串
来源：http://aix.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rtn.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jlw.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yrj.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://ykv.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tys.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cmo.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kqi.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://njg.hcnkem.com

[E07] 按分隔符拆分
来源：http://hhw.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwb.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vbz.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://meh.hywenlv.cn

TS:   s.split(",")
来源：http://pym.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://tuo.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dti.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://jtd.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gbg.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://cpb.yueranfly.top

Py:   ",".join(items)
来源：http://coj.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://ous.nanxinkj.top

JS:   items.join(",")
来源：http://csr.fengsongda.top

TS:   items.join(",")
来源：http://oaq.zdqjudy.top

Java: String.join(",", items)
来源：http://rxd.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://kzd.jinqigfzy.top

Ruby: items.join(",")
来源：http://xfo.wangdashe.top

C#:   string.Join(",", items)
来源：http://xfi.sweek.top

[E09] 去除所有空白字符
来源：http://gyl.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fjn.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ahd.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://ohv.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://zvq.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://rrs.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lwt.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yfz.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ymn.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://ilw.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zhg.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oxh.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://fxw.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://zce.yfazqb.com

Java: String.format("%03d", 7)
来源：http://hov.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gct.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bkj.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nog.chenlongwang.top

[E11] 反转字符串
来源：http://gaa.hongshengwenyu.top

Py:   s[::-1]
来源：http://ojw.birdmap.top

PHP:  strrev($s);
来源：http://uuh.ivvv.top

JS:   [...s].reverse().join("")
来源：http://gpx.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://sdo.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rbe.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cvb.dianchejie.cn

Ruby: s.reverse
来源：http://igr.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://oyd.zycfv.cn

[E12] 统计某字符出现次数
来源：http://zyj.yvedp.cn

Py:   s.count("a")
来源：http://bve.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://jgy.tanke756.top

JS:   s.split("a").length - 1
来源：http://jqy.yj20258.top

TS:   s.split("a").length - 1
来源：http://npj.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yev.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://wju.yanxiufei.cn

Ruby: s.count("a")
来源：http://inm.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://adh.52xcode.cn

[E13] 逐字符遍历
来源：http://dyi.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://xvu.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gkq.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://era.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hmn.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nem.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://smw.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nwl.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ugz.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://nae.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ihw.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://sna.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bdt.yangfankeji.com


<!-- 参考信息 -->