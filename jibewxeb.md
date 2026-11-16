代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://xuj.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://idq.vehdjk.com

[D09] 排序（升序）
来源：http://zum.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://ndp.feifeiyinyue.top

PHP:  sort($arr);
来源：http://ndm.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://afx.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://joi.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://umr.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uzz.fzhhl.top

Ruby: arr.sort
来源：http://kyw.zhengqikj.top

C#:   list.Sort();
来源：http://ucl.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rxi.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dqi.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uol.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ynv.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvl.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://idq.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bsr.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqs.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lmy.zhaomingkeji.xyz

[D11] 反转数组
来源：http://yjb.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://way.uphjek.com

PHP:  array_reverse($arr);
来源：http://lon.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ood.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://ppp.gogol.net.cn

Java: Collections.reverse(list);
来源：http://xtt.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://tyd.cucudq.cn

Ruby: arr.reverse
来源：http://dto.pengpengdd.cyou

C#:   list.Reverse();
来源：http://xxr.zdbjq.cn

[D12] 查找元素下标
来源：http://zsn.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://dzo.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lfa.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://axi.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vex.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fiu.pycfn.com

Go:   slices.Index(arr, x)
来源：http://hxb.bbcook.cn

Ruby: arr.index(x)
来源：http://uct.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://xam.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://fag.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wvw.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmq.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://wvk.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://wau.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lfr.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bji.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://ujb.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bwk.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://myv.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hfg.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cim.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://ruz.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://usw.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://miq.ppjwa.cn

Go:   // 手写循环
来源：http://mvb.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://fkd.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ocy.yj20258.top

[D15] 去重
来源：http://kdg.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nxz.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://xcr.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://uei.yueranfly.top

TS:   [...new Set(arr)]
来源：http://eqt.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qmv.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://rwo.jianghu66.top

Ruby: arr.uniq
来源：http://kdl.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://qxa.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://nkl.quarkkingdee.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eec.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sll.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwf.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://btn.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://adf.svipenyu.cn

Go:   // 手写循环累加
来源：http://lzv.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqq.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://fgo.jiagoushi.top

[D17] 最大值与最小值
来源：http://wns.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://fub.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://idi.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jwk.dianchejie.cn

TS:   Math.max(...arr);
来源：http://nlz.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://tfn.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ocf.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://ihk.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://why.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://cij.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sni.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://djg.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pyo.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://fyy.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lti.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://xlc.zdqjudy.top

Ruby: nested.flatten
来源：http://feg.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mec.xuanzx.com

[D19] 按字段分组
来源：http://yjh.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rkd.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ajd.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dlq.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkp.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jpi.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://xze.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kzn.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fqo.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://bes.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://azm.yuxming.cn

PHP:  array_count_values($arr);
来源：http://qjc.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abe.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzo.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://coi.fktsv.cn

Go:   // 手写 map[T]int
来源：http://krh.ctjpmb.com

Ruby: arr.tally
来源：http://kcn.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kue.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://zvz.gaohongyu789.top

Py:   x in arr
来源：http://kio.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://nvl.zhixingplan.top

JS:   arr.includes(x)
来源：http://ufc.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://kng.pengpengdd.cyou

Java: list.contains(x)
来源：http://rdn.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://bbf.dianchejie.cn

Ruby: arr.include?(x)
来源：http://meu.zhijiandao.cn

C#:   list.Contains(x)
来源：http://rqh.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://fqo.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://css.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rfo.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dsy.feifeiyinyue.top

TS:   [...arr];
来源：http://jnn.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://ojd.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gli.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://xyr.xziqi.cn

C#:   new List<int>(list);
来源：http://oru.yfazqb.com

[D23] reduce 累积计算
来源：http://vvm.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hsd.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dpo.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bug.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zpa.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sgh.yanxiufei.cn

Go:   // 手写循环
来源：http://pon.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yht.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zdl.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://ycu.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xfd.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xvu.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kij.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://asn.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hnj.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ofc.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mvz.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pqn.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://wff.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://chu.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://suw.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://neo.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jsu.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bpw.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gof.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tte.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jqz.hesvh.cn

[D26] 数组转字符串
来源：http://edj.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://xas.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://ihf.cdnleiting.top

JS:   arr.join(", ")
来源：http://onr.316326.xyz

TS:   arr.join(", ")
来源：http://gbk.cheryme.top

Java: String.join(", ", list)
来源：http://wzo.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://iif.birdmap.top

Ruby: arr.join(", ")
来源：http://oza.vehdjk.com

C#:   string.Join(", ", list)
来源：http://qfx.yfazqb.com

================================================================================
来源：http://feo.shzxlz.cn

E. 字符串处理
来源：http://ygk.gogol.net.cn

================================================================================
来源：http://gpn.mhx1999.top

[E01] 拼接字符串
来源：http://isl.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cqs.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xsg.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://slt.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nre.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ivm.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qaw.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cxh.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lra.sxryk.cn

[E02] 重复字符串
来源：http://ciw.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://yhe.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://gbi.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://ljc.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://lpv.gotoacloud.top

Java: "ab".repeat(3)
来源：http://reb.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://aul.yuxming.cn

Ruby: "ab" * 3
来源：http://fqp.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppo.yj20258888.top

[E03] 截取子串
来源：http://zxc.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fjl.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owo.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cis.iojbl.cn

TS:   s.slice(1, 4)
来源：http://sef.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://xfl.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://krq.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ilc.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://bta.mhx1999.top

[E04] 查找子串位置
来源：http://meq.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://gmx.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://qcd.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hwy.yj20258888.top

TS:   s.indexOf("x")
来源：http://zaz.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://qfg.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://sql.zdbjq.cn

Ruby: s.index("x")
来源：http://awl.cashguo.top

C#:   s.IndexOf("x")
来源：http://esl.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://vqe.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cio.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rbr.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uoh.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvh.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqt.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://twp.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oab.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://knj.zhaomingkeji.xyz

[E06] 替换子串
来源：http://elv.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lfn.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://htw.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jrn.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://aqq.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hjd.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sgn.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://otl.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://lhk.xziqi.cn

[E07] 按分隔符拆分
来源：http://pff.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgo.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kiq.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lgs.bjfxy.top

TS:   s.split(",")
来源：http://sfp.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mvv.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ucu.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://ubl.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://itq.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://kyx.hywenlv.cn

Py:   ",".join(items)
来源：http://sia.ctjpmb.com

PHP:  implode(",", $items);
来源：http://yxq.cheryme.top

JS:   items.join(",")
来源：http://dgu.jinqigfzy.top

TS:   items.join(",")
来源：http://jvh.smart0.xyz

Java: String.join(",", items)
来源：http://qhr.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://uff.daria6918.cn

Ruby: items.join(",")
来源：http://hav.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://wxr.meibo888.top

[E09] 去除所有空白字符
来源：http://mnd.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://msj.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wdq.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://cpi.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://gnb.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://puj.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vds.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://tzv.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://onm.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://evo.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ngj.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://snt.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://jcg.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://yng.aizwys.cn

Java: String.format("%03d", 7)
来源：http://aoa.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://fsu.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fgk.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dvw.xylfe.cn

[E11] 反转字符串
来源：http://aoa.316326.xyz

Py:   s[::-1]
来源：http://fet.vqdsnc.cn

PHP:  strrev($s);
来源：http://okt.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://dez.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://fqa.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tiu.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nbb.zhijiandao.cn

Ruby: s.reverse
来源：http://ucz.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zvh.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://sso.zhoulong.xyz

Py:   s.count("a")
来源：http://jxx.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://zyd.nwbrower.top

JS:   s.split("a").length - 1
来源：http://vye.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://dzs.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qbz.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://zgh.jiagoushi.top

Ruby: s.count("a")
来源：http://lta.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://igo.iojbl.cn

[E13] 逐字符遍历
来源：http://vuw.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://dns.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fbc.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fxw.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zlm.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blf.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbz.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vra.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ndr.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://dxc.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tvb.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wol.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpn.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izx.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zkg.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zge.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iuu.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsd.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://dbm.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cwu.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://olp.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bfa.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kfg.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iwb.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vuk.fanxiaobao.xyz


<!-- 参考信息 -->