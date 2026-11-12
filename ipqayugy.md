代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ugl.gzhubu.top

Ruby: arr.sort
来源：http://cdt.vehdjk.com

C#:   list.Sort();
来源：http://poy.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://krm.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yro.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bbu.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdy.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwv.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hnz.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ldk.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://azo.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cbo.guannengcc.top

[D11] 反转数组
来源：http://hph.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lbc.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://kkl.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://czp.gogol.net.cn

TS:   [...arr].reverse();
来源：http://mvb.havefunace.top

Java: Collections.reverse(list);
来源：http://mxo.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://kqc.zycfv.cn

Ruby: arr.reverse
来源：http://sph.yj202588.top

C#:   list.Reverse();
来源：http://fsi.shangyingyoupin.top

[D12] 查找元素下标
来源：http://uzq.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://mzv.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cim.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jiv.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxp.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njv.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://dac.fzhhl.top

Ruby: arr.index(x)
来源：http://lnt.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://sit.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://cmv.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xoe.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qeb.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://erh.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://ehh.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kfz.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kqk.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rmh.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rny.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://rag.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qni.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qda.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://fxf.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://fiv.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tpd.snrcjt.cn

Go:   // 手写循环
来源：http://anh.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://jzq.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gma.jqgfzy.top

[D15] 去重
来源：http://vac.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bli.snrcjt.cn

PHP:  array_unique($arr);
来源：http://yqy.fengsongda.top

JS:   [...new Set(arr)]
来源：http://jzk.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://lwx.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pzp.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://avr.tianlin.xyz

Ruby: arr.uniq
来源：http://aqv.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://aom.fengsongda.top

[D16] 求和与平均值
来源：http://vcu.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fml.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hmq.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jgb.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hie.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yin.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://qgi.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dnq.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://awe.redwolf501.top

[D17] 最大值与最小值
来源：http://jbx.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://fnq.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://kpl.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rtc.ppjwa.cn

TS:   Math.max(...arr);
来源：http://swx.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lgr.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mwx.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://tvi.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://vab.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://xaa.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rvw.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://mel.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cxw.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://bet.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://abl.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://tao.jqgfzy.top

Ruby: nested.flatten
来源：http://lpg.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://gqe.c1oappe.top

[D19] 按字段分组
来源：http://ynu.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wnt.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kuz.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nhk.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ohf.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dsk.yongpay.top

Go:   // 手写 map[string][]T
来源：http://ryw.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cqv.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rmh.havefunace.top

[D20] 统计每个元素出现次数
来源：http://sxp.feifeiyinyue.top

Py:   Counter(arr)
来源：http://mnn.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://kqe.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iow.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ptt.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nbt.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://lle.cucudq.cn

Ruby: arr.tally
来源：http://wfz.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://spv.fehbvm.com

[D21] 判断是否包含某元素
来源：http://thr.jinqigufen.top

Py:   x in arr
来源：http://dfw.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://pst.zhixingplan.top

JS:   arr.includes(x)
来源：http://nrz.bjfxy.top

TS:   arr.includes(x)
来源：http://hqo.nwbrower.top

Java: list.contains(x)
来源：http://lpw.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://xha.nanxinkj.top

Ruby: arr.include?(x)
来源：http://rdv.zhijiandao.cn

C#:   list.Contains(x)
来源：http://nib.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://pvj.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rba.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oby.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fje.yfazqb.com

TS:   [...arr];
来源：http://riq.c1oappe.top

Java: new ArrayList<>(list);
来源：http://qzq.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rvw.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://sbm.zhongyouzk.top

C#:   new List<int>(list);
来源：http://gcn.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://rms.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fmh.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ipl.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxi.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://plc.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hgb.fehbvm.com

Go:   // 手写循环
来源：http://hre.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tny.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jnf.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://ada.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nrg.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vmy.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpp.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://voq.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fzf.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rfd.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uzq.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eiu.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://smk.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jnu.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oqc.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xny.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cyq.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ria.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lwl.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bnb.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lmy.gogol.net.cn

[D26] 数组转字符串
来源：http://sxx.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://vls.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://mdb.hysaishi.cn

JS:   arr.join(", ")
来源：http://ykm.ppjwa.cn

TS:   arr.join(", ")
来源：http://itn.yuxming.cn

Java: String.join(", ", list)
来源：http://ayr.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://fnu.uphjek.com

Ruby: arr.join(", ")
来源：http://jqt.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://cgs.ydjk.org.cn

================================================================================
来源：http://hbz.fzhhl.top

E. 字符串处理
来源：http://rah.zhixingplan.top

================================================================================
来源：http://rue.ivvv.top

[E01] 拼接字符串
来源：http://ecm.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ylk.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tfn.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rwj.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vjb.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qhg.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nbp.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jxu.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cvu.yuxming.cn

[E02] 重复字符串
来源：http://orj.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://drx.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://tsx.bbcook.cn

JS:   "ab".repeat(3)
来源：http://vsf.fktsv.cn

TS:   "ab".repeat(3)
来源：http://hnx.uphjek.com

Java: "ab".repeat(3)
来源：http://vao.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://jig.nanxuanxn.top

Ruby: "ab" * 3
来源：http://luw.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rbi.birdmap.top

[E03] 截取子串
来源：http://iaf.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxl.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qap.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://veg.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://vnl.ctjpmb.com

Java: s.substring(1, 4)
来源：http://lgs.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fvm.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://urc.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://mqe.xinyue.icu

[E04] 查找子串位置
来源：http://cwb.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://omp.nwbrower.top

PHP:  strpos($s, "x");
来源：http://rkq.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amv.sufxvd.cn

TS:   s.indexOf("x")
来源：http://rgx.yongpay.top

Java: s.indexOf("x")
来源：http://lkc.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://pee.hesvh.cn

Ruby: s.index("x")
来源：http://hsi.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://dez.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qto.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xgw.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sja.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wbh.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://flr.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eby.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cae.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gcw.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ofv.yj20258888.top

[E06] 替换子串
来源：http://oin.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://duk.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://naf.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbc.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://xyf.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvt.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sxn.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fsv.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://epi.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://czl.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xyw.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sjl.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://usl.jyoumei.cn

TS:   s.split(",")
来源：http://flo.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zpo.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fzv.sweek.top

Ruby: s.split(",");  s.split
来源：http://rrn.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gqn.zycfv.cn

[E08] 数组按分隔符合并
来源：http://kgd.shzxlz.cn

Py:   ",".join(items)
来源：http://mmg.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://ynb.gotoacloud.top

JS:   items.join(",")
来源：http://aal.gaohongyu789.top

TS:   items.join(",")
来源：http://jyp.xuanzx.com

Java: String.join(",", items)
来源：http://nnb.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://jkr.zhijiandao.cn

Ruby: items.join(",")
来源：http://thc.guannengcc.top

C#:   string.Join(",", items)
来源：http://xzk.sufxvd.cn

[E09] 去除所有空白字符
来源：http://tut.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pds.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jnd.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://jlp.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://vkl.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://fwu.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bad.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://xoa.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nut.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://qzr.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wgs.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cny.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://wsr.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://ioz.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://roa.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ioy.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eni.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vhl.yj202588.top

[E11] 反转字符串
来源：http://pyg.fehbvm.com

Py:   s[::-1]
来源：http://qbj.sysykeji.top

PHP:  strrev($s);
来源：http://yml.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://agf.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://shz.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://nmt.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hiv.cheryme.top

Ruby: s.reverse
来源：http://pii.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://hql.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://hqj.zhoulong.xyz

Py:   s.count("a")
来源：http://ivs.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://qdi.shuidangran.top

JS:   s.split("a").length - 1
来源：http://eua.yongpay.top

TS:   s.split("a").length - 1
来源：http://wkk.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://evx.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://plt.ehwqpu.com

Ruby: s.count("a")
来源：http://nfy.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://hkj.jqgfzy.top

[E13] 逐字符遍历
来源：http://lsm.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://ktj.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zga.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://rtx.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tpg.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://srt.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jeq.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kaj.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bpj.yuxming.cn

[E14] URL 编码与 Base64
来源：http://gjg.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://msf.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kxo.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://acq.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vty.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mvx.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zkf.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfv.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pco.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://ubp.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dso.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mlw.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zxj.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ont.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://spb.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://syc.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://shr.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hki.fehbvm.com

[E16] 数字千分位
来源：http://nbp.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://daq.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://lcu.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://ncx.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://szl.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ccp.gzhubu.top


<!-- 参考信息 -->