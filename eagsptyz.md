代发 wailian999

Py:   len(arr)
来源：http://sms.316326.xyz

PHP:  count($arr);
来源：http://lvm.hfpthk.cn

JS:   arr.length
来源：http://ylm.svipenyu.cn

TS:   arr.length
来源：http://sqg.tanke756.top

Java: list.size();
来源：http://qjf.shangyingyoupin.top

Go:   len(arr)
来源：http://qqe.zycfv.cn

Ruby: arr.length; arr.size
来源：http://wre.gzhubu.top

C#:   list.Count;
来源：http://qma.xylfe.cn

[D07] 切片 / 取子数组
来源：http://wot.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxr.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://efc.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://lbj.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://qwd.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://xoh.zdbjq.cn

Go:   arr[1:4]
来源：http://jgb.shuidangran.top

Ruby: arr[1, 3]
来源：http://wvg.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://fvg.xuanzx.com

[D08] 合并两个数组
来源：http://hzn.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://njr.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://wng.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fma.yj20258.top

TS:   [...a, ...b];
来源：http://ovo.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cwn.tian-w.cn

Go:   append(a, b...)
来源：http://ntu.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://erc.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://xzp.gzhubu.top

[D09] 排序（升序）
来源：http://rbu.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://rvu.nanxuanxn.top

PHP:  sort($arr);
来源：http://aha.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nod.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ihf.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://uci.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uuc.aizwys.cn

Ruby: arr.sort
来源：http://lzv.yuanzhike.top

C#:   list.Sort();
来源：http://xzu.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zmk.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ujc.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ndz.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sna.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejh.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lru.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lvc.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pfy.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfn.ehwqpu.com

[D11] 反转数组
来源：http://hcy.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sjt.epnwcf.com

PHP:  array_reverse($arr);
来源：http://tsu.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fhj.tarul.cn

TS:   [...arr].reverse();
来源：http://vvv.zhengqikj.top

Java: Collections.reverse(list);
来源：http://iwn.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://ppe.ehwqpu.com

Ruby: arr.reverse
来源：http://sxz.daria6918.cn

C#:   list.Reverse();
来源：http://qrg.svipenyu.cn

[D12] 查找元素下标
来源：http://gtq.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://cas.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cmu.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://map.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fqs.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ptv.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://eve.daria6918.cn

Ruby: arr.index(x)
来源：http://jzb.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://muk.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://nhp.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bsd.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://txm.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://ypq.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://zia.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qkn.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iri.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://nfd.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://enk.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://eci.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ccn.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kpk.sweek.top

JS:   arr.map(x => x * 2)
来源：http://foq.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://tpj.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zse.jianghu66.top

Go:   // 手写循环
来源：http://izl.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vrv.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ozs.snrcjt.cn

[D15] 去重
来源：http://gvu.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rda.hywenlv.cn

PHP:  array_unique($arr);
来源：http://gyq.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://plc.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://lob.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gzj.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://zsg.aizwys.cn

Ruby: arr.uniq
来源：http://nie.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://xks.zhixingplan.top

[D16] 求和与平均值
来源：http://ehe.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://msu.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cic.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcf.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kch.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dwe.quarkkingdee.top

Go:   // 手写循环累加
来源：http://zou.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fqn.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://ekm.gzhubu.top

[D17] 最大值与最小值
来源：http://tqh.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://dyr.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://lyl.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ofy.yuanzhike.top

TS:   Math.max(...arr);
来源：http://nwn.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iew.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dcu.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://ayd.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://xmc.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://kgo.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jyy.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://qzo.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cqc.gogol.net.cn

TS:   nested.flat();
来源：http://rkw.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ltz.shzxlz.cn

Go:   // 手写双层循环
来源：http://hhn.gzhubu.top

Ruby: nested.flatten
来源：http://xyg.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://atx.zhongyouzk.top

[D19] 按字段分组
来源：http://qwj.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://smm.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rxn.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yad.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ckd.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uys.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://ezq.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sjg.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wqe.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://xxk.jqgufenzy.top

Py:   Counter(arr)
来源：http://pxz.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://npw.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fek.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hvp.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zxm.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://usv.pycfn.com

Ruby: arr.tally
来源：http://six.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wjv.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://rec.ppjwa.cn

Py:   x in arr
来源：http://cja.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://lgj.bjfxy.top

JS:   arr.includes(x)
来源：http://ulz.hfpthk.cn

TS:   arr.includes(x)
来源：http://hox.vqdsnc.cn

Java: list.contains(x)
来源：http://qwy.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://uvu.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://pve.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://ccw.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://tdt.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mix.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oiz.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rel.gotoacloud.top

TS:   [...arr];
来源：http://awu.vehdjk.com

Java: new ArrayList<>(list);
来源：http://ahz.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://puq.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://qcw.cashguo.top

C#:   new List<int>(list);
来源：http://qlc.redwolf501.top

[D23] reduce 累积计算
来源：http://uqd.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ica.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jxw.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfo.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfs.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qzr.ctjpmb.com

Go:   // 手写循环
来源：http://wzw.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bcn.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wzc.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://qas.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ulm.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aff.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jwb.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dfk.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kzl.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uuj.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://swg.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eqi.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://zra.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aea.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wfr.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dve.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gkd.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rhw.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vws.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yrl.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qov.nanxinkj.top

[D26] 数组转字符串
来源：http://lqx.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://bts.yonumen.top

PHP:  implode(", ", $arr);
来源：http://pyr.jqgufenzy.top

JS:   arr.join(", ")
来源：http://pvu.yongpay.top

TS:   arr.join(", ")
来源：http://naq.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://btv.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://cnq.fengsongda.top

Ruby: arr.join(", ")
来源：http://ifz.yongpay.top

C#:   string.Join(", ", list)
来源：http://fas.gzhubu.top

================================================================================
来源：http://vxr.zhoulong.xyz

E. 字符串处理
来源：http://fop.gotoacloud.top

================================================================================
来源：http://jko.xuanzx.com

[E01] 拼接字符串
来源：http://lbi.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zax.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wak.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tmz.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlw.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wfb.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jiq.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yzr.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vxk.gzhubu.top

[E02] 重复字符串
来源：http://fyq.yfazqb.com

Py:   "ab" * 3
来源：http://imf.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://baw.fktsv.cn

JS:   "ab".repeat(3)
来源：http://row.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://hhc.snrcjt.cn

Java: "ab".repeat(3)
来源：http://srb.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://hap.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://rno.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lcb.fengsongda.top

[E03] 截取子串
来源：http://cth.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://caz.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ipr.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xto.52xcode.cn

TS:   s.slice(1, 4)
来源：http://jej.yfazqb.com

Java: s.substring(1, 4)
来源：http://waq.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iee.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://dnw.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://bnv.shangyingyoupin.top

[E04] 查找子串位置
来源：http://dxa.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://urj.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://wkx.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aco.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://xns.wangdashe.top

Java: s.indexOf("x")
来源：http://mma.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://ayt.yj20258.top

Ruby: s.index("x")
来源：http://tdo.sxryk.cn

C#:   s.IndexOf("x")
来源：http://cmd.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pou.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fye.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lfb.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zuf.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sds.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bea.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ffb.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://klq.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uvf.kuanghao11.cn

[E06] 替换子串
来源：http://wbc.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ong.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://oyu.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwb.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://trr.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gvx.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hxf.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://frt.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://cfb.gzhubu.top

[E07] 按分隔符拆分
来源：http://por.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://isu.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pse.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kqx.svipenyu.cn

TS:   s.split(",")
来源：http://pgy.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jwh.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://flm.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://rjs.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yvg.fengsongda.top

[E08] 数组按分隔符合并
来源：http://hsq.yueranfly.top

Py:   ",".join(items)
来源：http://gas.c1oappe.top

PHP:  implode(",", $items);
来源：http://tif.zdqjudy.top

JS:   items.join(",")
来源：http://jmy.vqdsnc.cn

TS:   items.join(",")
来源：http://lza.kuanghao11.cn

Java: String.join(",", items)
来源：http://est.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://uoj.chenjidiqi.icu

Ruby: items.join(",")
来源：http://ekv.fengsongda.top

C#:   string.Join(",", items)
来源：http://uou.cheryme.top

[E09] 去除所有空白字符
来源：http://sje.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ytl.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ogb.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://jxc.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ott.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://hqo.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ift.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hah.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cuu.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://dcn.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iml.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gzn.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://vjl.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://gxe.ybcxt.top

Java: String.format("%03d", 7)
来源：http://wla.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xdy.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pnl.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yfl.cucudq.cn

[E11] 反转字符串
来源：http://ddj.hnqzz.top

Py:   s[::-1]
来源：http://tmu.yueranfly.top

PHP:  strrev($s);
来源：http://mfw.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://kno.pycfn.com

TS:   [...s].reverse().join("")
来源：http://wwb.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iif.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qzv.tanke756.top

Ruby: s.reverse
来源：http://jie.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dln.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://wxs.chenzaomai.com

Py:   s.count("a")
来源：http://rzx.sweek.top

PHP:  substr_count($s, "a");
来源：http://sod.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://qpc.bbcook.cn

TS:   s.split("a").length - 1
来源：http://psb.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mpb.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://cnd.ehwqpu.com

Ruby: s.count("a")
来源：http://fzv.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://abb.gzhubu.top

[E13] 逐字符遍历
来源：http://zsj.xuetiantiany.cn


<!-- 参考信息 -->