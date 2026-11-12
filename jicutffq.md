代发 wailian999

PHP:  sort($arr);
来源：http://xpk.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ngz.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://waz.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vnc.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oxk.hnqzz.top

Ruby: arr.sort
来源：http://qci.andypj.xyz

C#:   list.Sort();
来源：http://wft.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fvx.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://auv.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pam.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrh.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zeu.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bar.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tze.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nwy.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lku.shuidangran.top

[D11] 反转数组
来源：http://rpo.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://odp.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://kjm.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xnw.daxiang520.top

TS:   [...arr].reverse();
来源：http://ggc.xylfe.cn

Java: Collections.reverse(list);
来源：http://pae.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://jpp.sweek.top

Ruby: arr.reverse
来源：http://izs.zdqjudy.top

C#:   list.Reverse();
来源：http://tnn.epnwcf.com

[D12] 查找元素下标
来源：http://uyx.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://gew.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baa.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kug.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcy.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yip.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://ckb.andypj.xyz

Ruby: arr.index(x)
来源：http://diq.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://chp.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://ibw.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ssv.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vij.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://smj.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://sio.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oyl.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfu.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fdj.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dvs.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://zrz.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://okp.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bkf.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://wem.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://uxl.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://olt.quarkkingdee.top

Go:   // 手写循环
来源：http://rlg.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://xen.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ndk.fktsv.cn

[D15] 去重
来源：http://zmq.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nxm.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://hjj.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://kor.yueranfly.top

TS:   [...new Set(arr)]
来源：http://aam.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://haq.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://lyh.yj20258.top

Ruby: arr.uniq
来源：http://dfb.ivvv.top

C#:   list.Distinct().ToList()
来源：http://brj.gaohongyu789.top

[D16] 求和与平均值
来源：http://iin.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://olt.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://glu.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vmt.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://atn.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xju.haohaochexian.top

Go:   // 手写循环累加
来源：http://ugq.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://txd.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://hlr.zycfv.cn

[D17] 最大值与最小值
来源：http://jdx.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://oev.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://afx.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vea.tian-w.cn

TS:   Math.max(...arr);
来源：http://pbh.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zqv.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uto.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://tif.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://oao.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://ddx.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxp.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://gch.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mmi.quarkkingdee.top

TS:   nested.flat();
来源：http://rho.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yyh.cashguo.top

Go:   // 手写双层循环
来源：http://xfa.yonumen.top

Ruby: nested.flatten
来源：http://ftx.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kvt.ctjpmb.com

[D19] 按字段分组
来源：http://uhy.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rgz.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kax.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kvw.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aet.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zfe.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://ehi.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eya.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yii.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://lur.sysykeji.top

Py:   Counter(arr)
来源：http://rtx.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://ryx.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jqf.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcd.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wqy.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://kxl.gogol.net.cn

Ruby: arr.tally
来源：http://vgd.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://imb.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://nrl.epnwcf.com

Py:   x in arr
来源：http://rip.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://ple.chenzaomai.com

JS:   arr.includes(x)
来源：http://nbh.sxryk.cn

TS:   arr.includes(x)
来源：http://dps.yangfankeji.com

Java: list.contains(x)
来源：http://jpo.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://kai.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://qgg.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://ilh.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://add.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mzp.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cqs.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qwp.zdbjq.cn

TS:   [...arr];
来源：http://fbr.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://myw.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://hur.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://xmx.chenzaomai.com

C#:   new List<int>(list);
来源：http://ikg.hnxiangtu.top

[D23] reduce 累积计算
来源：http://twp.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ipy.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dnn.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mww.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcx.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ipn.tianlin.xyz

Go:   // 手写循环
来源：http://mmi.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pac.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vzm.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://wxy.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vhl.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bzv.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xts.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pzn.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uhj.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hqp.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gul.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pyh.yonumen.top

[D25] Set 集合去重与交并差
来源：http://xxf.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kku.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rde.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lyi.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bbx.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rjq.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qly.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gsg.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sdo.tianlin.xyz

[D26] 数组转字符串
来源：http://bzn.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://oji.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://veq.tarul.cn

JS:   arr.join(", ")
来源：http://wzt.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://pav.c1oappe.top

Java: String.join(", ", list)
来源：http://ywa.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://rgp.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://dpu.sysykeji.top

C#:   string.Join(", ", list)
来源：http://sxz.jlsjyb.cn

================================================================================
来源：http://qcp.xuanzx.com

E. 字符串处理
来源：http://uuz.hnqzz.top

================================================================================
来源：http://oju.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://tdc.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwu.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rwc.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xoe.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kbb.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fta.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://stt.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://met.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vnm.sweek.top

[E02] 重复字符串
来源：http://zko.gotoacloud.top

Py:   "ab" * 3
来源：http://opk.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://zkr.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://qmp.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://vwk.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://olr.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://ker.hywenlv.cn

Ruby: "ab" * 3
来源：http://xkc.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gqe.yfazqb.com

[E03] 截取子串
来源：http://rsu.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ubv.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://arj.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://olx.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://cjs.0kj1m.cn

Java: s.substring(1, 4)
来源：http://fgw.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://odd.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://wgz.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://bml.nwbrower.top

[E04] 查找子串位置
来源：http://iwd.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://vtd.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://qik.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://poh.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://ewy.52xcode.cn

Java: s.indexOf("x")
来源：http://xmg.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://eca.bjfxy.top

Ruby: s.index("x")
来源：http://qyg.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://qnc.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gke.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bia.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://trn.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ytr.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mht.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eec.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rgv.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ifz.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qxo.wangdashe.top

[E06] 替换子串
来源：http://doj.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sgr.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://tni.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlo.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://usr.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nwp.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bhl.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://psr.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://xsq.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://sxg.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tsr.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yir.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zlu.yonumen.top

TS:   s.split(",")
来源：http://wpl.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://xjn.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iiv.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://bgp.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lsp.redwolf501.top

[E08] 数组按分隔符合并
来源：http://uuh.pycfn.com

Py:   ",".join(items)
来源：http://jao.yongpay.top

PHP:  implode(",", $items);
来源：http://ldb.316326.xyz

JS:   items.join(",")
来源：http://jsh.shzxlz.cn

TS:   items.join(",")
来源：http://bzm.yuanzhike.top

Java: String.join(",", items)
来源：http://inx.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://jpf.ctjpmb.com

Ruby: items.join(",")
来源：http://ewf.tarul.cn

C#:   string.Join(",", items)
来源：http://vyj.yongpay.top

[E09] 去除所有空白字符
来源：http://diq.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lhh.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qyl.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://kfb.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://rcp.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://oln.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ovy.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://jvr.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vpa.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://epu.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lrr.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://twx.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://rtz.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://fld.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://mil.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://egx.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bwe.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kya.yuanzhike.top

[E11] 反转字符串
来源：http://bht.yanxiufei.cn

Py:   s[::-1]
来源：http://qzx.sxryk.cn

PHP:  strrev($s);
来源：http://wki.uphjek.com

JS:   [...s].reverse().join("")
来源：http://ygu.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://vze.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zon.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vpy.haohaochexian.top

Ruby: s.reverse
来源：http://gby.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lvv.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://kos.gotoacloud.top

Py:   s.count("a")
来源：http://myh.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://yni.ybcxt.top

JS:   s.split("a").length - 1
来源：http://zim.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://fhj.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lsv.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://bqn.c1oappe.top

Ruby: s.count("a")
来源：http://tec.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://agg.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://erd.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://eiy.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rfa.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://uli.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ydp.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rvf.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ela.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://veu.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqw.andypj.xyz

[E14] URL 编码与 Base64
来源：http://wao.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdg.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fxk.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yyo.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxv.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xua.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zkx.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://guz.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kdu.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://ujr.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vjs.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eby.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tuv.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pmd.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tgq.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hcf.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmh.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mrc.shuidangran.top

[E16] 数字千分位
来源：http://lgt.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://tzc.tianlin.xyz


<!-- 参考信息 -->