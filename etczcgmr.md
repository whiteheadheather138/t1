代发 wailian999

TS:   arr.slice(1, 4);
来源：http://fnr.smart0.xyz

Java: list.subList(1, 4);
来源：http://jmb.yuxming.cn

Go:   arr[1:4]
来源：http://dka.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://hcj.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://mwg.ydzc1.top

[D08] 合并两个数组
来源：http://khz.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://fvx.sweek.top

PHP:  array_merge($a, $b);
来源：http://zhj.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wwm.jlsjyb.cn

TS:   [...a, ...b];
来源：http://svu.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zrx.dashuyun.cn

Go:   append(a, b...)
来源：http://bkv.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://ote.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://wpz.shangyingyoupin.top

[D09] 排序（升序）
来源：http://dtt.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://the.ehwqpu.com

PHP:  sort($arr);
来源：http://wec.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ncs.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dop.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zio.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yck.wangshuangyany.cn

Ruby: arr.sort
来源：http://lti.chenzaomai.com

C#:   list.Sort();
来源：http://ezx.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pld.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://acp.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vtv.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://elu.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pul.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xvf.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://euo.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqm.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hen.hesvh.cn

[D11] 反转数组
来源：http://lsa.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://zbi.hcnkem.com

PHP:  array_reverse($arr);
来源：http://mhk.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://doc.xinyue.icu

TS:   [...arr].reverse();
来源：http://uya.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://jkw.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://mlr.tian-w.cn

Ruby: arr.reverse
来源：http://wno.gzhubu.top

C#:   list.Reverse();
来源：http://jsk.tanke756.top

[D12] 查找元素下标
来源：http://pzx.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://sov.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://icv.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bfp.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbe.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ppk.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://mlm.mhx1999.top

Ruby: arr.index(x)
来源：http://chc.andypj.xyz

C#:   list.IndexOf(x);
来源：http://pzk.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://ggy.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cfa.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://buk.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://fgt.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://qit.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nlu.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wda.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ast.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://nzo.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://fga.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lap.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://muh.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://lyu.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://rhv.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hck.fktsv.cn

Go:   // 手写循环
来源：http://hki.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://zqf.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fdi.ydjk.org.cn

[D15] 去重
来源：http://hoh.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lyf.gzhubu.top

PHP:  array_unique($arr);
来源：http://nxi.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://rbf.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://twu.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oqv.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://xml.sufxvd.cn

Ruby: arr.uniq
来源：http://quj.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://hpw.quarkkingdee.top

[D16] 求和与平均值
来源：http://mqa.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jwq.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yft.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://psa.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhq.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qrs.guannengcc.top

Go:   // 手写循环累加
来源：http://adq.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mpz.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://gde.jlsjyb.cn

[D17] 最大值与最小值
来源：http://rsv.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://inb.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://fhl.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ufa.shuidangran.top

TS:   Math.max(...arr);
来源：http://qzv.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://opg.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ivl.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://bde.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://yso.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://ohb.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ozd.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://skw.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hnu.52xcode.cn

TS:   nested.flat();
来源：http://flw.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ary.jlsjyb.cn

Go:   // 手写双层循环
来源：http://nws.jqgfzy.top

Ruby: nested.flatten
来源：http://yjy.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://lew.epnwcf.com

[D19] 按字段分组
来源：http://iyu.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ros.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://thm.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qaz.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qag.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggb.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://phu.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ors.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iga.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://vax.yvedp.cn

Py:   Counter(arr)
来源：http://mxn.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://cgu.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://usc.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://toz.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nno.shuidangran.top

Go:   // 手写 map[T]int
来源：http://qrw.cheryme.top

Ruby: arr.tally
来源：http://svs.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hqe.ydzc1.top

[D21] 判断是否包含某元素
来源：http://sez.andypj.xyz

Py:   x in arr
来源：http://ioa.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://vue.9152youxi.cn

JS:   arr.includes(x)
来源：http://vcf.haohaochexian.top

TS:   arr.includes(x)
来源：http://ltz.sysykeji.top

Java: list.contains(x)
来源：http://sgh.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://vvq.dashuyun.cn

Ruby: arr.include?(x)
来源：http://hkd.gotoacloud.top

C#:   list.Contains(x)
来源：http://gya.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://rmt.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://crg.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gtu.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qxs.cqqwz.cn

TS:   [...arr];
来源：http://gvg.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://nln.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://vfr.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://bgi.cqqwz.cn

C#:   new List<int>(list);
来源：http://ish.aizwys.cn

[D23] reduce 累积计算
来源：http://mwl.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ejq.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ego.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nan.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oog.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://axs.yangfankeji.com

Go:   // 手写循环
来源：http://dix.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zfk.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lnq.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://wzb.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://crk.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kfb.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myc.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ibt.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tgl.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ipn.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kfu.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vlh.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://wpw.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xcp.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kel.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iln.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dzy.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sqv.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jce.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qyq.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jwf.kuanghao11.cn

[D26] 数组转字符串
来源：http://qyl.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://kko.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://sos.fktsv.cn

JS:   arr.join(", ")
来源：http://emn.nwbrower.top

TS:   arr.join(", ")
来源：http://ose.ydjk.org.cn

Java: String.join(", ", list)
来源：http://sjj.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://lvz.daria6918.cn

Ruby: arr.join(", ")
来源：http://gnt.ybcxt.top

C#:   string.Join(", ", list)
来源：http://tfc.hysaishi.cn

================================================================================
来源：http://gwh.chenjidiqi.icu

E. 字符串处理
来源：http://gmj.ehwqpu.com

================================================================================
来源：http://qyg.yangfankeji.com

[E01] 拼接字符串
来源：http://pjp.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iuu.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cqv.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zhm.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qev.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iqf.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://biu.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kti.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmh.jlsjyb.cn

[E02] 重复字符串
来源：http://mut.yangfankeji.com

Py:   "ab" * 3
来源：http://ptg.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://xln.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://esx.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://cje.bbcook.cn

Java: "ab".repeat(3)
来源：http://sqv.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://bqm.guowangkeji.top

Ruby: "ab" * 3
来源：http://wef.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://slq.yueranfly.top

[E03] 截取子串
来源：http://hqi.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qbm.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ofz.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wrh.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://jgr.fktsv.cn

Java: s.substring(1, 4)
来源：http://qiq.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zkh.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cux.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://hcw.hywenlv.cn

[E04] 查找子串位置
来源：http://hek.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://iqs.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://kcz.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hla.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://rab.yj20258888.top

Java: s.indexOf("x")
来源：http://avb.yj202588.top

Go:   strings.Index(s, "x")
来源：http://mjl.zdqjudy.top

Ruby: s.index("x")
来源：http://hov.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://fww.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gln.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rbw.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://evp.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkq.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://huu.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qeo.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gcj.fanxiaobao.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xxg.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fbt.smart0.xyz

[E06] 替换子串
来源：http://lxo.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ebb.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://qci.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqt.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://hgw.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://los.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://syb.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rev.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://qam.9152youxi.cn

[E07] 按分隔符拆分
来源：http://dci.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wby.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zex.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yfr.52xcode.cn

TS:   s.split(",")
来源：http://qeo.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://kmk.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydx.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://mmv.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ukd.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://sjq.tanke756.top

Py:   ",".join(items)
来源：http://vta.nwbrower.top

PHP:  implode(",", $items);
来源：http://dgo.xziqi.cn

JS:   items.join(",")
来源：http://frd.hongshengwenyu.top

TS:   items.join(",")
来源：http://iib.52xcode.cn

Java: String.join(",", items)
来源：http://ito.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://efy.hywenlv.cn

Ruby: items.join(",")
来源：http://sly.sxryk.cn

C#:   string.Join(",", items)
来源：http://bae.tianlin.xyz

[E09] 去除所有空白字符
来源：http://ito.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ydq.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zdu.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://xzm.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://yhe.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://oee.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://enw.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zjw.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oor.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://bil.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yiv.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bch.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://lsk.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://byd.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://ecv.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ald.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kip.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vjb.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://qry.zycfv.cn

Py:   s[::-1]
来源：http://cot.meibo888.top

PHP:  strrev($s);
来源：http://wlk.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://fge.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://bon.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bbx.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qrz.zhijiandao.cn

Ruby: s.reverse
来源：http://gyq.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://bhf.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://syu.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://ltn.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://rrx.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://cgd.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://ubp.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mug.yj20258.top

Go:   strings.Count(s, "a")
来源：http://tdh.fktsv.cn

Ruby: s.count("a")
来源：http://yss.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://ymn.yj202588.top

[E13] 逐字符遍历
来源：http://vxm.birdmap.top

Py:   for ch in s: print(ch)
来源：http://lht.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wtc.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxl.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vzk.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mci.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jfj.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wrg.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dox.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://mkp.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lbc.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eti.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rff.cdnleiting.top


<!-- 参考信息 -->