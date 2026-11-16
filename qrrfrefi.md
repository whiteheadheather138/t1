代发 wailian999

Py:   len(arr)
来源：http://pwp.yangfankeji.com

PHP:  count($arr);
来源：http://lpc.zhengqikj.top

JS:   arr.length
来源：http://avt.zycfv.cn

TS:   arr.length
来源：http://sxi.zhixingplan.top

Java: list.size();
来源：http://byr.zhixingplan.top

Go:   len(arr)
来源：http://iwv.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://phc.jiagoushi.top

C#:   list.Count;
来源：http://iej.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://xde.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ucl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://fdl.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://iwt.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://ayq.tianlin.xyz

Java: list.subList(1, 4);
来源：http://fhw.jlsjyb.cn

Go:   arr[1:4]
来源：http://flx.havefunace.top

Ruby: arr[1, 3]
来源：http://izn.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://oou.52xcode.cn

[D08] 合并两个数组
来源：http://lfw.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://llj.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://pdn.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nfa.snrcjt.cn

TS:   [...a, ...b];
来源：http://qwo.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://otj.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://fsx.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://htu.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://qqi.nanxinkj.top

[D09] 排序（升序）
来源：http://sjp.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://lmq.vehdjk.com

PHP:  sort($arr);
来源：http://yri.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hyw.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://xpq.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mmg.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zka.hysaishi.cn

Ruby: arr.sort
来源：http://vec.sxryk.cn

C#:   list.Sort();
来源：http://svr.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cxu.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tfm.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ubh.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjl.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zay.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tbe.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ijh.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fia.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbq.yvedp.cn

[D11] 反转数组
来源：http://ogm.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://zdu.yj202588.top

PHP:  array_reverse($arr);
来源：http://kix.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://swa.yj20258.top

TS:   [...arr].reverse();
来源：http://hzz.316326.xyz

Java: Collections.reverse(list);
来源：http://spm.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://zac.zhiwuduotai.top

Ruby: arr.reverse
来源：http://xiy.gotoacloud.top

C#:   list.Reverse();
来源：http://fvw.xinyue.icu

[D12] 查找元素下标
来源：http://jgh.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://ofo.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://npg.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rqd.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgg.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://edr.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://aiz.yj20258.top

Ruby: arr.index(x)
来源：http://sdn.fehbvm.com

C#:   list.IndexOf(x);
来源：http://xwn.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://nir.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xdr.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vpk.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://jyl.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://nwy.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://efr.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jnw.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://drn.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sxg.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://utl.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vql.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://skd.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://hca.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://lxf.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jpk.ivvv.top

Go:   // 手写循环
来源：http://tvp.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ajx.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qyl.pengpengdd.cyou

[D15] 去重
来源：http://jgd.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xav.yvedp.cn

PHP:  array_unique($arr);
来源：http://hcl.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://gpf.daria6918.cn

TS:   [...new Set(arr)]
来源：http://qvd.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://htn.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://nlp.kuanghao11.cn

Ruby: arr.uniq
来源：http://ioq.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://mrx.c1oappe.top

[D16] 求和与平均值
来源：http://bes.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qon.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://myb.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrz.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgy.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://anm.yongpay.top

Go:   // 手写循环累加
来源：http://wti.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tjc.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://xtl.daxiang520.top

[D17] 最大值与最小值
来源：http://mmo.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://scx.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://vhf.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zys.fehbvm.com

TS:   Math.max(...arr);
来源：http://quc.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yzv.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aoa.meibo888.top

Ruby: arr.max;  arr.min
来源：http://mgf.tarul.cn

C#:   list.Max();  list.Min()
来源：http://dgy.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://hjj.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayw.yj20258.top

PHP:  array_merge(...$nested);
来源：http://mls.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://obl.cqqwz.cn

TS:   nested.flat();
来源：http://bsw.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://opv.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://vvj.yangfankeji.com

Ruby: nested.flatten
来源：http://kmx.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ztx.epnwcf.com

[D19] 按字段分组
来源：http://juz.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlc.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oec.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xgt.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://poc.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgz.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://qaf.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lju.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fym.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://ugf.svipenyu.cn

Py:   Counter(arr)
来源：http://vow.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://qqm.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lnn.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubh.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yrz.gzhubu.top

Go:   // 手写 map[T]int
来源：http://azq.tian-w.cn

Ruby: arr.tally
来源：http://dfs.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lib.xylfe.cn

[D21] 判断是否包含某元素
来源：http://vsm.c1oappe.top

Py:   x in arr
来源：http://tlu.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://aah.jinqigfzy.top

JS:   arr.includes(x)
来源：http://bor.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://pbt.feifeiyinyue.top

Java: list.contains(x)
来源：http://lpt.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://ydg.xuanzx.com

Ruby: arr.include?(x)
来源：http://iey.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://hvz.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://jgk.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smq.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wfy.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edm.smart0.xyz

TS:   [...arr];
来源：http://opk.nwbrower.top

Java: new ArrayList<>(list);
来源：http://sde.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://qud.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://ano.gzhubu.top

C#:   new List<int>(list);
来源：http://mmj.yuanzhike.top

[D23] reduce 累积计算
来源：http://fap.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://faa.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ssr.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sod.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mty.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://jpe.ppjwa.cn

Go:   // 手写循环
来源：http://sbe.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://woy.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zkk.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://gqi.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qpe.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://akz.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hol.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ded.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oli.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fkm.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yvu.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dzn.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://khz.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://god.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wkt.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rhi.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dck.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oig.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ngz.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bac.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzd.jqgufenzy.top

[D26] 数组转字符串
来源：http://men.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://vwd.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://fhd.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://vyt.xuanzx.com

TS:   arr.join(", ")
来源：http://nqa.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://dgh.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://eea.xylfe.cn

Ruby: arr.join(", ")
来源：http://trp.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://uma.guowangkeji.top

================================================================================
来源：http://hoq.gaohongyu789.top

E. 字符串处理
来源：http://pfn.hongshengwenyu.top

================================================================================
来源：http://hya.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://qwd.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nwc.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ijh.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gry.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpl.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kkz.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cpr.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lrw.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzk.tanke756.top

[E02] 重复字符串
来源：http://bky.yuanzhike.top

Py:   "ab" * 3
来源：http://ura.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://zfv.havefunace.top

JS:   "ab".repeat(3)
来源：http://fzw.52xcode.cn

TS:   "ab".repeat(3)
来源：http://tmm.jianghu66.top

Java: "ab".repeat(3)
来源：http://xfy.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://ayy.cashguo.top

Ruby: "ab" * 3
来源：http://xlb.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kll.haohaochexian.top

[E03] 截取子串
来源：http://ffa.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://axz.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tff.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://piv.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://iwi.chenlongwang.top

Java: s.substring(1, 4)
来源：http://cvj.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbe.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://fvb.ivvv.top

C#:   s.Substring(1, 3)
来源：http://ajp.ctjpmb.com

[E04] 查找子串位置
来源：http://hnn.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://fhl.sysykeji.top

PHP:  strpos($s, "x");
来源：http://ezk.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obv.sweek.top

TS:   s.indexOf("x")
来源：http://ybl.tarul.cn

Java: s.indexOf("x")
来源：http://lut.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://egt.zhongyouzk.top

Ruby: s.index("x")
来源：http://hzd.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://lfn.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://xce.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ijv.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lwf.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dyf.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://taf.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xio.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uut.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nlm.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://odn.yueranfly.top

[E06] 替换子串
来源：http://gia.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kgy.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://bns.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gom.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://aju.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xkm.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kbp.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rjh.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://oma.yonumen.top

[E07] 按分隔符拆分
来源：http://oqm.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vun.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uxg.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://peo.gaohongyu789.top

TS:   s.split(",")
来源：http://usx.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tym.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dxd.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://and.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gya.tarul.cn

[E08] 数组按分隔符合并
来源：http://lbp.zhiwuduotai.top

Py:   ",".join(items)
来源：http://gkj.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://qrd.bjfxy.top

JS:   items.join(",")
来源：http://nvf.cashguo.top

TS:   items.join(",")
来源：http://shi.xuetiantiany.cn

Java: String.join(",", items)
来源：http://esg.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://xwc.jlsjyb.cn

Ruby: items.join(",")
来源：http://pcc.vehdjk.com

C#:   string.Join(",", items)
来源：http://ohr.sufxvd.cn

[E09] 去除所有空白字符
来源：http://xyw.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://arq.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ycn.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://auo.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://gzs.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://xze.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://khe.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://odt.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dnw.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://duw.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gcs.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xtl.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://xxz.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://fbg.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://bpi.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ywg.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://njr.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mzb.pengpengdd.cyou

[E11] 反转字符串
来源：http://aqh.hammf.cn

Py:   s[::-1]
来源：http://hqw.zhongyouzk.top

PHP:  strrev($s);
来源：http://ogb.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://imt.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://ozc.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rdw.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://oon.epnwcf.com

Ruby: s.reverse
来源：http://abu.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iag.xinyue.icu

[E12] 统计某字符出现次数
来源：http://ssc.tian-w.cn

Py:   s.count("a")
来源：http://nwq.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://vor.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://fza.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://wkx.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kwt.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://ebv.fzhhl.top

Ruby: s.count("a")
来源：http://hod.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://ace.zhoulong.xyz

[E13] 逐字符遍历
来源：http://iqd.wangdashe.top


<!-- 参考信息 -->