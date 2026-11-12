代发 wailian999

[D07] 切片 / 取子数组
来源：http://aqd.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ysf.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fkp.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://tro.yongpay.top

TS:   arr.slice(1, 4);
来源：http://vyk.jyoumei.cn

Java: list.subList(1, 4);
来源：http://zpn.sysykeji.top

Go:   arr[1:4]
来源：http://kuy.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://taw.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://dbm.gzhubu.top

[D08] 合并两个数组
来源：http://nrx.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://rwu.cheryme.top

PHP:  array_merge($a, $b);
来源：http://rnf.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ilc.shzxlz.cn

TS:   [...a, ...b];
来源：http://mvi.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ern.wangdashe.top

Go:   append(a, b...)
来源：http://iif.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://lea.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://ezs.feifeiyinyue.top

[D09] 排序（升序）
来源：http://isc.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://mhe.gaohongyu789.top

PHP:  sort($arr);
来源：http://nck.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qtx.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jgj.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://sxl.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jiw.aizwys.cn

Ruby: arr.sort
来源：http://tkp.yj20258.top

C#:   list.Sort();
来源：http://kej.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://agf.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jau.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://stb.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzl.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghd.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvz.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vlu.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vwi.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qxa.fanxiaobao.xyz

[D11] 反转数组
来源：http://wyk.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bky.fktsv.cn

PHP:  array_reverse($arr);
来源：http://dnu.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gap.yonumen.top

TS:   [...arr].reverse();
来源：http://kzk.52xcode.cn

Java: Collections.reverse(list);
来源：http://yua.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://czg.hammf.cn

Ruby: arr.reverse
来源：http://bkh.aizwys.cn

C#:   list.Reverse();
来源：http://djv.ydzc1.top

[D12] 查找元素下标
来源：http://vhp.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://ocm.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rje.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jiu.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mny.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://crq.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://ynk.yuanzhike.top

Ruby: arr.index(x)
来源：http://hrw.xuanzx.com

C#:   list.IndexOf(x);
来源：http://fcc.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://byg.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aqh.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jci.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://muv.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://upq.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rcp.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dvc.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://pgi.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gbr.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://yws.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uml.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ztp.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://rbd.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://eja.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ylj.hfpthk.cn

Go:   // 手写循环
来源：http://gre.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gzr.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://smv.guowangkeji.top

[D15] 去重
来源：http://jva.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://adn.smart0.xyz

PHP:  array_unique($arr);
来源：http://ucw.aizwys.cn

JS:   [...new Set(arr)]
来源：http://qof.sysykeji.top

TS:   [...new Set(arr)]
来源：http://ywk.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jlc.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://ffj.yfazqb.com

Ruby: arr.uniq
来源：http://vzy.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://nlp.gzhubu.top

[D16] 求和与平均值
来源：http://lkc.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ruw.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oay.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pjb.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://trw.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vwj.aizwys.cn

Go:   // 手写循环累加
来源：http://baq.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zzi.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://xws.jyoumei.cn

[D17] 最大值与最小值
来源：http://xkt.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://cad.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://xpu.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fbn.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://kuo.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://she.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jrb.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://kfn.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://ruo.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://liy.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jlf.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://hgr.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xhz.ivvv.top

TS:   nested.flat();
来源：http://gfb.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lia.aizwys.cn

Go:   // 手写双层循环
来源：http://gef.zhengqikj.top

Ruby: nested.flatten
来源：http://mkm.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ziq.jlsjyb.cn

[D19] 按字段分组
来源：http://yjf.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nxq.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uqk.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nwp.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nnr.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gtw.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://eqg.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hah.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fbz.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://sbp.bbcook.cn

Py:   Counter(arr)
来源：http://zhi.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://qfr.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lyb.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bou.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://amj.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://dvm.jyoumei.cn

Ruby: arr.tally
来源：http://ckh.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kgb.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://bla.jinqigufen.top

Py:   x in arr
来源：http://iqo.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://qac.tanke756.top

JS:   arr.includes(x)
来源：http://kyo.fehbvm.com

TS:   arr.includes(x)
来源：http://msc.chenlongwang.top

Java: list.contains(x)
来源：http://qfq.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://dyn.epnwcf.com

Ruby: arr.include?(x)
来源：http://imj.zhijiandao.cn

C#:   list.Contains(x)
来源：http://ddh.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://ath.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sdb.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ezb.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gzf.yueranfly.top

TS:   [...arr];
来源：http://yow.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://zvk.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://nss.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://jsu.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://qwo.sysykeji.top

[D23] reduce 累积计算
来源：http://vpz.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jnr.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://itk.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhw.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kuq.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihf.316326.xyz

Go:   // 手写循环
来源：http://nvr.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cez.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://drp.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://pkw.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://noh.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qlc.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydv.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://twv.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qpr.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbg.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://djy.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://weh.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://ovf.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bqb.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qoh.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xpd.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dlh.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vmk.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://amu.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gbt.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cjk.yueranfly.top

[D26] 数组转字符串
来源：http://qki.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://bbu.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://rxa.zhoulong.xyz

JS:   arr.join(", ")
来源：http://vej.havefunace.top

TS:   arr.join(", ")
来源：http://guy.aizwys.cn

Java: String.join(", ", list)
来源：http://bfr.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://eyu.jqgfzy.top

Ruby: arr.join(", ")
来源：http://yko.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://xfo.redwolf501.top

================================================================================
来源：http://aix.shanyushiyangkeji.top

E. 字符串处理
来源：http://jke.xylfe.cn

================================================================================
来源：http://lvj.yfazqb.com

[E01] 拼接字符串
来源：http://zqf.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fxk.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fsq.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gbf.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gox.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://idu.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lrq.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zsa.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jnn.zhongyouzk.top

[E02] 重复字符串
来源：http://jiq.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://fzj.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://wzo.zycfv.cn

JS:   "ab".repeat(3)
来源：http://isx.xziqi.cn

TS:   "ab".repeat(3)
来源：http://tjh.nanxinkj.top

Java: "ab".repeat(3)
来源：http://hov.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://vlk.hnxiangtu.top

Ruby: "ab" * 3
来源：http://xyh.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ylo.hesvh.cn

[E03] 截取子串
来源：http://qau.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cmi.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nbw.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://umb.mhx1999.top

TS:   s.slice(1, 4)
来源：http://gku.jyoumei.cn

Java: s.substring(1, 4)
来源：http://cqc.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://azd.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://hfr.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://jzm.jinqigufen.top

[E04] 查找子串位置
来源：http://kqw.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://gyr.redwolf501.top

PHP:  strpos($s, "x");
来源：http://bkz.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yji.yueranfly.top

TS:   s.indexOf("x")
来源：http://ocs.hywenlv.cn

Java: s.indexOf("x")
来源：http://pbc.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://ecr.dashuyun.cn

Ruby: s.index("x")
来源：http://vfp.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://aio.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uel.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gwi.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yqs.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://azx.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hdh.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxk.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fgi.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://trk.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zmt.yj202588.top

[E06] 替换子串
来源：http://ijn.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mho.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://rqk.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pck.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://xaq.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpu.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mmi.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cnv.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://ypt.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://jlr.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ssx.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rev.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://okn.redwolf501.top

TS:   s.split(",")
来源：http://zgg.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rzs.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mcn.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://sgx.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://edn.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://agq.epnwcf.com

Py:   ",".join(items)
来源：http://vsv.snrcjt.cn

PHP:  implode(",", $items);
来源：http://sxp.zhengqikj.top

JS:   items.join(",")
来源：http://xhp.ivvv.top

TS:   items.join(",")
来源：http://xan.chenlongwang.top

Java: String.join(",", items)
来源：http://pet.havefunace.top

Go:   strings.Join(items, ",")
来源：http://pqr.ydjk.org.cn

Ruby: items.join(",")
来源：http://rtl.fktsv.cn

C#:   string.Join(",", items)
来源：http://hrp.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://oxw.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nzf.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ubx.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://fik.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://joy.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://unv.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://xfp.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://gvi.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eor.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://fee.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lbw.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jjk.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://nbo.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://guz.xinyue.icu

Java: String.format("%03d", 7)
来源：http://kwn.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ocq.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtf.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qpb.pycfn.com

[E11] 反转字符串
来源：http://omn.snrcjt.cn

Py:   s[::-1]
来源：http://lwv.hnxiangtu.top

PHP:  strrev($s);
来源：http://hzp.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://mjy.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://llm.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ovx.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzs.ivvv.top

Ruby: s.reverse
来源：http://bmf.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://qoj.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://hdh.316326.xyz

Py:   s.count("a")
来源：http://dxa.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://gru.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://jnt.hcnkem.com

TS:   s.split("a").length - 1
来源：http://icr.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xii.tarul.cn

Go:   strings.Count(s, "a")
来源：http://iid.yanxiufei.cn

Ruby: s.count("a")
来源：http://dlo.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://pka.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://uno.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://des.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mqs.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lnl.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mwk.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cfz.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://clp.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pga.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fnp.dashuyun.cn


<!-- 参考信息 -->