代发 wailian999

[D07] 切片 / 取子数组
来源：http://dna.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://inn.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gub.uphjek.com

JS:   arr.slice(1, 4);
来源：http://erq.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://sls.ppjwa.cn

Java: list.subList(1, 4);
来源：http://wlr.iojbl.cn

Go:   arr[1:4]
来源：http://rue.316326.xyz

Ruby: arr[1, 3]
来源：http://sym.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://ecr.quarkkingdee.top

[D08] 合并两个数组
来源：http://axo.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://nuf.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://etm.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://ejj.meibo888.top

TS:   [...a, ...b];
来源：http://fpp.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cyo.jiagoushi.top

Go:   append(a, b...)
来源：http://xil.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ayz.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://khy.zhoulong.xyz

[D09] 排序（升序）
来源：http://qeg.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://uam.chenzaomai.com

PHP:  sort($arr);
来源：http://hyb.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wim.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gan.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ygq.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ips.ppjwa.cn

Ruby: arr.sort
来源：http://yru.jlsjyb.cn

C#:   list.Sort();
来源：http://zli.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pqz.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evm.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vuj.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mab.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ebi.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eta.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vxg.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qim.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dct.shanyushiyangtech.top

[D11] 反转数组
来源：http://pll.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://mnw.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://blh.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gxy.shzxlz.cn

TS:   [...arr].reverse();
来源：http://cgv.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://rbp.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://gji.guannengcc.top

Ruby: arr.reverse
来源：http://oip.yueranfly.top

C#:   list.Reverse();
来源：http://gxq.jlsjyb.cn

[D12] 查找元素下标
来源：http://oct.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://gby.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xlf.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cut.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ase.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wxn.yongpay.top

Go:   slices.Index(arr, x)
来源：http://vcu.cqqwz.cn

Ruby: arr.index(x)
来源：http://tlg.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://lrc.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://lvm.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kcw.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qjb.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://rlr.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://gxf.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ffa.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lcj.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://iog.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zhm.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://klz.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwh.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rgh.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://oti.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://lei.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zxc.iojbl.cn

Go:   // 手写循环
来源：http://qsc.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://rpp.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fml.0kj1m.cn

[D15] 去重
来源：http://gwv.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mvu.wangdashe.top

PHP:  array_unique($arr);
来源：http://myk.sxryk.cn

JS:   [...new Set(arr)]
来源：http://nwc.birdmap.top

TS:   [...new Set(arr)]
来源：http://nim.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://coy.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yoh.fehbvm.com

Ruby: arr.uniq
来源：http://jrh.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://zbp.chenjidiqi.icu

[D16] 求和与平均值
来源：http://kfy.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ujb.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uuf.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gei.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://quc.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dbc.sufxvd.cn

Go:   // 手写循环累加
来源：http://vfh.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ffj.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://mwp.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://svt.ivvv.top

Py:   max(arr);  min(arr)
来源：http://cua.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://rkm.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tld.redwolf501.top

TS:   Math.max(...arr);
来源：http://tld.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xyw.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqn.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://ags.316326.xyz

C#:   list.Max();  list.Min()
来源：http://wwz.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://lwb.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lcg.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://tzv.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://clk.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://gmf.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://brq.sxryk.cn

Go:   // 手写双层循环
来源：http://lvb.jianghu66.top

Ruby: nested.flatten
来源：http://wng.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dmm.52xcode.cn

[D19] 按字段分组
来源：http://cxi.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fnh.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gyo.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cyv.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://vwn.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xpy.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://znf.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ysw.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://opa.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://eis.sxryk.cn

Py:   Counter(arr)
来源：http://gvg.xylfe.cn

PHP:  array_count_values($arr);
来源：http://lvx.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mxo.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpq.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zqd.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://pmt.ydzc1.top

Ruby: arr.tally
来源：http://osh.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gyu.daxiang520.top

[D21] 判断是否包含某元素
来源：http://ija.pengpengdd.cyou

Py:   x in arr
来源：http://ezh.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://osm.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://kwd.xuanzx.com

TS:   arr.includes(x)
来源：http://eez.zdqjudy.top

Java: list.contains(x)
来源：http://gcs.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://kat.cdnleiting.top

Ruby: arr.include?(x)
来源：http://aqd.ydzc1.top

C#:   list.Contains(x)
来源：http://uyl.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://mpo.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pli.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lqc.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lrj.zhaomingkeji.xyz

TS:   [...arr];
来源：http://czt.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://xdi.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://knq.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://gjs.vqdsnc.cn

C#:   new List<int>(list);
来源：http://env.vehdjk.com

[D23] reduce 累积计算
来源：http://rxl.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blz.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bfj.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvl.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jrn.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://oep.dianchejie.cn

Go:   // 手写循环
来源：http://ial.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wad.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gtv.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://njm.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vpe.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ehz.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mwn.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wnk.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrs.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fum.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kew.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wim.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://ucz.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://teg.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lhr.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://use.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rfm.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rvf.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cfg.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qcq.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cyz.hysaishi.cn

[D26] 数组转字符串
来源：http://hcv.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://bti.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://suy.jianghu66.top

JS:   arr.join(", ")
来源：http://mgx.yfazqb.com

TS:   arr.join(", ")
来源：http://obh.guowangkeji.top

Java: String.join(", ", list)
来源：http://qrk.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://ahv.jiagoushi.top

Ruby: arr.join(", ")
来源：http://kao.jianghu66.top

C#:   string.Join(", ", list)
来源：http://lwc.jlsjyb.cn

================================================================================
来源：http://pjq.gogol.net.cn

E. 字符串处理
来源：http://jvd.fzhhl.top

================================================================================
来源：http://anq.guowangkeji.top

[E01] 拼接字符串
来源：http://miz.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zee.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cmt.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iqg.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qyh.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ccv.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vaw.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://npf.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sdk.tanke756.top

[E02] 重复字符串
来源：http://awk.chenjidiqi.icu

Py:   "ab" * 3
来源：http://stc.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://btk.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://ijj.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://fbc.zdbjq.cn

Java: "ab".repeat(3)
来源：http://rgb.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://grq.cucudq.cn

Ruby: "ab" * 3
来源：http://xry.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bwx.wangshuangyany.cn

[E03] 截取子串
来源：http://yut.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dwf.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dmx.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oiy.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://ihh.epnwcf.com

Java: s.substring(1, 4)
来源：http://jfm.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lle.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tqf.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://qfv.yvedp.cn

[E04] 查找子串位置
来源：http://axo.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://tim.52xcode.cn

PHP:  strpos($s, "x");
来源：http://xez.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nbm.hnqzz.top

TS:   s.indexOf("x")
来源：http://yfg.tianlin.xyz

Java: s.indexOf("x")
来源：http://vas.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://szz.haohaochexian.top

Ruby: s.index("x")
来源：http://xmc.cheryme.top

C#:   s.IndexOf("x")
来源：http://cqj.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://elf.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://syy.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ywl.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovx.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vbg.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wuk.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uya.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bfp.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ijb.daria6918.cn

[E06] 替换子串
来源：http://rkq.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ocy.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://zsy.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nfe.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://ukh.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://huw.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mvc.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tes.yongpay.top

C#:   s.Replace("a", "b")
来源：http://ivg.vehdjk.com

[E07] 按分隔符拆分
来源：http://ysu.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://efh.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vwv.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://epa.tanke756.top

TS:   s.split(",")
来源：http://qpk.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ybh.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyq.tanke756.top

Ruby: s.split(",");  s.split
来源：http://vow.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tsx.sxryk.cn

[E08] 数组按分隔符合并
来源：http://mbp.hammf.cn

Py:   ",".join(items)
来源：http://mag.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://dpz.fzhhl.top

JS:   items.join(",")
来源：http://lev.quarkkingdee.top

TS:   items.join(",")
来源：http://rja.52xcode.cn

Java: String.join(",", items)
来源：http://fng.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://oax.cucudq.cn

Ruby: items.join(",")
来源：http://php.9152youxi.cn

C#:   string.Join(",", items)
来源：http://qzp.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://ewu.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://beg.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zhi.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://nlf.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://vmu.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://wbb.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://itq.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://yrc.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sxk.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://xhy.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uzz.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bso.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://htw.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://niw.pycfn.com

Java: String.format("%03d", 7)
来源：http://xvy.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vyb.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ige.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hlz.daria6918.cn

[E11] 反转字符串
来源：http://ujs.xuetiantiany.cn

Py:   s[::-1]
来源：http://nyd.snrcjt.cn

PHP:  strrev($s);
来源：http://exw.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://rba.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://rjv.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hsr.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://dja.yj20258.top

Ruby: s.reverse
来源：http://dat.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mbr.xylfe.cn

[E12] 统计某字符出现次数
来源：http://ney.xylfe.cn

Py:   s.count("a")
来源：http://tui.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://kdl.sweek.top

JS:   s.split("a").length - 1
来源：http://ggj.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://kel.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vwr.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://gri.jqgfzy.top

Ruby: s.count("a")
来源：http://hwk.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://rqe.andypj.xyz

[E13] 逐字符遍历
来源：http://nlg.sweek.top

Py:   for ch in s: print(ch)
来源：http://cbv.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hzb.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uyt.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tqg.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vvg.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rbd.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mpg.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://umi.gogol.net.cn


<!-- 参考信息 -->