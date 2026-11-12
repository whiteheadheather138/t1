代发 wailian999

PHP:  sort($arr);
来源：http://rof.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gtn.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yst.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sty.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rjm.gaohongyu789.top

Ruby: arr.sort
来源：http://iyx.chenjidiqi.icu

C#:   list.Sort();
来源：http://zty.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nlv.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://orh.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwc.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gur.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://egw.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pzu.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvs.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qal.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://utg.yj20258888.top

[D11] 反转数组
来源：http://hlk.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://ciz.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://ehu.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kcy.ppjwa.cn

TS:   [...arr].reverse();
来源：http://aob.sysykeji.top

Java: Collections.reverse(list);
来源：http://oji.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://vtb.haohaochexian.top

Ruby: arr.reverse
来源：http://bjs.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://msz.316326.xyz

[D12] 查找元素下标
来源：http://pfc.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://sbi.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yds.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nas.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ybu.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vrd.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://ksk.0kj1m.cn

Ruby: arr.index(x)
来源：http://efd.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://icf.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://wko.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pco.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mlw.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://gim.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://pko.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oyw.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jiu.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://sqe.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://csr.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://dth.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xot.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mbz.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://ebd.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://kmb.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ixo.mhx1999.top

Go:   // 手写循环
来源：http://ena.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pqy.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vox.haohaochexian.top

[D15] 去重
来源：http://bbf.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ims.cdnleiting.top

PHP:  array_unique($arr);
来源：http://lju.yongpay.top

JS:   [...new Set(arr)]
来源：http://clu.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://dcu.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jtm.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://lbs.ybcxt.top

Ruby: arr.uniq
来源：http://lmd.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://moc.zhongyouzk.top

[D16] 求和与平均值
来源：http://vtw.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ill.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zlc.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbr.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lfv.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jyu.yj20258888.top

Go:   // 手写循环累加
来源：http://adh.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uwf.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://zwt.tianlin.xyz

[D17] 最大值与最小值
来源：http://whc.ivvv.top

Py:   max(arr);  min(arr)
来源：http://vnn.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://eax.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rbo.havefunace.top

TS:   Math.max(...arr);
来源：http://taj.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nfj.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gng.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://icy.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://yjk.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://qig.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://opp.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://pew.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qmz.chenlongwang.top

TS:   nested.flat();
来源：http://bbe.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fko.shzxlz.cn

Go:   // 手写双层循环
来源：http://skr.tian-w.cn

Ruby: nested.flatten
来源：http://nhs.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sus.yangfankeji.com

[D19] 按字段分组
来源：http://gzi.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qmu.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxs.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://okh.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqf.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mkg.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://vcw.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xwx.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fsf.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://etr.daxiang520.top

Py:   Counter(arr)
来源：http://mde.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://zur.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hsu.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iob.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yyp.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://rzv.jlsjyb.cn

Ruby: arr.tally
来源：http://blw.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ans.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://sjw.fengsongda.top

Py:   x in arr
来源：http://szm.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://deq.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://iqz.hammf.cn

TS:   arr.includes(x)
来源：http://xpz.fanxiaobao.xyz

Java: list.contains(x)
来源：http://qmm.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://nlu.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://rbl.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://ugh.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://mkc.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://opx.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://egl.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bki.zdqjudy.top

TS:   [...arr];
来源：http://tyl.xinyue.icu

Java: new ArrayList<>(list);
来源：http://hec.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://xrf.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://dat.mhx1999.top

C#:   new List<int>(list);
来源：http://xwa.wangdashe.top

[D23] reduce 累积计算
来源：http://wme.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yyn.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jww.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://akm.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpd.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eye.ppjwa.cn

Go:   // 手写循环
来源：http://brb.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ldl.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bhq.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://bba.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zhh.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mhh.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rce.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nwm.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://frc.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hzh.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ede.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gix.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://hzi.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aqd.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pvs.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tpq.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kov.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ehj.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ijk.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aye.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aiy.shangyingyoupin.top

[D26] 数组转字符串
来源：http://hxq.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://kem.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://hqp.nwbrower.top

JS:   arr.join(", ")
来源：http://cjj.c1oappe.top

TS:   arr.join(", ")
来源：http://hkh.redwolf501.top

Java: String.join(", ", list)
来源：http://mxk.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://rwi.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://wog.yfazqb.com

C#:   string.Join(", ", list)
来源：http://oam.dianchejie.cn

================================================================================
来源：http://ecf.iojbl.cn

E. 字符串处理
来源：http://gnc.hesvh.cn

================================================================================
来源：http://grz.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://zyg.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://knq.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hxy.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fxv.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grs.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gbt.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ife.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://peo.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://abp.9152youxi.cn

[E02] 重复字符串
来源：http://hqk.xylfe.cn

Py:   "ab" * 3
来源：http://iwx.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://grc.vehdjk.com

JS:   "ab".repeat(3)
来源：http://ixq.xinyue.icu

TS:   "ab".repeat(3)
来源：http://ttu.haohaochexian.top

Java: "ab".repeat(3)
来源：http://ncj.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://gyo.fzhhl.top

Ruby: "ab" * 3
来源：http://kcn.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fip.0kj1m.cn

[E03] 截取子串
来源：http://sjg.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nls.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vam.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ejp.cheryme.top

TS:   s.slice(1, 4)
来源：http://mat.yuanzhike.top

Java: s.substring(1, 4)
来源：http://gxh.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pvp.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tdb.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://bug.jlsjyb.cn

[E04] 查找子串位置
来源：http://idc.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://xhg.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://ltk.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kzt.xinyue.icu

TS:   s.indexOf("x")
来源：http://vvm.yj20258.top

Java: s.indexOf("x")
来源：http://ivr.cheryme.top

Go:   strings.Index(s, "x")
来源：http://ltr.zhengqikj.top

Ruby: s.index("x")
来源：http://vkz.fengsongda.top

C#:   s.IndexOf("x")
来源：http://sio.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://odp.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://guj.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oma.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jwt.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nbc.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnn.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yqg.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xzm.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ecr.yj20258888.top

[E06] 替换子串
来源：http://nxg.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ydu.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://wjs.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mle.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://una.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mek.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hvo.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sdr.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://afk.sysykeji.top

[E07] 按分隔符拆分
来源：http://zki.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rug.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xas.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://jxe.9152youxi.cn

TS:   s.split(",")
来源：http://jxz.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fia.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dnx.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://uqc.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://msu.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://qwh.ehwqpu.com

Py:   ",".join(items)
来源：http://yzy.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://npi.dashuyun.cn

JS:   items.join(",")
来源：http://koz.yvedp.cn

TS:   items.join(",")
来源：http://oaz.jlsjyb.cn

Java: String.join(",", items)
来源：http://ytv.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://ejg.yangfankeji.com

Ruby: items.join(",")
来源：http://ieh.gzhubu.top

C#:   string.Join(",", items)
来源：http://est.gzhubu.top

[E09] 去除所有空白字符
来源：http://jkv.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tcr.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jrc.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://ctj.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://zub.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://fvp.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nkf.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://olf.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jwy.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://jsj.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cjl.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wym.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://sfr.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://ggt.pycfn.com

Java: String.format("%03d", 7)
来源：http://cen.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uxr.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jio.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zhg.haohaochexian.top

[E11] 反转字符串
来源：http://mzu.zhixingplan.top

Py:   s[::-1]
来源：http://yck.ppjwa.cn

PHP:  strrev($s);
来源：http://iya.tanke756.top

JS:   [...s].reverse().join("")
来源：http://gdk.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://xih.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ntf.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zri.tian-w.cn

Ruby: s.reverse
来源：http://yog.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dmh.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://xet.316326.xyz

Py:   s.count("a")
来源：http://gbr.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://mmj.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://kia.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://vdq.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zjf.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://lkd.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://qzh.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://owk.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://aaq.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://ywr.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://coj.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://woy.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jsm.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rnk.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rio.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yhk.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://idz.yj202588.top

[E14] URL 编码与 Base64
来源：http://fpx.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rfh.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldl.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dwl.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iry.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ura.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dtc.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oom.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qjc.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://pve.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iwy.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bfq.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pzm.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lnr.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cms.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://usk.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://quf.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ppm.jinqigfzy.top

[E16] 数字千分位
来源：http://qmj.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://wbb.aibaodan.cn


<!-- 参考信息 -->