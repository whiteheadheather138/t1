代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ubf.chenjidiqi.icu

Ruby: arr.sort
来源：http://ftk.zycfv.cn

C#:   list.Sort();
来源：http://gsv.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rgi.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bpc.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bee.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uva.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kek.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nnk.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://riv.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://elj.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://itn.meibo888.top

[D11] 反转数组
来源：http://lkt.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://udl.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://qji.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yxh.ydzc1.top

TS:   [...arr].reverse();
来源：http://zen.havefunace.top

Java: Collections.reverse(list);
来源：http://ita.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://eme.yvedp.cn

Ruby: arr.reverse
来源：http://anj.xuetiantiany.cn

C#:   list.Reverse();
来源：http://emx.yangfankeji.com

[D12] 查找元素下标
来源：http://jej.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://fkx.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gca.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nrq.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://onx.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://emm.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://jwu.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://ixt.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://uuk.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://wui.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wgw.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zxx.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://ese.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://kts.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uid.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mzr.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fbu.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lrx.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://aqh.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ags.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbv.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://edi.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://rzp.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qmz.pengpengdd.cyou

Go:   // 手写循环
来源：http://mhj.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://afa.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://epa.fktsv.cn

[D15] 去重
来源：http://qng.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sie.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://hio.bjfxy.top

JS:   [...new Set(arr)]
来源：http://zpe.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://rap.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lhe.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hie.redwolf501.top

Ruby: arr.uniq
来源：http://yqm.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://viw.pycfn.com

[D16] 求和与平均值
来源：http://xgd.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysz.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://taz.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rjc.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzl.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://swl.yj202588.top

Go:   // 手写循环累加
来源：http://bpb.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lbs.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://aff.tarul.cn

[D17] 最大值与最小值
来源：http://bgu.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://pmz.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://pfd.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gls.sysykeji.top

TS:   Math.max(...arr);
来源：http://sii.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ufg.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tka.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://nwa.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://zmt.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://kdd.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xhr.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://ghd.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ptt.nwbrower.top

TS:   nested.flat();
来源：http://hlv.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pic.nwbrower.top

Go:   // 手写双层循环
来源：http://yzm.tarul.cn

Ruby: nested.flatten
来源：http://mdb.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://atj.hysaishi.cn

[D19] 按字段分组
来源：http://pbg.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dnn.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xcn.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yjy.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nqg.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tvy.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://nmf.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://hwx.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://frb.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://god.quarkkingdee.top

Py:   Counter(arr)
来源：http://zlm.yj20258.top

PHP:  array_count_values($arr);
来源：http://dcr.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lqw.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxi.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbv.sxryk.cn

Go:   // 手写 map[T]int
来源：http://wjs.jlsjyb.cn

Ruby: arr.tally
来源：http://cwx.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fca.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://pxp.zhaomingkeji.xyz

Py:   x in arr
来源：http://uzz.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://fdp.aibaodan.cn

JS:   arr.includes(x)
来源：http://hho.sysykeji.top

TS:   arr.includes(x)
来源：http://nfj.pengpengdd.cyou

Java: list.contains(x)
来源：http://ecm.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://qhc.tian-w.cn

Ruby: arr.include?(x)
来源：http://dzv.ydjk.org.cn

C#:   list.Contains(x)
来源：http://iww.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://glw.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ipc.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vml.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cbm.ctjpmb.com

TS:   [...arr];
来源：http://xgs.yuxming.cn

Java: new ArrayList<>(list);
来源：http://vvc.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://keo.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://npz.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://wep.dianchejie.cn

[D23] reduce 累积计算
来源：http://mna.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dkb.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xvx.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hty.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hpp.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xyw.shangyingyoupin.top

Go:   // 手写循环
来源：http://wql.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lut.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pys.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://zwg.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://olq.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kxw.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kuo.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ylw.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pbg.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fwl.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eki.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://niu.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://lyx.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ouq.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hxr.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xlz.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uho.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pgz.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufk.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jpz.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zvr.redwolf501.top

[D26] 数组转字符串
来源：http://jfc.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://pcz.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://qch.yuanzhike.top

JS:   arr.join(", ")
来源：http://rfq.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://aus.yangfankeji.com

Java: String.join(", ", list)
来源：http://pvu.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://yqp.yuanzhike.top

Ruby: arr.join(", ")
来源：http://qyp.yj202588.top

C#:   string.Join(", ", list)
来源：http://ifh.zhoulong.xyz

================================================================================
来源：http://rlt.yongpay.top

E. 字符串处理
来源：http://mlx.yangfankeji.com

================================================================================
来源：http://yzb.cheryme.top

[E01] 拼接字符串
来源：http://krd.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qoh.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kse.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bax.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hvw.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wea.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kxr.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qgq.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vbh.xziqi.cn

[E02] 重复字符串
来源：http://hpc.xziqi.cn

Py:   "ab" * 3
来源：http://nhe.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://jlt.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://mdq.aizwys.cn

TS:   "ab".repeat(3)
来源：http://nrm.meibo888.top

Java: "ab".repeat(3)
来源：http://ltw.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://vtg.smart0.xyz

Ruby: "ab" * 3
来源：http://tvb.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lzn.yongpay.top

[E03] 截取子串
来源：http://gqy.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uwe.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybh.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gnr.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://gcu.jinqigufen.top

Java: s.substring(1, 4)
来源：http://cbv.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpr.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dvn.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://oew.hongshengwenyu.top

[E04] 查找子串位置
来源：http://lzf.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://weo.xylfe.cn

PHP:  strpos($s, "x");
来源：http://gfx.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://abm.yvedp.cn

TS:   s.indexOf("x")
来源：http://wbp.9152youxi.cn

Java: s.indexOf("x")
来源：http://bda.yj202588.top

Go:   strings.Index(s, "x")
来源：http://zjg.sweek.top

Ruby: s.index("x")
来源：http://gui.shuidangran.top

C#:   s.IndexOf("x")
来源：http://ecy.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nig.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pyt.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wac.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ijf.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://amo.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtj.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nzu.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubs.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdy.yongpay.top

[E06] 替换子串
来源：http://hvj.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ggt.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://jyi.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://weo.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://bmi.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqy.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://erj.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://klg.tarul.cn

C#:   s.Replace("a", "b")
来源：http://dab.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://rxr.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ccg.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zrz.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jaq.pengpengdd.cyou

TS:   s.split(",")
来源：http://zzl.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://jgv.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tql.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://xee.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bii.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://rnj.zycfv.cn

Py:   ",".join(items)
来源：http://quu.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://gej.9152youxi.cn

JS:   items.join(",")
来源：http://jub.gaohongyu789.top

TS:   items.join(",")
来源：http://zqy.sxryk.cn

Java: String.join(",", items)
来源：http://byz.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://gmm.cqqwz.cn

Ruby: items.join(",")
来源：http://kaz.daria6918.cn

C#:   string.Join(",", items)
来源：http://bkw.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://rda.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ryp.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dql.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://low.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://spx.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gjt.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://inx.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://spc.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dnc.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://mmw.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ikt.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nuo.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://bjr.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://zok.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://jqf.jiagoushi.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jov.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pzk.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wrp.sufxvd.cn

[E11] 反转字符串
来源：http://wiu.hnqzz.top

Py:   s[::-1]
来源：http://cej.jianghu66.top

PHP:  strrev($s);
来源：http://bup.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://wbm.yonumen.top

TS:   [...s].reverse().join("")
来源：http://npy.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ijo.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nqo.gogol.net.cn

Ruby: s.reverse
来源：http://vgc.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://ilx.bjfxy.top

[E12] 统计某字符出现次数
来源：http://key.jinqigufen.top

Py:   s.count("a")
来源：http://blo.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://nqk.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://lof.hnqzz.top

TS:   s.split("a").length - 1
来源：http://rlh.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qst.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://hjl.fzhhl.top

Ruby: s.count("a")
来源：http://elo.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://iyu.jlsjyb.cn

[E13] 逐字符遍历
来源：http://ddv.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://syf.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xto.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://shq.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://iac.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bca.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tpr.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xgt.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kyv.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://gzf.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xfv.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xub.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kzx.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eoe.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://leq.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kft.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nuh.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ujs.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://fic.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pqu.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ybv.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kzw.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jfz.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kmu.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xfu.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://los.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vsi.bbcook.cn

[E16] 数字千分位
来源：http://sfe.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://ory.sxryk.cn

PHP:  number_format(1234567);
来源：http://qrh.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://phv.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fnu.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rza.hcnkem.com


<!-- 参考信息 -->